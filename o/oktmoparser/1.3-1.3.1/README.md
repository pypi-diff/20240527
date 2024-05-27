# Comparing `tmp/oktmoparser-1.3.tar.gz` & `tmp/oktmoparser-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oktmoparser-1.3.tar", last modified: Fri May 24 06:32:19 2024, max compression
+gzip compressed data, was "oktmoparser-1.3.1.tar", last modified: Mon May 27 01:10:17 2024, max compression
```

## Comparing `oktmoparser-1.3.tar` & `oktmoparser-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 06:32:19.870161 oktmoparser-1.3/
-drwxrwxrwx   0        0        0        0 2024-05-24 06:32:19.840725 oktmoparser-1.3/OktmoParser/
--rw-rw-rw-   0        0        0       20 2024-05-24 06:22:53.000000 oktmoparser-1.3/OktmoParser/__init__.py
--rw-rw-rw-   0        0        0     2919 2024-05-24 06:28:18.000000 oktmoparser-1.3/OktmoParser/oktmo.py
--rw-rw-rw-   0        0        0     2169 2024-05-24 06:32:19.869051 oktmoparser-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1379 2024-05-24 05:51:05.000000 oktmoparser-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 06:32:19.866843 oktmoparser-1.3/oktmoparser.egg-info/
--rw-rw-rw-   0        0        0     2169 2024-05-24 06:32:19.000000 oktmoparser-1.3/oktmoparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-05-24 06:32:19.000000 oktmoparser-1.3/oktmoparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 06:32:19.000000 oktmoparser-1.3/oktmoparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-24 06:32:19.000000 oktmoparser-1.3/oktmoparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-24 06:32:19.000000 oktmoparser-1.3/oktmoparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 06:32:19.872312 oktmoparser-1.3/setup.cfg
--rw-rw-rw-   0        0        0      911 2024-05-24 06:31:00.000000 oktmoparser-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:10:17.270477 oktmoparser-1.3.1/
+drwxrwxrwx   0        0        0        0 2024-05-27 01:10:17.243173 oktmoparser-1.3.1/OktmoParser/
+-rw-rw-rw-   0        0        0       20 2024-05-24 06:22:53.000000 oktmoparser-1.3.1/OktmoParser/__init__.py
+-rw-rw-rw-   0        0        0     3610 2024-05-27 01:09:50.000000 oktmoparser-1.3.1/OktmoParser/oktmo.py
+-rw-rw-rw-   0        0        0     2215 2024-05-27 01:10:17.270477 oktmoparser-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1425 2024-05-24 06:49:31.000000 oktmoparser-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 01:10:17.269399 oktmoparser-1.3.1/oktmoparser.egg-info/
+-rw-rw-rw-   0        0        0     2215 2024-05-27 01:10:17.000000 oktmoparser-1.3.1/oktmoparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-05-27 01:10:17.000000 oktmoparser-1.3.1/oktmoparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 01:10:17.000000 oktmoparser-1.3.1/oktmoparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 01:10:17.000000 oktmoparser-1.3.1/oktmoparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 01:10:17.000000 oktmoparser-1.3.1/oktmoparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 01:10:17.272577 oktmoparser-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      913 2024-05-27 01:07:21.000000 oktmoparser-1.3.1/setup.py
```

### Comparing `oktmoparser-1.3/OktmoParser/oktmo.py` & `oktmoparser-1.3.1/OktmoParser/oktmo.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,35 +30,47 @@
                         f.write(file_response.content)
                     print('Файл успешно загружен, формирую результат в формате JSON')
 
                     encoding = 'windows-1251'
                     data_found = False
                     result_data = {}
                     try:
-                        with open('data.csv', newline='', encoding=encoding) as csvfile:
+                        with open('data/csv/data.csv', newline='', encoding=encoding) as csvfile:
                             csvreader = csv.reader(csvfile, delimiter=';')
+
                             for row in csvreader:
-                                if data_found and row[6] != end_keyword:
+                                if start_keyword and end_keyword:
+                                    if row[6] == start_keyword:
+                                        data_found = True
+                                    elif row[6] == end_keyword:
+                                        data_found = False
+                                        break
+                                    if data_found and row[6] != end_keyword:
+                                        oktmo_code = row[0] + ' ' + row[1] + ' ' + row[2]
+                                        if row[3] != '000':
+                                            oktmo_code += ' ' + row[3]
+                                        settlement_name = row[6]
+                                        result_data[settlement_name] = {
+                                            'ОКТМО': oktmo_code,
+                                            'КЧ': row[4]
+                                        }
+                                else:
                                     oktmo_code = row[0] + ' ' + row[1] + ' ' + row[2]
                                     if row[3] != '000':
                                         oktmo_code += ' ' + row[3]
                                     settlement_name = row[6]
                                     result_data[settlement_name] = {
                                         'ОКТМО': oktmo_code,
                                         'КЧ': row[4]
                                     }
-                                if row[6] == start_keyword:
-                                    data_found = True
-                                elif row[6] == end_keyword:
-                                    data_found = False
-                                    break
+
                     except UnicodeDecodeError:
                         print(f'Не удалось прочитать файл с кодировкой {encoding}')
 
-                    with open('result.json', 'w') as json_file:
+                    with open('data/json/result.json', 'w') as json_file:
                         json.dump(result_data, json_file, ensure_ascii=False, indent=4)
                         print('Готово')
                 else:
                     print('Не удалось загрузить файл')
             else:
                 print('Ссылка на файл не найдена')
         else:
```

### Comparing `oktmoparser-1.3/PKG-INFO` & `oktmoparser-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oktmoparser
-Version: 1.3
+Version: 1.3.1
 Summary: Simple and useful parser that helps you get actual All-Russian Classifier of Municipal Territories (OKTMO)
 Home-page: https://github.com/letimvkocmoc/oktmo-parser
 Author: letimvkocmoc
 Author-email: letimvkocmoc@gmail.com
 Project-URL: GitGub, https://github.com/letimvkocmoc
 Keywords: oktmo parser municipal territory classifier
 Classifier: Programming Language :: Python :: 3.12
@@ -14,14 +14,17 @@
 Requires-Dist: requests
 
 # All-Russian Classifier of Municipal Territories (OKTMO) Parser #
 
 ## What is this? ##
 Simple and useful parser that helps you get actual All-Russian Classifier of Municipal Territories (OKTMO).
 
+## Install ##
+`pip install oktmoparser`
+
 ## Quick Guide ##
 The parser is based on the following structure:
 
     parser = OktmoParser()
     start_keyword = ''
     end_keyword = ''
     parser.parse_oktmo(start_keyword, end_keyword)
```

### Comparing `oktmoparser-1.3/README.md` & `oktmoparser-1.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # All-Russian Classifier of Municipal Territories (OKTMO) Parser #
 
 ## What is this? ##
 Simple and useful parser that helps you get actual All-Russian Classifier of Municipal Territories (OKTMO).
 
+## Install ##
+`pip install oktmoparser`
+
 ## Quick Guide ##
 The parser is based on the following structure:
 
     parser = OktmoParser()
     start_keyword = ''
     end_keyword = ''
     parser.parse_oktmo(start_keyword, end_keyword)
@@ -48,8 +51,8 @@
 5. That's it.
 
 
 ----------
 
 
 ## Developer ##
-[@letimvkocmoc](https://github.com/letimvkocmoc/) 
+[@letimvkocmoc](https://github.com/letimvkocmoc/)
```

### Comparing `oktmoparser-1.3/oktmoparser.egg-info/PKG-INFO` & `oktmoparser-1.3.1/oktmoparser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oktmoparser
-Version: 1.3
+Version: 1.3.1
 Summary: Simple and useful parser that helps you get actual All-Russian Classifier of Municipal Territories (OKTMO)
 Home-page: https://github.com/letimvkocmoc/oktmo-parser
 Author: letimvkocmoc
 Author-email: letimvkocmoc@gmail.com
 Project-URL: GitGub, https://github.com/letimvkocmoc
 Keywords: oktmo parser municipal territory classifier
 Classifier: Programming Language :: Python :: 3.12
@@ -14,14 +14,17 @@
 Requires-Dist: requests
 
 # All-Russian Classifier of Municipal Territories (OKTMO) Parser #
 
 ## What is this? ##
 Simple and useful parser that helps you get actual All-Russian Classifier of Municipal Territories (OKTMO).
 
+## Install ##
+`pip install oktmoparser`
+
 ## Quick Guide ##
 The parser is based on the following structure:
 
     parser = OktmoParser()
     start_keyword = ''
     end_keyword = ''
     parser.parse_oktmo(start_keyword, end_keyword)
```

### Comparing `oktmoparser-1.3/setup.py` & `oktmoparser-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='oktmoparser',
-    version='1.3',
+    version='1.3.1',
     author='letimvkocmoc',
     author_email='letimvkocmoc@gmail.com',
     description='Simple and useful parser that helps you get actual All-Russian Classifier of Municipal Territories (OKTMO)',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/letimvkocmoc/oktmo-parser',
     classifiers=[
```

