# Comparing `tmp/fastmrz-1.1.tar.gz` & `tmp/fastmrz-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmrz-1.1.tar", last modified: Sun May 12 14:00:51 2024, max compression
+gzip compressed data, was "fastmrz-1.2.tar", last modified: Mon May 27 19:56:08 2024, max compression
```

## Comparing `fastmrz-1.1.tar` & `fastmrz-1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 14:00:51.058173 fastmrz-1.1/
--rw-rw-rw-   0        0        0    35184 2024-03-31 11:40:54.000000 fastmrz-1.1/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-08 11:27:20.000000 fastmrz-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7491 2024-05-12 14:00:51.057021 fastmrz-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4887 2024-05-12 08:09:25.000000 fastmrz-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 14:00:51.044569 fastmrz-1.1/fastmrz/
--rw-rw-rw-   0        0        0       62 2024-04-07 16:27:29.000000 fastmrz-1.1/fastmrz/__init__.py
--rw-rw-rw-   0        0        0     9375 2024-05-12 08:11:25.000000 fastmrz-1.1/fastmrz/fastmrz.py
--rw-rw-rw-   0        0        0      498 2024-05-12 08:19:01.000000 fastmrz-1.1/fastmrz/main.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:00:51.050085 fastmrz-1.1/fastmrz/model/
--rw-rw-rw-   0        0        0  5254428 2024-03-31 11:40:54.000000 fastmrz-1.1/fastmrz/model/mrz_seg.tflite
-drwxrwxrwx   0        0        0        0 2024-05-12 14:00:51.049075 fastmrz-1.1/fastmrz.egg-info/
--rw-rw-rw-   0        0        0     7491 2024-05-12 14:00:50.000000 fastmrz-1.1/fastmrz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-12 14:00:50.000000 fastmrz-1.1/fastmrz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 14:00:50.000000 fastmrz-1.1/fastmrz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      688 2024-05-12 14:00:50.000000 fastmrz-1.1/fastmrz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-12 14:00:50.000000 fastmrz-1.1/fastmrz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 14:00:51.058173 fastmrz-1.1/setup.cfg
--rw-rw-rw-   0        0        0     2729 2024-05-12 14:00:27.000000 fastmrz-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:00:51.055623 fastmrz-1.1/tests/
--rw-rw-rw-   0        0        0     2172 2024-04-07 16:29:57.000000 fastmrz-1.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-27 19:56:08.836139 fastmrz-1.2/
+-rw-rw-rw-   0        0        0    35184 2024-03-31 11:40:54.000000 fastmrz-1.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-08 11:27:20.000000 fastmrz-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7491 2024-05-27 19:56:08.834139 fastmrz-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4887 2024-05-12 08:09:25.000000 fastmrz-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 19:56:08.811139 fastmrz-1.2/fastmrz/
+-rw-rw-rw-   0        0        0       62 2024-04-07 16:27:29.000000 fastmrz-1.2/fastmrz/__init__.py
+-rw-rw-rw-   0        0        0    10806 2024-05-27 19:51:28.000000 fastmrz-1.2/fastmrz/fastmrz.py
+-rw-rw-rw-   0        0        0      498 2024-05-12 08:19:01.000000 fastmrz-1.2/fastmrz/main.py
+drwxrwxrwx   0        0        0        0 2024-05-27 19:56:08.823140 fastmrz-1.2/fastmrz/model/
+-rw-rw-rw-   0        0        0  5254428 2024-03-31 11:40:54.000000 fastmrz-1.2/fastmrz/model/mrz_seg.tflite
+drwxrwxrwx   0        0        0        0 2024-05-27 19:56:08.821139 fastmrz-1.2/fastmrz.egg-info/
+-rw-rw-rw-   0        0        0     7491 2024-05-27 19:56:08.000000 fastmrz-1.2/fastmrz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-27 19:56:08.000000 fastmrz-1.2/fastmrz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 19:56:08.000000 fastmrz-1.2/fastmrz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      688 2024-05-27 19:56:08.000000 fastmrz-1.2/fastmrz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 19:56:08.000000 fastmrz-1.2/fastmrz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 19:56:08.836139 fastmrz-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2729 2024-05-27 19:53:24.000000 fastmrz-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 19:56:08.831139 fastmrz-1.2/tests/
+-rw-rw-rw-   0        0        0     2172 2024-04-07 16:29:57.000000 fastmrz-1.2/tests/test.py
```

### Comparing `fastmrz-1.1/LICENSE` & `fastmrz-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmrz-1.1/PKG-INFO` & `fastmrz-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmrz
-Version: 1.1
+Version: 1.2
 Summary: Extracts the Machine Readable Zone (MRZ) data from document images
 Home-page: https://github.com/sivakumar-mahalingam/fastmrz
 Author: Sivakumar Mahalingam
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastmrz Version: 1.1 Summary: Extracts the Machine
+Metadata-Version: 2.1 Name: fastmrz Version: 1.2 Summary: Extracts the Machine
 Readable Zone (MRZ) data from document images Home-page: https://github.com/
 sivakumar-mahalingam/fastmrz Author: Sivakumar Mahalingam Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 or later (AGPLv3+) Classifier: Programming Language
 :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `fastmrz-1.1/README.md` & `fastmrz-1.2/README.md`

 * *Files identical despite different names*

### Comparing `fastmrz-1.1/fastmrz/fastmrz.py` & `fastmrz-1.2/fastmrz/fastmrz.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,19 +57,20 @@
 
         selection_length = None
         for item in input_list:
             if '<' in item and len(item) in (30, 36, 44):
                 selection_length = len(item)
                 break
 
-        new_list = [item for item in input_list if len(item) >= selection_length]
-
-        output_text = '\n'.join(new_list)
-
-        return output_text
+        if selection_length is None:
+            return ''
+        else:
+            new_list = [item for item in input_list if len(item) >= selection_length]
+            output_text = '\n'.join(new_list)
+            return output_text
 
     def _get_final_check_digit(self, input_string, input_type):
         if input_type == 'TD3':
             return self._get_check_digit(input_string[0:10] + input_string[13:20] + input_string[21:43])
         elif input_type == 'TD2':
             return self._get_check_digit(input_string[0:10] + input_string[13:20] + input_string[21:35])
         else:
@@ -124,44 +125,60 @@
         file_status = self._is_valid_file(image_path)
         if image_path == file_status:
             mrz_text = self.get_raw_mrz(image_path)
             return self._parse_mrz(mrz_text)
         else:
             return {'status': 'FAILURE', 'message': file_status}
 
+    def _get_date_of_birth(self, date_of_birth_str, date_of_expiry_str):
+        birth_year = int(date_of_birth_str[:4])
+        expiry_year = int(date_of_expiry_str[:4])
+
+        if expiry_year <= birth_year:
+            adjusted_year = birth_year - 100
+            return f"{adjusted_year}-{date_of_birth_str[5:]}"
+        else:
+            return date_of_birth_str
+
     def _parse_mrz(self, mrz_text):
         mrz_lines = mrz_text.strip().split('\n')
         if len(mrz_lines) not in [2, 3]:
             return {'status': 'FAILURE', 'message': 'Invalid MRZ format'}
 
         mrz_code_dict = {}
         if len(mrz_lines) == 2:
             mrz_code_dict['mrz_type'] = 'TD2' if len(mrz_lines[0]) == 36 else 'TD3'
 
             # Line 1
             mrz_code_dict['document_type'] = mrz_lines[0][:2].strip('<')
             mrz_code_dict['country_code'] = mrz_lines[0][2:5]
+            if not mrz_code_dict['country_code'].isalpha():
+                return {'status': 'FAILURE', 'message': 'Invalid MRZ format'}
             names = mrz_lines[0][5:].split('<<')
             mrz_code_dict['surname'] = names[0].replace('<', ' ')
             mrz_code_dict['given_name'] = names[1].replace('<', ' ')
 
             # Line 2
             mrz_code_dict['document_number'] = mrz_lines[1][0:9].replace('<', '')
             if self._get_check_digit(mrz_code_dict['document_number']) != mrz_lines[1][9]:
                 return {'status': 'FAILURE', 'message': 'document number checksum is not matching'}
             mrz_code_dict['nationality'] = mrz_lines[1][10:13]
+            if not mrz_code_dict['nationality'].isalpha():
+                return {'status': 'FAILURE', 'message': 'Invalid MRZ format'}
             mrz_code_dict['date_of_birth'] = mrz_lines[1][13:19]
             if self._get_check_digit(mrz_code_dict['date_of_birth']) != mrz_lines[1][19]:
                 return {'status': 'FAILURE', 'message': 'date of birth checksum is not matching'}
             mrz_code_dict['date_of_birth'] = self._format_date(mrz_code_dict['date_of_birth'])
             mrz_code_dict['sex'] = mrz_lines[1][20]
             mrz_code_dict['date_of_expiry'] = mrz_lines[1][21:27]
             if self._get_check_digit(mrz_code_dict['date_of_expiry']) != mrz_lines[1][27]:
                 return {'status': 'FAILURE', 'message': 'date of expiry checksum is not matching'}
             mrz_code_dict['date_of_expiry'] = self._format_date(mrz_code_dict['date_of_expiry'])
+            mrz_code_dict['date_of_birth'] = self._get_date_of_birth(mrz_code_dict['date_of_birth'],
+                                                                     mrz_code_dict['date_of_expiry'])
             if mrz_code_dict['mrz_type'] == 'TD3':
                 mrz_code_dict['optional_data'] = mrz_lines[1][28:35].strip('<')
 
             mrz_code_dict['optional_data'] = mrz_lines[1][28:35].strip('<') if mrz_code_dict['mrz_type'] == 'TD2' else mrz_lines[1][28:42].strip('<')
             if mrz_lines[1][-1] != self._get_final_check_digit(mrz_lines[1], mrz_code_dict['mrz_type']):
                 return {'status': 'FAILURE', 'message': 'final checksum is not matching'}
 
@@ -169,14 +186,16 @@
             mrz_code_dict['status'] = 'SUCCESS'
         else:
             mrz_code_dict['mrz_type'] = 'TD1'
 
             # Line 1
             mrz_code_dict['document_type'] = mrz_lines[0][:2].strip('<')
             mrz_code_dict['country_code'] = mrz_lines[0][2:5]
+            if not mrz_code_dict['country_code'].isalpha():
+                return {'status': 'FAILURE', 'message': 'Invalid MRZ format'}
             mrz_code_dict['document_number'] = mrz_lines[0][5:14]
             if self._get_check_digit(mrz_code_dict['document_number']) != mrz_lines[0][14]:
                 return {'status': 'FAILURE', 'message': 'document number checksum is not matching'}
             mrz_code_dict['optional_data_1'] = mrz_lines[0][15:].strip('<')
 
             # Line 2
             mrz_code_dict['date_of_birth'] = mrz_lines[1][:6]
@@ -184,15 +203,19 @@
                 return {'status': 'FAILURE', 'message': 'date of birth checksum is not matching'}
             mrz_code_dict['date_of_birth'] = self._format_date(mrz_code_dict['date_of_birth'])
             mrz_code_dict['sex'] = mrz_lines[1][7]
             mrz_code_dict['date_of_expiry'] = mrz_lines[1][8:14]
             if self._get_check_digit(mrz_code_dict['date_of_expiry']) != mrz_lines[1][14]:
                 return {'status': 'FAILURE', 'message': 'date of expiry checksum is not matching'}
             mrz_code_dict['date_of_expiry'] = self._format_date(mrz_code_dict['date_of_expiry'])
+            mrz_code_dict['date_of_birth'] = self._get_date_of_birth(mrz_code_dict['date_of_birth'],
+                                                                     mrz_code_dict['date_of_expiry'])
             mrz_code_dict['nationality'] = mrz_lines[1][15:18]
+            if not mrz_code_dict['nationality'].isalpha():
+                return {'status': 'FAILURE', 'message': 'Invalid MRZ format'}
             mrz_code_dict['optional_data_2'] = mrz_lines[0][18:29].strip('<')
             if mrz_lines[1][-1] != self._get_final_check_digit(mrz_lines, mrz_code_dict['mrz_type']):
                 return {'status': 'FAILURE', 'message': 'final checksum is not matching'}
 
             # Line 3
             names = mrz_lines[2].split('<<')
             mrz_code_dict['surname'] = names[0].replace('<', ' ')
```

### Comparing `fastmrz-1.1/fastmrz/model/mrz_seg.tflite` & `fastmrz-1.2/fastmrz/model/mrz_seg.tflite`

 * *Files identical despite different names*

### Comparing `fastmrz-1.1/fastmrz.egg-info/PKG-INFO` & `fastmrz-1.2/fastmrz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmrz
-Version: 1.1
+Version: 1.2
 Summary: Extracts the Machine Readable Zone (MRZ) data from document images
 Home-page: https://github.com/sivakumar-mahalingam/fastmrz
 Author: Sivakumar Mahalingam
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastmrz Version: 1.1 Summary: Extracts the Machine
+Metadata-Version: 2.1 Name: fastmrz Version: 1.2 Summary: Extracts the Machine
 Readable Zone (MRZ) data from document images Home-page: https://github.com/
 sivakumar-mahalingam/fastmrz Author: Sivakumar Mahalingam Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 or later (AGPLv3+) Classifier: Programming Language
 :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `fastmrz-1.1/fastmrz.egg-info/requires.txt` & `fastmrz-1.2/fastmrz.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fastmrz-1.1/setup.py` & `fastmrz-1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r', encoding='utf8') as f:
     long_description = f.read()
 
 
 setup(
     name='fastmrz',
-    version='1.1',
+    version='1.2',
     author='Sivakumar Mahalingam',
     description='Extracts the Machine Readable Zone (MRZ) data from document images',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sivakumar-mahalingam/fastmrz',
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `fastmrz-1.1/tests/test.py` & `fastmrz-1.2/tests/test.py`

 * *Files identical despite different names*

