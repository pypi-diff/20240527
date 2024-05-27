# Comparing `tmp/oktmoparser-1.3.1.tar.gz` & `tmp/oktmoparser-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oktmoparser-1.3.1.tar", last modified: Mon May 27 01:10:17 2024, max compression
+gzip compressed data, was "oktmoparser-1.3.2.tar", last modified: Mon May 27 01:27:51 2024, max compression
```

## Comparing `oktmoparser-1.3.1.tar` & `oktmoparser-1.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 01:10:17.270477 oktmoparser-1.3.1/
-drwxrwxrwx   0        0        0        0 2024-05-27 01:10:17.243173 oktmoparser-1.3.1/OktmoParser/
--rw-rw-rw-   0        0        0       20 2024-05-24 06:22:53.000000 oktmoparser-1.3.1/OktmoParser/__init__.py
--rw-rw-rw-   0        0        0     3610 2024-05-27 01:09:50.000000 oktmoparser-1.3.1/OktmoParser/oktmo.py
--rw-rw-rw-   0        0        0     2215 2024-05-27 01:10:17.270477 oktmoparser-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1425 2024-05-24 06:49:31.000000 oktmoparser-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 01:10:17.269399 oktmoparser-1.3.1/oktmoparser.egg-info/
--rw-rw-rw-   0        0        0     2215 2024-05-27 01:10:17.000000 oktmoparser-1.3.1/oktmoparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-05-27 01:10:17.000000 oktmoparser-1.3.1/oktmoparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 01:10:17.000000 oktmoparser-1.3.1/oktmoparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 01:10:17.000000 oktmoparser-1.3.1/oktmoparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-27 01:10:17.000000 oktmoparser-1.3.1/oktmoparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 01:10:17.272577 oktmoparser-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      913 2024-05-27 01:07:21.000000 oktmoparser-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:27:51.874688 oktmoparser-1.3.2/
+drwxrwxrwx   0        0        0        0 2024-05-27 01:27:51.856560 oktmoparser-1.3.2/OktmoParser/
+-rw-rw-rw-   0        0        0       20 2024-05-24 06:22:53.000000 oktmoparser-1.3.2/OktmoParser/__init__.py
+-rw-rw-rw-   0        0        0     3774 2024-05-27 01:24:42.000000 oktmoparser-1.3.2/OktmoParser/oktmo.py
+-rw-rw-rw-   0        0        0     2215 2024-05-27 01:27:51.874688 oktmoparser-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1425 2024-05-24 06:49:31.000000 oktmoparser-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 01:27:51.873688 oktmoparser-1.3.2/oktmoparser.egg-info/
+-rw-rw-rw-   0        0        0     2215 2024-05-27 01:27:51.000000 oktmoparser-1.3.2/oktmoparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-05-27 01:27:51.000000 oktmoparser-1.3.2/oktmoparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 01:27:51.000000 oktmoparser-1.3.2/oktmoparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 01:27:51.000000 oktmoparser-1.3.2/oktmoparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 01:27:51.000000 oktmoparser-1.3.2/oktmoparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 01:27:51.876792 oktmoparser-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      913 2024-05-27 01:27:49.000000 oktmoparser-1.3.2/setup.py
```

### Comparing `oktmoparser-1.3.1/OktmoParser/oktmo.py` & `oktmoparser-1.3.2/OktmoParser/oktmo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import os
+import re
 import csv
 import json
-import re
 import requests
 
 
-class OktmoParser():
+class OktmoParser:
 
     def __init__(self):
         self.url = 'https://rosstat.gov.ru/opendata/7708234640-oktmo'
         self.file_name = 'data.csv'
 
     def parse_oktmo(self, start_keyword, end_keyword):
 
@@ -22,15 +23,16 @@
                 download_url = match.group(1)
                 print(f'Найдена ссылка для скачивания: {download_url}')
 
                 file_response = requests.get(download_url)
 
                 if file_response.status_code == 200:
 
-                    with open(self.file_name, 'wb') as f:
+                    os.makedirs('data/csv/', exist_ok=True)
+                    with open('data/csv/' + self.file_name, 'wb') as f:
                         f.write(file_response.content)
                     print('Файл успешно загружен, формирую результат в формате JSON')
 
                     encoding = 'windows-1251'
                     data_found = False
                     result_data = {}
                     try:
@@ -62,15 +64,16 @@
                                         'ОКТМО': oktmo_code,
                                         'КЧ': row[4]
                                     }
 
                     except UnicodeDecodeError:
                         print(f'Не удалось прочитать файл с кодировкой {encoding}')
 
-                    with open('data/json/result.json', 'w') as json_file:
+                    os.makedirs('data/json/', exist_ok=True)
+                    with open('data/json/result.json', 'w', encoding='utf-8') as json_file:
                         json.dump(result_data, json_file, ensure_ascii=False, indent=4)
                         print('Готово')
                 else:
                     print('Не удалось загрузить файл')
             else:
                 print('Ссылка на файл не найдена')
         else:
```

### Comparing `oktmoparser-1.3.1/PKG-INFO` & `oktmoparser-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oktmoparser
-Version: 1.3.1
+Version: 1.3.2
 Summary: Simple and useful parser that helps you get actual All-Russian Classifier of Municipal Territories (OKTMO)
 Home-page: https://github.com/letimvkocmoc/oktmo-parser
 Author: letimvkocmoc
 Author-email: letimvkocmoc@gmail.com
 Project-URL: GitGub, https://github.com/letimvkocmoc
 Keywords: oktmo parser municipal territory classifier
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `oktmoparser-1.3.1/README.md` & `oktmoparser-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `oktmoparser-1.3.1/oktmoparser.egg-info/PKG-INFO` & `oktmoparser-1.3.2/oktmoparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oktmoparser
-Version: 1.3.1
+Version: 1.3.2
 Summary: Simple and useful parser that helps you get actual All-Russian Classifier of Municipal Territories (OKTMO)
 Home-page: https://github.com/letimvkocmoc/oktmo-parser
 Author: letimvkocmoc
 Author-email: letimvkocmoc@gmail.com
 Project-URL: GitGub, https://github.com/letimvkocmoc
 Keywords: oktmo parser municipal territory classifier
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `oktmoparser-1.3.1/setup.py` & `oktmoparser-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='oktmoparser',
-    version='1.3.1',
+    version='1.3.2',
     author='letimvkocmoc',
     author_email='letimvkocmoc@gmail.com',
     description='Simple and useful parser that helps you get actual All-Russian Classifier of Municipal Territories (OKTMO)',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/letimvkocmoc/oktmo-parser',
     classifiers=[
```

