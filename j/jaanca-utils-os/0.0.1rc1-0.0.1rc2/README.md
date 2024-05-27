# Comparing `tmp/jaanca_utils_os-0.0.1rc1.tar.gz` & `tmp/jaanca_utils_os-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.0.1rc1.tar", last modified: Mon May 27 20:34:40 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.0.1rc2.tar", last modified: Mon May 27 20:39:23 2024, max compression
```

## Comparing `jaanca_utils_os-0.0.1rc1.tar` & `jaanca_utils_os-0.0.1rc2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 20:34:40.244175 jaanca_utils_os-0.0.1rc1/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc1/LICENSE.txt
--rw-rw-rw-   0        0        0     3980 2024-05-27 20:34:40.243172 jaanca_utils_os-0.0.1rc1/PKG-INFO
--rw-rw-rw-   0        0        0     2655 2024-05-27 20:05:31.000000 jaanca_utils_os-0.0.1rc1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 20:34:40.217173 jaanca_utils_os-0.0.1rc1/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc1/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:34:40.228170 jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:34:40.240171 jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     2129 2024-05-27 20:29:05.000000 jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6701 2024-05-27 17:46:38.000000 jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3213 2024-05-27 19:49:12.000000 jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1207 2024-05-27 15:10:36.000000 jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:34:40.242172 jaanca_utils_os-0.0.1rc1/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0     3980 2024-05-27 20:34:40.000000 jaanca_utils_os-0.0.1rc1/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-05-27 20:34:40.000000 jaanca_utils_os-0.0.1rc1/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 20:34:40.000000 jaanca_utils_os-0.0.1rc1/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 20:34:40.000000 jaanca_utils_os-0.0.1rc1/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 20:34:40.245174 jaanca_utils_os-0.0.1rc1/setup.cfg
--rw-rw-rw-   0        0        0     1662 2024-05-27 20:34:34.000000 jaanca_utils_os-0.0.1rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:39:23.170743 jaanca_utils_os-0.0.1rc2/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3980 2024-05-27 20:39:23.169745 jaanca_utils_os-0.0.1rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     2655 2024-05-27 20:05:31.000000 jaanca_utils_os-0.0.1rc2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 20:39:23.144744 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:39:23.153746 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:39:23.165743 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     2145 2024-05-27 20:38:54.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6701 2024-05-27 17:46:38.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3213 2024-05-27 19:49:12.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:39:23.167762 jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0     3980 2024-05-27 20:39:23.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-05-27 20:39:23.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 20:39:23.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 20:39:23.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 20:39:23.171744 jaanca_utils_os-0.0.1rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1662 2024-05-27 20:39:16.000000 jaanca_utils_os-0.0.1rc2/setup.py
```

### Comparing `jaanca_utils_os-0.0.1rc1/LICENSE.txt` & `jaanca_utils_os-0.0.1rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc1/PKG-INFO` & `jaanca_utils_os-0.0.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.0.1rc1
+Version: 0.0.1rc2
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
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc1 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc2 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `jaanca_utils_os-0.0.1rc1/README.md` & `jaanca_utils_os-0.0.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc1/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.0.1rc2/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/helpers/environment_parser_loader.py` & `jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/environment_parser_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import StrEnum
 from pathlib import Path
-from utils.helpers.parse_types import parse_types
+from jaanca_utils_os.utils.helpers.parse_types import parse_types
 import os
 
 class EnvironmentParserLoaderErrorCodes:
     class KeyErrors(StrEnum):
         VARIABLES_HAVE_NOT_BEEN_CREATED = "The following environment variables have not been created or assigned a default value: {}"
     class Dependencies(StrEnum):
         DOTENV = "I need the python-dotenv>=1.0.0 library to work."
```

### Comparing `jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc1/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils.helpers.parse_bool import parse_bool
+from jaanca_utils_os.utils.helpers.parse_bool import parse_bool
 import ast
 import json
 
 def is_float(value:str):
     try:
         float(value)
         return True
```

### Comparing `jaanca_utils_os-0.0.1rc1/jaanca_utils_os.egg-info/PKG-INFO` & `jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.0.1rc1
+Version: 0.0.1rc2
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
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc1 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc2 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `jaanca_utils_os-0.0.1rc1/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc1/setup.py` & `jaanca_utils_os-0.0.1rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.0.1rc1"
+VERSION = "0.0.1rc2"
 
 install_requires = [""]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.',
```

