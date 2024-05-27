# Comparing `tmp/jaanca_utils_os-0.0.1rc2.tar.gz` & `tmp/jaanca_utils_os-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.0.1rc2.tar", last modified: Mon May 27 20:39:23 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.0.1rc3.tar", last modified: Mon May 27 21:24:22 2024, max compression
```

## Comparing `jaanca_utils_os-0.0.1rc2.tar` & `jaanca_utils_os-0.0.1rc3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 20:39:23.170743 jaanca_utils_os-0.0.1rc2/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc2/LICENSE.txt
--rw-rw-rw-   0        0        0     3980 2024-05-27 20:39:23.169745 jaanca_utils_os-0.0.1rc2/PKG-INFO
--rw-rw-rw-   0        0        0     2655 2024-05-27 20:05:31.000000 jaanca_utils_os-0.0.1rc2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 20:39:23.144744 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:39:23.153746 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:39:23.165743 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     2145 2024-05-27 20:38:54.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6701 2024-05-27 17:46:38.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3213 2024-05-27 19:49:12.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:39:23.167762 jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0     3980 2024-05-27 20:39:23.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-05-27 20:39:23.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 20:39:23.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 20:39:23.000000 jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 20:39:23.171744 jaanca_utils_os-0.0.1rc2/setup.cfg
--rw-rw-rw-   0        0        0     1662 2024-05-27 20:39:16.000000 jaanca_utils_os-0.0.1rc2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:24:22.039850 jaanca_utils_os-0.0.1rc3/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3980 2024-05-27 21:24:22.038844 jaanca_utils_os-0.0.1rc3/PKG-INFO
+-rw-rw-rw-   0        0        0     2655 2024-05-27 20:05:31.000000 jaanca_utils_os-0.0.1rc3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 21:24:22.013524 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:24:22.023524 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:24:22.035526 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     2145 2024-05-27 20:38:54.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6786 2024-05-27 21:23:44.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3213 2024-05-27 19:49:12.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:24:22.037525 jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0     3980 2024-05-27 21:24:21.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-05-27 21:24:21.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 21:24:21.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 21:24:21.000000 jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 21:24:22.040853 jaanca_utils_os-0.0.1rc3/setup.cfg
+-rw-rw-rw-   0        0        0     1662 2024-05-27 21:24:16.000000 jaanca_utils_os-0.0.1rc3/setup.py
```

### Comparing `jaanca_utils_os-0.0.1rc2/LICENSE.txt` & `jaanca_utils_os-0.0.1rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc2/PKG-INFO` & `jaanca_utils_os-0.0.1rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.0.1rc2
+Version: 0.0.1rc3
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
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc2 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc3 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `jaanca_utils_os-0.0.1rc2/README.md` & `jaanca_utils_os-0.0.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc2/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.0.1rc3/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/environment_parser_loader.py` & `jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/environment_parser_loader.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,37 +17,35 @@
 
     def __exit__(self, exc_type, exc_value, traceback):
         if self.file:
             self.file.close()
             return False
     
     @classmethod
-    def get_current_folder(self)->str:
-        return os.path.abspath(os.path.join(os.path.dirname(__file__)))
-    
-    @classmethod
-    def build_full_path_from_current_folder(cls,folder_list:list=[])->str:
+    def build_full_path_from_current_folder(cls,path_base:str,folder_list:list=[],filename:str="")->str:
         '''Description
         Create the full path to reach the file or folders structure.
+        :param path_base:str: Use the __file__ parameter, as the path of the current execution file.
 
         ## Example:
         
         ```Phython
         from file_management import FileFolderManagement
 
         # root path
         folder_list = ["folder1", "folder2","file_name"]
-        print(f"Full path from current folder: {FileFolderManagement.build_full_path_from_current_folder()}")
+        print(f"Full path from current folder: {FileFolderManagement.build_full_path_from_current_folder(__file__)}")
 
         # subfolders path from current folder
         folder_list = ["folder1", "folder2","file_name"]
-        print(f"Full path from current folder: {FileFolderManagement.build_full_path_from_current_folder()}")
+        print(f"Full path from current folder: {FileFolderManagement.build_full_path_from_current_folder(__file__)}")
         ```
         '''
-        return os.path.abspath(os.path.join(os.path.dirname(__file__),cls.get_folder_path(folder_list)))
+        folder_path=os.path.abspath(os.path.join(os.path.dirname(path_base),cls.get_folder_path(folder_list)))
+        return os.path.abspath(os.path.join(folder_path,filename))
     
     @classmethod
     def build_full_path_to_file(cls,drive:str, file_name:str, folder_list:list[str]=[])->str:
         '''Description
         Create the full path to reach the file. If filename is empty, returns the full folder path to the file without the filename.
 
         :param: drive str               : Disk letter in windows or mount point in unix, examples: "c:", "d:", "/", "/home"
```

### Comparing `jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc2/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.0.1rc3/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/PKG-INFO` & `jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.0.1rc2
+Version: 0.0.1rc3
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
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc2 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc3 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `jaanca_utils_os-0.0.1rc2/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.0.1rc3/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc2/setup.py` & `jaanca_utils_os-0.0.1rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.0.1rc2"
+VERSION = "0.0.1rc3"
 
 install_requires = [""]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.',
```

