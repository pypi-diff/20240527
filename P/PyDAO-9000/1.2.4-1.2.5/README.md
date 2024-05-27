# Comparing `tmp/PyDAO_9000-1.2.4.tar.gz` & `tmp/pydao_9000-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDAO_9000-1.2.4.tar", last modified: Tue Aug 15 18:08:04 2023, max compression
+gzip compressed data, was "pydao_9000-1.2.5.tar", last modified: Mon May 27 12:37:46 2024, max compression
```

## Comparing `PyDAO_9000-1.2.4.tar` & `pydao_9000-1.2.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-08-15 18:08:04.933840 PyDAO_9000-1.2.4/
--rw-rw-rw-   0        0        0     1090 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/LICENSE
--rw-rw-rw-   0        0        0     4328 2023-08-15 18:08:04.933840 PyDAO_9000-1.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-15 18:08:04.824468 PyDAO_9000-1.2.4/PyDAO_9000.egg-info/
--rw-rw-rw-   0        0        0     4328 2023-08-15 18:08:04.000000 PyDAO_9000-1.2.4/PyDAO_9000.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2023-08-15 18:08:04.000000 PyDAO_9000-1.2.4/PyDAO_9000.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-15 18:08:04.000000 PyDAO_9000-1.2.4/PyDAO_9000.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-15 18:08:04.000000 PyDAO_9000-1.2.4/PyDAO_9000.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3810 2023-08-15 17:28:32.000000 PyDAO_9000-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-15 18:08:04.855715 PyDAO_9000-1.2.4/SqltDAO/
-drwxrwxrwx   0        0        0        0 2023-08-15 18:08:04.871348 PyDAO_9000-1.2.4/SqltDAO/CodeGen01/
--rw-rw-rw-   0        0        0     3108 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/CodeGen01/CodeGen.py
--rw-rw-rw-   0        0        0      865 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/CodeGen01/CodeLevel.py
--rw-rw-rw-   0        0        0      264 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/CodeGen01/DaoExceptions.py
--rw-rw-rw-   0        0        0      478 2023-08-15 17:53:30.000000 PyDAO_9000-1.2.4/SqltDAO/CodeGen01/Meta.py
--rw-rw-rw-   0        0        0     1816 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/CodeGen01/Normalizers.py
--rw-rw-rw-   0        0        0     4309 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/CodeGen01/OrderClass.py
--rw-rw-rw-   0        0        0    12415 2023-06-03 13:14:31.000000 PyDAO_9000-1.2.4/SqltDAO/CodeGen01/SqlSyntax.py
--rw-rw-rw-   0        0        0     7315 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/CodeGen01/TextDataDetector.py
--rw-rw-rw-   0        0        0    13912 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/CrudMeister.py
-drwxrwxrwx   0        0        0        0 2023-08-15 18:08:04.902593 PyDAO_9000-1.2.4/SqltDAO/DaoTest01/
--rw-rw-rw-   0        0        0      678 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/DaoTest01/GenNasdaq.py
--rw-rw-rw-   0        0        0      507 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/DaoTest01/GenNasdaqTest.py
--rw-rw-rw-   0        0        0     3252 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/DaoTest01/Income.py
--rw-rw-rw-   0        0        0     3054 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/DaoTest01/NasdaqDAO.py
--rw-rw-rw-   0        0        0     3488 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/DaoTest01/foo.py
--rw-rw-rw-   0        0        0      847 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/DaoTest01/tc001_driver.py
--rw-rw-rw-   0        0        0      691 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/DaoTest01/tc001_gen.py
--rw-rw-rw-   0        0        0     2923 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/Demo123.py
-drwxrwxrwx   0        0        0        0 2023-08-15 18:08:04.918220 PyDAO_9000-1.2.4/SqltDAO/Gui/
--rw-rw-rw-   0        0        0     6185 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/Gui/Data2Code.py
--rw-rw-rw-   0        0        0     6553 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/Gui/DataAI.py
--rw-rw-rw-   0        0        0     4628 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/Gui/DataFrameOne.py
--rw-rw-rw-   0        0        0     4934 2023-08-15 17:33:54.000000 PyDAO_9000-1.2.4/SqltDAO/Gui/DataPreferences.py
--rw-rw-rw-   0        0        0     4771 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/Gui/StandardEntry.py
--rw-rw-rw-   0        0        0     6403 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/Gui/TableDef.py
--rw-rw-rw-   0        0        0     3504 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/Ledger.py
--rw-rw-rw-   0        0        0      293 2023-08-15 18:02:09.000000 PyDAO_9000-1.2.4/SqltDAO/MainGUI.py
-drwxrwxrwx   0        0        0        0 2023-08-15 18:08:04.918220 PyDAO_9000-1.2.4/SqltDAO/SchemaDef/
--rw-rw-rw-   0        0        0     8393 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/SchemaDef/DataDetective.py
--rw-rw-rw-   0        0        0     9378 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/SchemaDef/Factory.py
--rw-rw-rw-   0        0        0     8987 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/SchemaDef/OrderDef.py
--rw-rw-rw-   0        0        0     3179 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/SchemaDef/Table.py
--rw-rw-rw-   0        0        0     3602 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.4/SqltDAO/UpdateTestCase.py
--rw-rw-rw-   0        0        0      300 2023-08-15 17:24:38.000000 PyDAO_9000-1.2.4/SqltDAO/__init__.py
--rw-rw-rw-   0        0        0     7751 2023-06-03 13:21:45.000000 PyDAO_9000-1.2.4/SqltDAO/main.py
--rw-rw-rw-   0        0        0      506 2023-08-15 17:53:03.000000 PyDAO_9000-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-15 18:08:04.933840 PyDAO_9000-1.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 12:37:46.326426 pydao_9000-1.2.5/
+-rw-rw-rw-   0        0        0     1090 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0     4281 2024-05-27 12:37:46.326426 pydao_9000-1.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 12:37:46.326426 pydao_9000-1.2.5/PyDAO_9000.egg-info/
+-rw-rw-rw-   0        0        0     4281 2024-05-27 12:37:45.000000 pydao_9000-1.2.5/PyDAO_9000.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1059 2024-05-27 12:37:45.000000 pydao_9000-1.2.5/PyDAO_9000.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 12:37:45.000000 pydao_9000-1.2.5/PyDAO_9000.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 12:37:45.000000 pydao_9000-1.2.5/PyDAO_9000.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3763 2024-05-24 05:53:56.000000 pydao_9000-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 12:37:46.076428 pydao_9000-1.2.5/SqltDAO/
+drwxrwxrwx   0        0        0        0 2024-05-27 12:37:46.154549 pydao_9000-1.2.5/SqltDAO/CodeGen01/
+-rw-rw-rw-   0        0        0     3108 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/CodeGen01/CodeGen.py
+-rw-rw-rw-   0        0        0      865 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/CodeGen01/CodeLevel.py
+-rw-rw-rw-   0        0        0      264 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/CodeGen01/DaoExceptions.py
+-rw-rw-rw-   0        0        0      478 2024-05-24 06:02:20.000000 pydao_9000-1.2.5/SqltDAO/CodeGen01/Meta.py
+-rw-rw-rw-   0        0        0     1816 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/CodeGen01/Normalizers.py
+-rw-rw-rw-   0        0        0     4309 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/CodeGen01/OrderClass.py
+-rw-rw-rw-   0        0        0    13458 2024-05-27 12:23:52.000000 pydao_9000-1.2.5/SqltDAO/CodeGen01/SqlSyntax.py
+-rw-rw-rw-   0        0        0     7315 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/CodeGen01/TextDataDetector.py
+-rw-rw-rw-   0        0        0    13912 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/CrudMeister.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:37:46.232680 pydao_9000-1.2.5/SqltDAO/DaoTest01/
+-rw-rw-rw-   0        0        0      678 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/DaoTest01/GenNasdaq.py
+-rw-rw-rw-   0        0        0      507 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/DaoTest01/GenNasdaqTest.py
+-rw-rw-rw-   0        0        0     3252 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/DaoTest01/Income.py
+-rw-rw-rw-   0        0        0     3054 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/DaoTest01/NasdaqDAO.py
+-rw-rw-rw-   0        0        0     3488 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/DaoTest01/foo.py
+-rw-rw-rw-   0        0        0      847 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/DaoTest01/tc001_driver.py
+-rw-rw-rw-   0        0        0      691 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/DaoTest01/tc001_gen.py
+-rw-rw-rw-   0        0        0     2926 2024-05-24 05:53:56.000000 pydao_9000-1.2.5/SqltDAO/Demo123.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:37:46.279552 pydao_9000-1.2.5/SqltDAO/Gui/
+-rw-rw-rw-   0        0        0     6185 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/Gui/Data2Code.py
+-rw-rw-rw-   0        0        0     6553 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/Gui/DataAI.py
+-rw-rw-rw-   0        0        0     4628 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/Gui/DataFrameOne.py
+-rw-rw-rw-   0        0        0     4934 2023-08-15 17:33:54.000000 pydao_9000-1.2.5/SqltDAO/Gui/DataPreferences.py
+-rw-rw-rw-   0        0        0     4771 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/Gui/StandardEntry.py
+-rw-rw-rw-   0        0        0     6403 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/Gui/TableDef.py
+-rw-rw-rw-   0        0        0     3504 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/Ledger.py
+-rw-rw-rw-   0        0        0      368 2024-05-27 12:35:24.000000 pydao_9000-1.2.5/SqltDAO/MainGUI.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:37:46.310805 pydao_9000-1.2.5/SqltDAO/SchemaDef/
+-rw-rw-rw-   0        0        0     8393 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/SchemaDef/DataDetective.py
+-rw-rw-rw-   0        0        0     9378 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/SchemaDef/Factory.py
+-rw-rw-rw-   0        0        0     8987 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/SchemaDef/OrderDef.py
+-rw-rw-rw-   0        0        0     3179 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/SchemaDef/Table.py
+-rw-rw-rw-   0        0        0     3602 2023-05-27 11:01:18.000000 pydao_9000-1.2.5/SqltDAO/UpdateTestCase.py
+-rw-rw-rw-   0        0        0      300 2023-08-15 17:24:38.000000 pydao_9000-1.2.5/SqltDAO/__init__.py
+-rw-rw-rw-   0        0        0     7751 2023-06-03 13:21:45.000000 pydao_9000-1.2.5/SqltDAO/main.py
+-rw-rw-rw-   0        0        0      506 2024-05-27 11:08:13.000000 pydao_9000-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 12:37:46.326426 pydao_9000-1.2.5/setup.cfg
```

### Comparing `PyDAO_9000-1.2.4/LICENSE` & `pydao_9000-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/PKG-INFO` & `pydao_9000-1.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDAO_9000
-Version: 1.2.4
+Version: 1.2.5
 Summary: 'All-In-One File' SQL Code Generator
 Author-email: Randall Nagy <r.a.nagy@gmail.com>
 Project-URL: Homepage, https://github.com/soft9000/PyDAO
 Project-URL: Bug Tracker, https://github.com/soft9000/PyDAO/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,16 +27,14 @@
 
 (3) Creating database code from __PyDAO 9000__ projects, and 
 
 (4) Directly creating code from the __PyDAO 9000__ API. Result output-locations can also be specified.
 
 The generated code can be used to create / drop database schema (DDL,) as well as to import & work with (C.R.U.D & query) your designed / detected / updated projects.
 
-Project Video: https://youtu.be/azCokv4iI8k
-
 All four (4) workflows are supported - feel free to give each a try!
 
 
 The GUI
 -------
 ![PyDAO GUI](PyDAO_GUI.png)
```

### Comparing `PyDAO_9000-1.2.4/PyDAO_9000.egg-info/PKG-INFO` & `pydao_9000-1.2.5/PyDAO_9000.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: PyDAO-9000
-Version: 1.2.4
+Name: PyDAO_9000
+Version: 1.2.5
 Summary: 'All-In-One File' SQL Code Generator
 Author-email: Randall Nagy <r.a.nagy@gmail.com>
 Project-URL: Homepage, https://github.com/soft9000/PyDAO
 Project-URL: Bug Tracker, https://github.com/soft9000/PyDAO/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,16 +27,14 @@
 
 (3) Creating database code from __PyDAO 9000__ projects, and 
 
 (4) Directly creating code from the __PyDAO 9000__ API. Result output-locations can also be specified.
 
 The generated code can be used to create / drop database schema (DDL,) as well as to import & work with (C.R.U.D & query) your designed / detected / updated projects.
 
-Project Video: https://youtu.be/azCokv4iI8k
-
 All four (4) workflows are supported - feel free to give each a try!
 
 
 The GUI
 -------
 ![PyDAO GUI](PyDAO_GUI.png)
```

### Comparing `PyDAO_9000-1.2.4/PyDAO_9000.egg-info/SOURCES.txt` & `pydao_9000-1.2.5/PyDAO_9000.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/README.md` & `pydao_9000-1.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 
 (3) Creating database code from __PyDAO 9000__ projects, and 
 
 (4) Directly creating code from the __PyDAO 9000__ API. Result output-locations can also be specified.
 
 The generated code can be used to create / drop database schema (DDL,) as well as to import & work with (C.R.U.D & query) your designed / detected / updated projects.
 
-Project Video: https://youtu.be/azCokv4iI8k
-
 All four (4) workflows are supported - feel free to give each a try!
 
 
 The GUI
 -------
 ![PyDAO GUI](PyDAO_GUI.png)
```

### Comparing `PyDAO_9000-1.2.4/SqltDAO/CodeGen01/CodeGen.py` & `pydao_9000-1.2.5/SqltDAO/CodeGen01/CodeGen.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/CodeGen01/CodeLevel.py` & `pydao_9000-1.2.5/SqltDAO/CodeGen01/CodeLevel.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/CodeGen01/Normalizers.py` & `pydao_9000-1.2.5/SqltDAO/CodeGen01/Normalizers.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/CodeGen01/OrderClass.py` & `pydao_9000-1.2.5/SqltDAO/CodeGen01/OrderClass.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/CodeGen01/SqlSyntax.py` & `pydao_9000-1.2.5/SqltDAO/CodeGen01/SqlSyntax.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Author: Soft9000.com
 # 2018/03/08: Class Created
 # 2021/02/18: Adding DAO / Dict I/O usages.
+# 2024/05/24: Pythonic.
 
 import os
 import sys
 sys.path.insert(1, os.path.join(sys.path[0], '../..'))
 
 from collections import OrderedDict
 from SqltDAO.CodeGen01.OrderClass import OrderClass
@@ -180,14 +181,37 @@
         self.level.dec()
         result += self.level.print("return None")
         result += self.level.print("")
         self.level.dec()
         self.level.dec()
 
         self.level.push()
+        result += self.level.print("''' New: Explicitly convert the SQLRow to a list. '''")
+        result += self.level.print("def select_list(self, sql_select):")
+        self.level.inc()
+        result += self.level.print("if self.bOpen:")
+        self.level.inc();
+        result += self.level.print('self.curs.execute(sql_select)')
+        result += self.level.print("zlist = self.curs.fetchall()")
+        result += self.level.print("for ref in zlist:")
+        self.level.inc();
+        result += self.level.print("try:")
+        self.level.inc();
+        result += self.level.print("yield [*ref]")
+        self.level.dec()
+        result += self.level.print("except:")
+        self.level.inc();
+        result += self.level.print("pass")
+        self.level.dec()
+        self.level.dec()
+        result += self.level.print("return None")
+        result += self.level.print("")
+        self.level.pop()
+
+        self.level.push()
         result += self.level.print("@staticmethod")
         if self.order.encoding:
             encoding = "'" + self.order.encoding + "'"
         else:
             encoding = str(self.order.encoding)
         result += self.level.print("def Import(dao, encoding=" + encoding
                                    + ", text_file='" + text_file
@@ -262,25 +286,26 @@
         self.level.dec()
         self.level.dec()
         result += self.level.print('return True')
         return result
 
     def _inject_import(self):
         result = ''
+        result += self.level.print("# Table creation & open DAO.")
         result += self.level.print("try:")
         self.level.inc()
         result += self.level.print('# dao.open()')
         result += self.level.print("with open(text_file, encoding=encoding) as fh:")
         self.level.inc()
         result += self.level.print("line = fh.readline().strip()")
         result += self.level.print("if hasHeader is True:")
         self.level.inc()
         result += self.level.print("line = fh.readline().strip()")
         self.level.dec()
-        result += self.level.print("while len(line) != 0:")
+        result += self.level.print("while line:")
         self.level.inc()
         result += self.level.print("if dao.insert(line.split(sep)) is False:")
         self.level.inc()
         result += self.level.print("return False")
         self.level.dec()
         result += self.level.print("line = fh.readline().strip()")
         self.level.dec()
```

### Comparing `PyDAO_9000-1.2.4/SqltDAO/CodeGen01/TextDataDetector.py` & `pydao_9000-1.2.5/SqltDAO/CodeGen01/TextDataDetector.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/CrudMeister.py` & `pydao_9000-1.2.5/SqltDAO/CrudMeister.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/DaoTest01/GenNasdaq.py` & `pydao_9000-1.2.5/SqltDAO/DaoTest01/GenNasdaq.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/DaoTest01/Income.py` & `pydao_9000-1.2.5/SqltDAO/DaoTest01/Income.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/DaoTest01/NasdaqDAO.py` & `pydao_9000-1.2.5/SqltDAO/DaoTest01/NasdaqDAO.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/DaoTest01/foo.py` & `pydao_9000-1.2.5/SqltDAO/DaoTest01/foo.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/DaoTest01/tc001_driver.py` & `pydao_9000-1.2.5/SqltDAO/DaoTest01/tc001_driver.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/DaoTest01/tc001_gen.py` & `pydao_9000-1.2.5/SqltDAO/DaoTest01/tc001_gen.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/Demo123.py` & `pydao_9000-1.2.5/SqltDAO/Demo123.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,21 +73,21 @@
 # STEP 3: Enjoy!
 # ######
 
 from SqltDAO.CodeGen01.OrderClass import OrderClass
 from SqltDAO.CodeGen01.SqlSyntax import SqliteCrud
 
 
-for line in tables:
-    zname = line["ObjectName"]
+for table in tables:
+    zname = table["ObjectName"]
     print("Table:", zname)
     order = OrderClass(
         db_name=output_file + ".sqlt3",
         class_name=zname,
         table_name=zname,
         file_name="./" + zname + ".py")
-    zfields = line["Fields"]
+    zfields = table["Fields"]
     sql = SqliteCrud(order, zfields)
     data_file = str(zname + '.csv')
     result = sql.code_class_template(data_file)
     with open(output_file + ".py", 'a') as fh:
         print(result, file=fh)
```

### Comparing `PyDAO_9000-1.2.4/SqltDAO/Gui/Data2Code.py` & `pydao_9000-1.2.5/SqltDAO/Gui/Data2Code.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/Gui/DataAI.py` & `pydao_9000-1.2.5/SqltDAO/Gui/DataAI.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/Gui/DataFrameOne.py` & `pydao_9000-1.2.5/SqltDAO/Gui/DataFrameOne.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/Gui/DataPreferences.py` & `pydao_9000-1.2.5/SqltDAO/Gui/DataPreferences.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/Gui/StandardEntry.py` & `pydao_9000-1.2.5/SqltDAO/Gui/StandardEntry.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/Gui/TableDef.py` & `pydao_9000-1.2.5/SqltDAO/Gui/TableDef.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/Ledger.py` & `pydao_9000-1.2.5/SqltDAO/Ledger.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/SchemaDef/DataDetective.py` & `pydao_9000-1.2.5/SqltDAO/SchemaDef/DataDetective.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/SchemaDef/Factory.py` & `pydao_9000-1.2.5/SqltDAO/SchemaDef/Factory.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/SchemaDef/OrderDef.py` & `pydao_9000-1.2.5/SqltDAO/SchemaDef/OrderDef.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/SchemaDef/Table.py` & `pydao_9000-1.2.5/SqltDAO/SchemaDef/Table.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/UpdateTestCase.py` & `pydao_9000-1.2.5/SqltDAO/UpdateTestCase.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2.4/SqltDAO/main.py` & `pydao_9000-1.2.5/SqltDAO/main.py`

 * *Files identical despite different names*

