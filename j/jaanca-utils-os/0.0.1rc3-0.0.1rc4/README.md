# Comparing `tmp/jaanca_utils_os-0.0.1rc3.tar.gz` & `tmp/jaanca_utils_os-0.0.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.0.1rc3.tar", last modified: Mon May 27 21:24:22 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.0.1rc4.tar", last modified: Mon May 27 21:26:36 2024, max compression
```

## Comparing `jaanca_utils_os-0.0.1rc3.tar` & `jaanca_utils_os-0.0.1rc4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 21:24:22.039850 jaanca_utils_os-0.0.1rc3/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc3/LICENSE.txt
--rw-rw-rw-   0        0        0     3980 2024-05-27 21:24:22.038844 jaanca_utils_os-0.0.1rc3/PKG-INFO
--rw-rw-rw-   0        0        0     2655 2024-05-27 20:05:31.000000 jaanca_utils_os-0.0.1rc3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 21:24:22.013524 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 21:24:22.023524 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 21:24:22.035526 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     2145 2024-05-27 20:38:54.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6786 2024-05-27 21:23:44.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3213 2024-05-27 19:49:12.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 21:24:22.037525 jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0     3980 2024-05-27 21:24:21.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-05-27 21:24:21.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 21:24:21.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 21:24:21.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 21:24:22.040853 jaanca_utils_os-0.0.1rc3/setup.cfg
--rw-rw-rw-   0        0        0     1662 2024-05-27 21:24:16.000000 jaanca_utils_os-0.0.1rc3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:26:36.558267 jaanca_utils_os-0.0.1rc4/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3980 2024-05-27 21:26:36.557267 jaanca_utils_os-0.0.1rc4/PKG-INFO
+-rw-rw-rw-   0        0        0     2655 2024-05-27 20:05:31.000000 jaanca_utils_os-0.0.1rc4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 21:26:36.531266 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:26:36.541270 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:26:36.552269 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     2145 2024-05-27 20:38:54.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6786 2024-05-27 21:23:44.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3213 2024-05-27 19:49:12.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:26:36.556268 jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0     3980 2024-05-27 21:26:36.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-05-27 21:26:36.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 21:26:36.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 21:26:36.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 21:26:36.559267 jaanca_utils_os-0.0.1rc4/setup.cfg
+-rw-rw-rw-   0        0        0     1662 2024-05-27 21:26:29.000000 jaanca_utils_os-0.0.1rc4/setup.py
```

### Comparing `jaanca_utils_os-0.0.1rc3/LICENSE.txt` & `jaanca_utils_os-0.0.1rc4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc3/PKG-INFO` & `jaanca_utils_os-0.0.1rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc3 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc4 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `jaanca_utils_os-0.0.1rc3/README.md` & `jaanca_utils_os-0.0.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc3/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.0.1rc4/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/environment_parser_loader.py` & `jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/environment_parser_loader.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/PKG-INFO` & `jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc3 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc4 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc3/setup.py` & `jaanca_utils_os-0.0.1rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.0.1rc3"
+VERSION = "0.0.1rc4"
 
 install_requires = [""]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.',
```

