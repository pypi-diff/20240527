# Comparing `tmp/pysql_manager-0.0.1.2.tar.gz` & `tmp/pysql_manager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysql_manager-0.0.1.2.tar", last modified: Wed Feb 15 19:18:35 2023, max compression
+gzip compressed data, was "pysql_manager-0.0.3.tar", last modified: Mon May 27 17:39:48 2024, max compression
```

## Comparing `pysql_manager-0.0.1.2.tar` & `pysql_manager-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 badhusha   (502) staff       (20)        0 2023-02-15 19:18:35.745882 pysql_manager-0.0.1.2/
--rw-r--r--   0 badhusha   (502) staff       (20)     1488 2023-01-25 19:51:12.000000 pysql_manager-0.0.1.2/LICENCE.txt
--rw-r--r--   0 badhusha   (502) staff       (20)     5983 2023-02-15 19:18:35.745504 pysql_manager-0.0.1.2/PKG-INFO
--rw-r--r--   0 badhusha   (502) staff       (20)     5402 2023-02-15 16:14:55.000000 pysql_manager-0.0.1.2/README.md
-drwxr-xr-x   0 badhusha   (502) staff       (20)        0 2023-02-15 19:18:35.741196 pysql_manager-0.0.1.2/pysql_manager/
--rw-r--r--   0 badhusha   (502) staff       (20)     2234 2023-01-23 09:00:44.000000 pysql_manager-0.0.1.2/pysql_manager/__init__.py
--rw-r--r--   0 badhusha   (502) staff       (20)     4345 2023-02-15 17:14:44.000000 pysql_manager-0.0.1.2/pysql_manager/bases.py
--rw-r--r--   0 badhusha   (502) staff       (20)      636 2023-01-21 16:26:41.000000 pysql_manager-0.0.1.2/pysql_manager/errors.py
--rw-r--r--   0 badhusha   (502) staff       (20)      502 2023-02-15 16:57:24.000000 pysql_manager-0.0.1.2/pysql_manager/functions.py
--rw-r--r--   0 badhusha   (502) staff       (20)      359 2023-01-25 10:26:50.000000 pysql_manager-0.0.1.2/pysql_manager/types.py
-drwxr-xr-x   0 badhusha   (502) staff       (20)        0 2023-02-15 19:18:35.743834 pysql_manager-0.0.1.2/pysql_manager.egg-info/
--rw-r--r--   0 badhusha   (502) staff       (20)     5983 2023-02-15 19:18:35.000000 pysql_manager-0.0.1.2/pysql_manager.egg-info/PKG-INFO
--rw-r--r--   0 badhusha   (502) staff       (20)      356 2023-02-15 19:18:35.000000 pysql_manager-0.0.1.2/pysql_manager.egg-info/SOURCES.txt
--rw-r--r--   0 badhusha   (502) staff       (20)        1 2023-02-15 19:18:35.000000 pysql_manager-0.0.1.2/pysql_manager.egg-info/dependency_links.txt
--rw-r--r--   0 badhusha   (502) staff       (20)       36 2023-02-15 19:18:35.000000 pysql_manager-0.0.1.2/pysql_manager.egg-info/requires.txt
--rw-r--r--   0 badhusha   (502) staff       (20)       14 2023-02-15 19:18:35.000000 pysql_manager-0.0.1.2/pysql_manager.egg-info/top_level.txt
--rw-r--r--   0 badhusha   (502) staff       (20)       38 2023-02-15 19:18:35.746054 pysql_manager-0.0.1.2/setup.cfg
--rw-r--r--   0 badhusha   (502) staff       (20)      955 2023-02-15 17:14:55.000000 pysql_manager-0.0.1.2/setup.py
-drwxr-xr-x   0 badhusha   (502) staff       (20)        0 2023-02-15 19:18:35.744485 pysql_manager-0.0.1.2/test/
--rw-r--r--   0 badhusha   (502) staff       (20)      533 2023-02-15 17:14:44.000000 pysql_manager-0.0.1.2/test/test_case1.py
+drwxr-xr-x   0 badhusha   (501) staff       (20)        0 2024-05-27 17:39:48.466141 pysql_manager-0.0.3/
+-rw-r--r--   0 badhusha   (501) staff       (20)     1488 2024-05-18 22:18:57.000000 pysql_manager-0.0.3/LICENCE.txt
+-rw-r--r--   0 badhusha   (501) staff       (20)     5800 2024-05-27 17:39:48.465532 pysql_manager-0.0.3/PKG-INFO
+-rw-r--r--   0 badhusha   (501) staff       (20)     5160 2024-05-27 16:49:50.000000 pysql_manager-0.0.3/README.md
+drwxr-xr-x   0 badhusha   (501) staff       (20)        0 2024-05-27 17:39:48.457111 pysql_manager-0.0.3/pysql_manager/
+-rw-r--r--   0 badhusha   (501) staff       (20)      141 2024-05-19 06:13:19.000000 pysql_manager-0.0.3/pysql_manager/__init__.py
+drwxr-xr-x   0 badhusha   (501) staff       (20)        0 2024-05-27 17:39:48.463788 pysql_manager-0.0.3/pysql_manager/core/
+-rw-r--r--   0 badhusha   (501) staff       (20)        0 2024-05-19 05:17:45.000000 pysql_manager-0.0.3/pysql_manager/core/__init__.py
+-rw-r--r--   0 badhusha   (501) staff       (20)       43 2024-05-19 06:11:00.000000 pysql_manager-0.0.3/pysql_manager/core/api.py
+-rw-r--r--   0 badhusha   (501) staff       (20)     5040 2024-05-19 06:21:49.000000 pysql_manager-0.0.3/pysql_manager/core/bases.py
+-rw-r--r--   0 badhusha   (501) staff       (20)     2378 2024-05-27 16:34:53.000000 pysql_manager-0.0.3/pysql_manager/core/pysql.py
+-rw-r--r--   0 badhusha   (501) staff       (20)      315 2024-05-19 05:56:01.000000 pysql_manager-0.0.3/pysql_manager/core/wrapper.py
+drwxr-xr-x   0 badhusha   (501) staff       (20)        0 2024-05-27 17:39:48.464297 pysql_manager-0.0.3/pysql_manager/errors/
+-rw-r--r--   0 badhusha   (501) staff       (20)      690 2024-05-19 05:49:42.000000 pysql_manager-0.0.3/pysql_manager/errors/__init__.py
+-rw-r--r--   0 badhusha   (501) staff       (20)      570 2024-05-18 22:18:57.000000 pysql_manager-0.0.3/pysql_manager/functions.py
+-rw-r--r--   0 badhusha   (501) staff       (20)      762 2024-05-27 16:39:51.000000 pysql_manager-0.0.3/pysql_manager/types.py
+drwxr-xr-x   0 badhusha   (501) staff       (20)        0 2024-05-27 17:39:48.460759 pysql_manager-0.0.3/pysql_manager.egg-info/
+-rw-r--r--   0 badhusha   (501) staff       (20)     5800 2024-05-27 17:39:48.000000 pysql_manager-0.0.3/pysql_manager.egg-info/PKG-INFO
+-rw-r--r--   0 badhusha   (501) staff       (20)      480 2024-05-27 17:39:48.000000 pysql_manager-0.0.3/pysql_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 badhusha   (501) staff       (20)        1 2024-05-27 17:39:48.000000 pysql_manager-0.0.3/pysql_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 badhusha   (501) staff       (20)       36 2024-05-27 17:39:48.000000 pysql_manager-0.0.3/pysql_manager.egg-info/requires.txt
+-rw-r--r--   0 badhusha   (501) staff       (20)       14 2024-05-27 17:39:48.000000 pysql_manager-0.0.3/pysql_manager.egg-info/top_level.txt
+-rw-r--r--   0 badhusha   (501) staff       (20)       38 2024-05-27 17:39:48.466362 pysql_manager-0.0.3/setup.cfg
+-rw-r--r--   0 badhusha   (501) staff       (20)      981 2024-05-27 17:39:37.000000 pysql_manager-0.0.3/setup.py
+drwxr-xr-x   0 badhusha   (501) staff       (20)        0 2024-05-27 17:39:48.464799 pysql_manager-0.0.3/test/
+-rw-r--r--   0 badhusha   (501) staff       (20)      660 2024-05-27 16:51:03.000000 pysql_manager-0.0.3/test/test1.py
```

### Comparing `pysql_manager-0.0.1.2/LICENCE.txt` & `pysql_manager-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pysql_manager-0.0.1.2/PKG-INFO` & `pysql_manager-0.0.3/pysql_manager.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
-Name: pysql_manager
-Version: 0.0.1.2
+Name: pysql-manager
+Version: 0.0.3
 Summary: A python package for managing Mysql
 Home-page: https://github.com/Badhsuha/PysqlManager
 Author: Badhusha K Muhammed
 Author-email: badhushamuhammed09@gmail.com
 License: BSD 3-Clause License
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
+Requires-Dist: mysql-connector-python
+Requires-Dist: pandas
+Requires-Dist: numpy
 
 # PysqlManager
 A python package to manage sql
 
 # GETTING STARTED !
 
 Creating a PySql object is the first step. All function are defined in PySql Class (Which is base class for PysqlManager Module)
@@ -25,44 +27,50 @@
 For creating PySql object we need a meta_class / reference class (meta_class is nothing but a class structure for SQL table)
 
 User(id varchar(25), name varchar(20), Age INT)
 
 For above table , the reference class will be
 
 ```Python
-from pysql_manager.types import Column, IntegerType, StringType
-    
+from pysql_manager.types import IntegerType, StringType
+
+
 class User:
-    id = Column(col_type=IntegerType())
-    name = Column(col_type=StringType(25))
-    age = Column(col_type=IntegerType())
+    id = IntegerType()
+    name = StringType(length=25)
+    age = IntegerType()
     __table__ = "User"
 
+
 # Now we can use this meta_class to create actual PySql objcet 
 
 from pysql_manager import PySql
+
 users = PySql("localhost", "root", "passowrd", "DB", User)
-users.fetch_all.show() #sample method for fetching and showing all the data from table User
+users.fetch_all.show()  # sample method for fetching and showing all the data from table User
 ```  
 
 
 ## FETCH ALL DATA FROM SQL TABLE
+
 ```Python
-from pysql_manager.types import Column, IntegerType, StringType
-    
+from pysql_manager.types import IntegerType, StringType
+
+
 class User:
-    id = Column(col_type=IntegerType())
-    name = Column(col_type=StringType(25))
-    age = Column(col_type=IntegerType())
+    id = IntegerType()
+    name = StringType(25)
+    age = IntegerType()
     __table__ = "User"
-    
+
+
 from pysql_manager import PySql
 
 users = PySql("localhost", "root", "passowrd", "DB", User)
-users.fetch_all # Return PySqlConnection
+users.fetch_all  # Return PySqlConnection
 ```
 
 fetch_all method will return a PySqlCollection object , which contain rich functionalities.
 
 <br />
 
 ### .show() - To show data in table form
@@ -168,43 +176,47 @@
 ### .delete() - To delete filtered data
 ```Python
 users.filter("age > 10").delete() # Return None
 ```
 
 ## INSERT DATA TO SQL TABLE
 Insert is done using .insert() method, The data should be List of python dictionaries.
+
 ```Python
-from pysql_manager.types import Column, IntegerType, StringType
-    
+from pysql_manager.types import IntegerType, StringType
+
+
 class User:
-    id = Column(col_type=IntegerType())
-    name = Column(col_type=StringType(25))
-    age = Column(col_type=IntegerType())
+    id = IntegerType()
+    name = StringType(25)
+    age = IntegerType()
     __table__ = "User"
-    
+
+
 from pysql_manager import PySql
 
 users = PySql("localhost", "root", "passowrd", "DB", User)
-sql_data = [{"id": 1, "name": "user1", "age": 22}, {"id": 2, "name": "user2", "age": 12}] 
-users.insert(sql_data) # Return PySql self
+sql_data = [{"id": 1, "name": "user1", "age": 22}, {"id": 2, "name": "user2", "age": 12}]
+users.insert(sql_data)  # Return PySql self
 ```
 
 If there is duplicate entry for primary key (In this case `id` column, it will raise `PRIMARY KEY ERROR`). To avoid this and update on duplicate key you can use `update_on_duplicate` argument and pass list columns you need to update when there is a duplicate entry.
+
 ```Python
-from pysql_manager.types import Column, IntegerType, StringType
-    
+from pysql_manager.types import IntegerType, StringType
+
+
 class User:
-    id = Column(col_type=IntegerType())
-    name = Column(col_type=StringType(25))
-    age = Column(col_type=IntegerType())
+    id = IntegerType()
+    name = StringType(25)
+    age = IntegerType()
     __table__ = "User"
-    
+
+
 from pysql_manager import PySql
 
 users = PySql("localhost", "root", "passowrd", "DB", User)
-sql_data = [{"id": 1, "name": "user1", "age": 22}, {"id": 2, "name": "user2", "age": 12}] 
-users.insert(sql_data, update_on_duplicate=["age"]) # Return PySql self
+sql_data = [{"id": 1, "name": "user1", "age": 22}, {"id": 2, "name": "user2", "age": 12}]
+users.insert(sql_data, update_on_duplicate=["age"])  # Return PySql self
 ```
 
 
-
-
```

### Comparing `pysql_manager-0.0.1.2/README.md` & `pysql_manager-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,44 +8,50 @@
 For creating PySql object we need a meta_class / reference class (meta_class is nothing but a class structure for SQL table)
 
 User(id varchar(25), name varchar(20), Age INT)
 
 For above table , the reference class will be
 
 ```Python
-from pysql_manager.types import Column, IntegerType, StringType
-    
+from pysql_manager.types import IntegerType, StringType
+
+
 class User:
-    id = Column(col_type=IntegerType())
-    name = Column(col_type=StringType(25))
-    age = Column(col_type=IntegerType())
+    id = IntegerType()
+    name = StringType(length=25)
+    age = IntegerType()
     __table__ = "User"
 
+
 # Now we can use this meta_class to create actual PySql objcet 
 
 from pysql_manager import PySql
+
 users = PySql("localhost", "root", "passowrd", "DB", User)
-users.fetch_all.show() #sample method for fetching and showing all the data from table User
+users.fetch_all.show()  # sample method for fetching and showing all the data from table User
 ```  
 
 
 ## FETCH ALL DATA FROM SQL TABLE
+
 ```Python
-from pysql_manager.types import Column, IntegerType, StringType
-    
+from pysql_manager.types import IntegerType, StringType
+
+
 class User:
-    id = Column(col_type=IntegerType())
-    name = Column(col_type=StringType(25))
-    age = Column(col_type=IntegerType())
+    id = IntegerType()
+    name = StringType(25)
+    age = IntegerType()
     __table__ = "User"
-    
+
+
 from pysql_manager import PySql
 
 users = PySql("localhost", "root", "passowrd", "DB", User)
-users.fetch_all # Return PySqlConnection
+users.fetch_all  # Return PySqlConnection
 ```
 
 fetch_all method will return a PySqlCollection object , which contain rich functionalities.
 
 <br />
 
 ### .show() - To show data in table form
@@ -151,41 +157,47 @@
 ### .delete() - To delete filtered data
 ```Python
 users.filter("age > 10").delete() # Return None
 ```
 
 ## INSERT DATA TO SQL TABLE
 Insert is done using .insert() method, The data should be List of python dictionaries.
+
 ```Python
-from pysql_manager.types import Column, IntegerType, StringType
-    
+from pysql_manager.types import IntegerType, StringType
+
+
 class User:
-    id = Column(col_type=IntegerType())
-    name = Column(col_type=StringType(25))
-    age = Column(col_type=IntegerType())
+    id = IntegerType()
+    name = StringType(25)
+    age = IntegerType()
     __table__ = "User"
-    
+
+
 from pysql_manager import PySql
 
 users = PySql("localhost", "root", "passowrd", "DB", User)
-sql_data = [{"id": 1, "name": "user1", "age": 22}, {"id": 2, "name": "user2", "age": 12}] 
-users.insert(sql_data) # Return PySql self
+sql_data = [{"id": 1, "name": "user1", "age": 22}, {"id": 2, "name": "user2", "age": 12}]
+users.insert(sql_data)  # Return PySql self
 ```
 
 If there is duplicate entry for primary key (In this case `id` column, it will raise `PRIMARY KEY ERROR`). To avoid this and update on duplicate key you can use `update_on_duplicate` argument and pass list columns you need to update when there is a duplicate entry.
+
 ```Python
-from pysql_manager.types import Column, IntegerType, StringType
-    
+from pysql_manager.types import IntegerType, StringType
+
+
 class User:
-    id = Column(col_type=IntegerType())
-    name = Column(col_type=StringType(25))
-    age = Column(col_type=IntegerType())
+    id = IntegerType()
+    name = StringType(25)
+    age = IntegerType()
     __table__ = "User"
-    
+
+
 from pysql_manager import PySql
 
 users = PySql("localhost", "root", "passowrd", "DB", User)
-sql_data = [{"id": 1, "name": "user1", "age": 22}, {"id": 2, "name": "user2", "age": 12}] 
-users.insert(sql_data, update_on_duplicate=["age"]) # Return PySql self
+sql_data = [{"id": 1, "name": "user1", "age": 22}, {"id": 2, "name": "user2", "age": 12}]
+users.insert(sql_data, update_on_duplicate=["age"])  # Return PySql self
 ```
```

### Comparing `pysql_manager-0.0.1.2/pysql_manager/__init__.py` & `pysql_manager-0.0.3/pysql_manager/core/pysql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+import sys
 from typing import List
-
 import mysql.connector
 from mysql.connector.errors import ProgrammingError
-from .bases import PySqlCollection, PySqlFilterObj
-from .types import Column
-from .errors import ColumnNotFountInClass, TableNotFoundInClass
+from pysql_manager.core.bases import PySqlFilterObj, PySqlCollection
+from pysql_manager.types import _Column
+from pysql_manager.errors import TableNotFoundInClass
 
-__version__ = "0.1.0"
+__version__ = "0.0.1"
 __author__ = 'Badhusha K Muhammed'
 
 """
 Main Class for bkm-pysql_manager, Used to connect to mysql, Getting data and create PySqpDataCollection
 """
 
 
@@ -19,15 +19,16 @@
         self.db = mysql.connector.connect(
             host=host,
             user=username,
             password=password,
             database=dbname
         )
         self._meta_class = meta_class
-        self.columns = list(filter(lambda x: isinstance(getattr(self._meta_class, x), Column), dir(meta_class)))
+        self.columns = list(filter(lambda x: isinstance(getattr(self._meta_class, x), _Column), dir(meta_class)))
+
         try:
             self.table = getattr(self._meta_class, "__table__")
         except AttributeError:
             raise TableNotFoundInClass(self._meta_class.__name__)
 
         self._cursor = self.db.cursor()
 
@@ -46,16 +47,19 @@
                               columns=self.columns,
                               table=self.table,
                               db=self.db
                               )
 
     def insert(self, ins_data: List[dict], update_on_duplicate=None):
         query = f"INSERT INTO {self.table}({','.join(self.columns)}) VALUES "
-        gen = ["(" + ','.join([f"'{data.get(col)}'" for col in self.columns]) + ")" for data in ins_data]
+        gen = ["(" + ','.join([f"'{data.get(col) if data.get(col) else  getattr(self._meta_class, col).default}'" for col in self.columns]) + ")" for data in ins_data]
+
         ex_query = query + ",".join(gen)
+        print(ex_query)
+        # sys.exit(-1)
         if update_on_duplicate is not None:
             ex_query += "ON DUPLICATE KEY UPDATE " + ",".join([f"{col}=VALUES({col})" for col in update_on_duplicate])
 
         self._cursor.execute(ex_query)
 
         self.db.commit()
         return self
```

### Comparing `pysql_manager-0.0.1.2/pysql_manager/bases.py` & `pysql_manager-0.0.3/pysql_manager/core/bases.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,95 @@
-from csv import DictWriter
 from pandas import DataFrame
-from .errors import EmptyPysqlCollectionError, ColumnNotFountInClass
-from .functions import _ColumnFunc
-
-"""
-Dynamic Class Creation from given meta class base
-"""
-
-
-def create_mata(columns, data, meta_class):
-    return type(meta_class.__table__, (), {column: d for column, d in zip(columns, data)})
-
+from csv import DictWriter
+from typing import List, Callable
+from pysql_manager.errors import ColumnNotFountInClass
+from pysql_manager.functions import _ColumnFunc
+from pysql_manager.core.wrapper import check_data_availability
+from pysql_manager.types import StringType, IntegerType
 
 """
 A collection of meta class, for querying data
 """
 
 
 class PySqlCollection:
 
-    def __init__(self, mysql_data, column, meta_class):
-        self.__columns__ = column
+    def __init__(self, mysql_data, columns, meta_class):
+        self.__columns__ = columns
         self.__meta_class = meta_class
-        self.__data__ = [create_mata(column, data, meta_class) for data in mysql_data]
-
-    def check_data_availability(func):
-        def wrap(self, *args, **kwargs):
-            if self.count() != 0:
-                result = func(self, *args, **kwargs)
-                return result
-            else:
-                raise EmptyPysqlCollectionError()
-
-        return wrap
+        self.__data__ = _generate_data(mysql_data, meta_class, columns)
 
     @check_data_availability
     def first(self):
         return self.__data__[0]
 
     @check_data_availability
     def last(self):
         return self.__data__[-1]
 
-    def is_empty(self):
+    def is_empty(self) -> bool:
         return not bool(self.__data__)
 
-    def count(self):
+    def count(self) -> int:
         return len(self.__data__)
 
     @check_data_availability
-    def to_df(self):
+    def to_df(self) -> DataFrame:
         return DataFrame.from_dict(self.to_list_dict())
 
-    def to_list_dict(self):
-        obj_dicts = map(lambda obj: obj.__dict__, self.__data__)
-        return list(map(lambda obj: {key: obj[key] for key in obj if key in self.__columns__}, obj_dicts))
+    def to_list_dict(self) -> List[dict]:
+        return list(map(lambda data: {col: getattr(data, col).get_value() for col in self.__columns__}, self.__data__))
 
     @check_data_availability
     def save_as_csv(self, path, delimiter=","):
 
         data = self.to_list_dict()
         with open(path, "w") as file:
             csv_writer = DictWriter(file, data[0].keys(), delimiter=delimiter)
             csv_writer.writeheader()
             csv_writer.writerows(data)
 
     def show(self):
-        str_po = "{:<10}" * len(self.__columns__)
+        str_po = "".join(["{:<" + f"{len(col) + 5}" + "}" for col in self.__columns__])
         print(str_po.format(*[col for col in self.__columns__]))
         for data in self.__data__:
-            print(str_po.format(*[getattr(data, col) for col in self.__columns__]))
+            print(str_po.format(*[getattr(data, col).get_value() for col in self.__columns__]))
 
     @check_data_availability
     def select(self, columns=None):
         if not isinstance(columns, list):
             print("Pleas pass column / Column as List")
             return None
 
-        mysql_data = list(map(lambda x: (getattr(x, col) for col in columns), self.__data__))
+        mysql_data = list(map(lambda x: [getattr(x, col).get_value() for col in columns], self.__data__))
 
         if len(columns) == 1:
             return PysqlCollectionSingle(mysql_data, columns, self.__meta_class)
 
         return PySqlCollection(mysql_data, columns, self.__meta_class)
 
     @check_data_availability
     def sum(self, col: _ColumnFunc):
         return {col.alias_name("sum"): sum([getattr(row, col.column_name) for row in self.__data__])}
 
     def unique(self, col: _ColumnFunc):
-        return {col.alias_name("unique"): list(set([getattr(row, col.column_name) for row in self.__data__]))}
+        return {col.alias_name("unique"): list(set([getattr(row, col.column_name).get_value() for row in self.__data__]))}
+
+    def filter(self, lambda_function: Callable):
+
+        mysql_data = list(map(lambda x: (getattr(x, col).get_value() for col in self.__columns__),
+                              list(filter(lambda_function, self.__data__))))
+
+        return PySqlCollection(mysql_data, self.__columns__, self.__meta_class)
 
 
 class PysqlCollectionSingle(PySqlCollection):
     def to_list(self):
-        obj_dicts = map(lambda obj: obj.__dict__, self.__data__)
-        return {self.__columns__[0]: list(map(lambda obj: obj[self.__columns__[0]], obj_dicts))}
+        return {
+            self.__columns__[0]: list(map(lambda rec: getattr(rec, self.__columns__[0]).get_value(), self.__data__))}
 
 
 class PySqlFilterObj:
     def __init__(self, filter_query, cursor, meta_class, columns, table, db):
         self.columns = columns
         self._filter_query = filter_query
         self._cursor = cursor
@@ -111,20 +101,49 @@
         if not all([key in self.columns for key in kwargs.keys()]):
             raise (ColumnNotFountInClass(kwargs.keys(), self.table))
         else:
             set_array = [f"{key}='{kwargs[key]}'" for key in kwargs.keys()]
             query = f"UPDATE {self.table} SET " + f"{','.join(set_array)}" + f" WHERE {self._filter_query}"
             self._cursor.execute(query)
             self._db.commit()
-            # print(query)
-            print("Update Done")
 
     def delete(self):
         query = f"DELETE FROM {self.table} WHERE " + self._filter_query
         self._cursor.execute(query)
         self._db.commit()
-        print("Deletion Done")
 
     @property
     def fetch_filtered(self):
         self._cursor.execute(f"SELECT {','.join(self.columns)} from {self.table} WHERE {self._filter_query}")
-        return PySqlCollection(self._cursor.fetchall(), self.columns, self._meta_class)
+        return PySqlCollection(self._cursor.fetchall(), self.columns, self._meta_class)
+
+
+def _get_class_of(meta_class, col):
+    return eval(getattr(meta_class, col).__class__.__name__)
+
+
+def _get_col_feature(meta_class, col, feature):
+    return getattr(getattr(meta_class, col), feature)
+
+
+"""
+Dynamic Class Creation from given meta class base
+"""
+
+
+def _generate_data(mysql_data, meta_class, columns) -> List:
+    collection_list = []
+
+    for m_data in mysql_data:
+        meta_cls = _create_mata(columns, m_data, meta_class)
+        collection_list.append(meta_cls)
+
+    return collection_list
+
+
+def _create_mata(columns, data, meta_class):
+
+    return type(meta_class.__table__, (),
+
+                {column: _get_class_of(meta_class, column)(length=_get_col_feature(meta_class, column, "length")).set_value(d)
+
+                 for column, d in zip(columns, data)})
```

### Comparing `pysql_manager-0.0.1.2/pysql_manager/errors.py` & `pysql_manager-0.0.3/pysql_manager/errors/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 class ColumnNotFountInClass(Exception):
-    def __init__(self, columns, table, message="Column {0} not found in master class for table "):
-        self.salary = columns
+    def __init__(self, columns, table, message="Column `{0}` not found in master class for table "):
+        self.columns = columns
         self.table = table
         self.message = message
-        super().__init__(self.message.format(list(columns)) + self.table)
+        super().__init__(self.message.format(columns if isinstance(columns, str) else ",".join(list(columns))) + self.table)
 
 
 class TableNotFoundInClass(Exception):
     def __init__(self,  meta_class_name):
         self.meta_class_name = meta_class_name
         super().__init__(f"Table not defined in Class {self.meta_class_name}")
```

### Comparing `pysql_manager-0.0.1.2/pysql_manager.egg-info/PKG-INFO` & `pysql_manager-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
-Name: pysql-manager
-Version: 0.0.1.2
+Name: pysql_manager
+Version: 0.0.3
 Summary: A python package for managing Mysql
 Home-page: https://github.com/Badhsuha/PysqlManager
 Author: Badhusha K Muhammed
 Author-email: badhushamuhammed09@gmail.com
 License: BSD 3-Clause License
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
+Requires-Dist: mysql-connector-python
+Requires-Dist: pandas
+Requires-Dist: numpy
 
 # PysqlManager
 A python package to manage sql
 
 # GETTING STARTED !
 
 Creating a PySql object is the first step. All function are defined in PySql Class (Which is base class for PysqlManager Module)
@@ -25,44 +27,50 @@
 For creating PySql object we need a meta_class / reference class (meta_class is nothing but a class structure for SQL table)
 
 User(id varchar(25), name varchar(20), Age INT)
 
 For above table , the reference class will be
 
 ```Python
-from pysql_manager.types import Column, IntegerType, StringType
-    
+from pysql_manager.types import IntegerType, StringType
+
+
 class User:
-    id = Column(col_type=IntegerType())
-    name = Column(col_type=StringType(25))
-    age = Column(col_type=IntegerType())
+    id = IntegerType()
+    name = StringType(length=25)
+    age = IntegerType()
     __table__ = "User"
 
+
 # Now we can use this meta_class to create actual PySql objcet 
 
 from pysql_manager import PySql
+
 users = PySql("localhost", "root", "passowrd", "DB", User)
-users.fetch_all.show() #sample method for fetching and showing all the data from table User
+users.fetch_all.show()  # sample method for fetching and showing all the data from table User
 ```  
 
 
 ## FETCH ALL DATA FROM SQL TABLE
+
 ```Python
-from pysql_manager.types import Column, IntegerType, StringType
-    
+from pysql_manager.types import IntegerType, StringType
+
+
 class User:
-    id = Column(col_type=IntegerType())
-    name = Column(col_type=StringType(25))
-    age = Column(col_type=IntegerType())
+    id = IntegerType()
+    name = StringType(25)
+    age = IntegerType()
     __table__ = "User"
-    
+
+
 from pysql_manager import PySql
 
 users = PySql("localhost", "root", "passowrd", "DB", User)
-users.fetch_all # Return PySqlConnection
+users.fetch_all  # Return PySqlConnection
 ```
 
 fetch_all method will return a PySqlCollection object , which contain rich functionalities.
 
 <br />
 
 ### .show() - To show data in table form
@@ -168,43 +176,47 @@
 ### .delete() - To delete filtered data
 ```Python
 users.filter("age > 10").delete() # Return None
 ```
 
 ## INSERT DATA TO SQL TABLE
 Insert is done using .insert() method, The data should be List of python dictionaries.
+
 ```Python
-from pysql_manager.types import Column, IntegerType, StringType
-    
+from pysql_manager.types import IntegerType, StringType
+
+
 class User:
-    id = Column(col_type=IntegerType())
-    name = Column(col_type=StringType(25))
-    age = Column(col_type=IntegerType())
+    id = IntegerType()
+    name = StringType(25)
+    age = IntegerType()
     __table__ = "User"
-    
+
+
 from pysql_manager import PySql
 
 users = PySql("localhost", "root", "passowrd", "DB", User)
-sql_data = [{"id": 1, "name": "user1", "age": 22}, {"id": 2, "name": "user2", "age": 12}] 
-users.insert(sql_data) # Return PySql self
+sql_data = [{"id": 1, "name": "user1", "age": 22}, {"id": 2, "name": "user2", "age": 12}]
+users.insert(sql_data)  # Return PySql self
 ```
 
 If there is duplicate entry for primary key (In this case `id` column, it will raise `PRIMARY KEY ERROR`). To avoid this and update on duplicate key you can use `update_on_duplicate` argument and pass list columns you need to update when there is a duplicate entry.
+
 ```Python
-from pysql_manager.types import Column, IntegerType, StringType
-    
+from pysql_manager.types import IntegerType, StringType
+
+
 class User:
-    id = Column(col_type=IntegerType())
-    name = Column(col_type=StringType(25))
-    age = Column(col_type=IntegerType())
+    id = IntegerType()
+    name = StringType(25)
+    age = IntegerType()
     __table__ = "User"
-    
+
+
 from pysql_manager import PySql
 
 users = PySql("localhost", "root", "passowrd", "DB", User)
-sql_data = [{"id": 1, "name": "user1", "age": 22}, {"id": 2, "name": "user2", "age": 12}] 
-users.insert(sql_data, update_on_duplicate=["age"]) # Return PySql self
+sql_data = [{"id": 1, "name": "user1", "age": 22}, {"id": 2, "name": "user2", "age": 12}]
+users.insert(sql_data, update_on_duplicate=["age"])  # Return PySql self
 ```
 
 
-
-
```

### Comparing `pysql_manager-0.0.1.2/setup.py` & `pysql_manager-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_dir = Path(__file__).parent
 long_description = (this_dir / "README.md").read_text()
 
 setup(
     name='pysql_manager',
-    version='0.0.1.2',
+    version='0.0.3',
     description='A python package for managing Mysql',
     url='https://github.com/Badhsuha/PysqlManager',
     author='Badhusha K Muhammed',
     author_email='badhushamuhammed09@gmail.com',
     install_requires=['mysql-connector-python',
                       'pandas',
                       'numpy'
@@ -22,8 +22,9 @@
         'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
     ],
     license='BSD 3-Clause License',
+    python_reuires=">= 3.6"
 )
```

