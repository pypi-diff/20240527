# Comparing `tmp/io_file_validator-0.1.4.tar.gz` & `tmp/io_file_validator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "io_file_validator-0.1.4.tar", max compression
+gzip compressed data, was "io_file_validator-0.1.5.tar", max compression
```

## Comparing `io_file_validator-0.1.4.tar` & `io_file_validator-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2440 2024-05-24 04:41:07.385898 io_file_validator-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-05-24 04:41:07.385898 io_file_validator-0.1.4/io_file_validator/__init__.py
--rw-r--r--   0        0        0     3961 2024-05-24 04:41:07.385898 io_file_validator-0.1.4/io_file_validator/validator.py
--rw-r--r--   0        0        0     1056 2024-05-24 04:41:07.385898 io_file_validator-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 io_file_validator-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2440 2024-05-27 03:37:24.189803 io_file_validator-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 03:37:24.189803 io_file_validator-0.1.5/io_file_validator/__init__.py
+-rw-r--r--   0        0        0     4119 2024-05-27 03:37:24.189803 io_file_validator-0.1.5/io_file_validator/validator.py
+-rw-r--r--   0        0        0     1037 2024-05-27 03:37:24.189803 io_file_validator-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 io_file_validator-0.1.5/PKG-INFO
```

### Comparing `io_file_validator-0.1.4/README.md` & `io_file_validator-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `io_file_validator-0.1.4/io_file_validator/validator.py` & `io_file_validator-0.1.5/io_file_validator/validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 from tempfile import NamedTemporaryFile
 
 import pandas as pd
 import pandera as pa
 import requests
 import yaml
 
 
+class UnsupportedFormat(Exception):
+    "File Format Not Specified or Supported"
+
+
 class Validator:
     def __init__(self, file_format) -> None:
         self.file_format = file_format
 
     @staticmethod
     def check_size(my_upload):
-        MAX_FILE_SIZE = 5 * 1024 * 1024  # 5MB
-        if my_upload.size > MAX_FILE_SIZE:
+        max_file_size = 5 * 1024 * 1024  # 5MB
+        if my_upload.size > max_file_size:
             print("The uploaded file is too large. Please upload a file smaller than 5MB.")
 
     @abstractmethod
     def load_and_validate_file(self, my_upload, yaml_content):
         pass
 
     @abstractmethod
@@ -32,15 +36,15 @@
         self._validation_method = "yaml_url"
         self.url = url
 
     @staticmethod
     def fetch_yaml_from_github(url):
         try:
             # Send a GET request to fetch the raw content of the YAML file from GitHub
-            response = requests.get(url)
+            response = requests.get(url, verify=False, timeout=60)
             response.raise_for_status()  # Raise an exception for non-200 status codes
             yaml_content = response.text
             return yaml_content
         except requests.RequestException as e:
             print(f"Error fetching YAML from GitHub: {e}")
             return None
 
@@ -59,25 +63,23 @@
         if yaml_content:
             # Read YAML locally
             yaml_data = self.read_yaml_locally(yaml_content)
             if yaml_data:
                 print("YAML file fetched and read successfully:")
                 print(yaml_data)
                 return yaml_data
-            else:
-                print("Failed to read YAML locally.")
-                return None
-        else:
-            print("Failed to fetch YAML from GitHub.")
+            print("Failed to read YAML locally.")
             return None
+        print("Failed to fetch YAML from GitHub.")
+        return None
 
     @staticmethod
     def write_dict_to_yaml(data, filename):
         try:
-            with open(filename, "w") as yaml_file:
+            with open(filename, "w", encoding="utf-8") as yaml_file:
                 yaml.dump(data, yaml_file, default_flow_style=False)
             print(f"Dictionary successfully written to '{filename}' as YAML.")
         except IOError as e:
             print(f"Error writing YAML file: {e}")
 
     def load_and_validate_file(self, my_upload, yaml_content):
         dataframe = self.read_file(my_upload=my_upload)
@@ -92,21 +94,23 @@
         return validated_df
 
     def read_file(self, my_upload):
         if self.file_format == "json":
             dataframe = pd.read_json(my_upload)
         elif self.file_format == "csv":
             dataframe = pd.read_csv(my_upload)
-
+        else:
+            raise UnsupportedFormat
         return dataframe
 
     def validate(self, dataframe, file_name):
         schema = pa.DataFrameSchema.from_yaml(file_name)
         validated_df = schema.validate(dataframe)
         return validated_df
 
     def run_validation(self, uploaded_file) -> pd.DataFrame:
-        if self._validation_method == "yaml_url":
-            self.check_size(my_upload=uploaded_file)
-            yaml_content = self.get_yaml_content(self.url)
-            validated_df = self.load_and_validate_file(my_upload=uploaded_file, yaml_content=yaml_content)
+        # TODO: add other validation methods
+        # if self._validation_method == "yaml_url":
+        self.check_size(my_upload=uploaded_file)
+        yaml_content = self.get_yaml_content(self.url)
+        validated_df = self.load_and_validate_file(my_upload=uploaded_file, yaml_content=yaml_content)
         return validated_df
```

### Comparing `io_file_validator-0.1.4/pyproject.toml` & `io_file_validator-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "io_file_validator"
-version = "0.1.4"
+version = "0.1.5"
 description = "File Validator Tool helps you validate your data with a plethora of formats"
 authors = ["Manrique Vargas <machomaxg@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 validators = "^0.28.1"
@@ -14,15 +14,14 @@
 pandera = { version = "^0.7.2", extras = ["io"] }
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 pytest = "*"
 pylint = "^3.2.0"
 twine = "*"
-pydiggs = "^0.1.3"
 lxml = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `io_file_validator-0.1.4/PKG-INFO` & `io_file_validator-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: io_file_validator
-Version: 0.1.4
+Version: 0.1.5
 Summary: File Validator Tool helps you validate your data with a plethora of formats
 Author: Manrique Vargas
 Author-email: machomaxg@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

