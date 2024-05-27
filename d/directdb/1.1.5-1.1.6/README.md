# Comparing `tmp/directdb-1.1.5.tar.gz` & `tmp/directdb-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "directdb-1.1.5.tar", last modified: Sun Oct 22 02:56:31 2023, max compression
+gzip compressed data, was "directdb-1.1.6.tar", last modified: Mon May 27 16:02:41 2024, max compression
```

## Comparing `directdb-1.1.5.tar` & `directdb-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-10-22 02:56:31.980200 directdb-1.1.5/
--rw-rw-rw-   0        0        0    35182 2023-07-31 07:28:41.000000 directdb-1.1.5/LICENSE
--rw-rw-rw-   0        0        0     2604 2023-10-22 02:56:31.979200 directdb-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2023-08-05 11:08:18.000000 directdb-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-10-22 02:56:31.971200 directdb-1.1.5/directdb/
--rw-rw-rw-   0        0        0      605 2023-08-05 11:05:15.000000 directdb-1.1.5/directdb/__init__.py
--rw-rw-rw-   0        0        0     2412 2023-08-05 11:05:04.000000 directdb-1.1.5/directdb/exceptions.py
--rw-rw-rw-   0        0        0     5828 2023-08-05 11:04:58.000000 directdb-1.1.5/directdb/main.py
--rw-rw-rw-   0        0        0     6473 2023-10-22 02:55:32.000000 directdb-1.1.5/directdb/sqlite.py
-drwxrwxrwx   0        0        0        0 2023-10-22 02:56:31.978202 directdb-1.1.5/directdb.egg-info/
--rw-rw-rw-   0        0        0     2604 2023-10-22 02:56:31.000000 directdb-1.1.5/directdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-10-22 02:56:31.000000 directdb-1.1.5/directdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-22 02:56:31.000000 directdb-1.1.5/directdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-10-22 02:56:31.000000 directdb-1.1.5/directdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-10-22 02:56:31.000000 directdb-1.1.5/directdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-22 02:56:31.981201 directdb-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1157 2023-10-22 02:56:19.000000 directdb-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 16:02:41.535485 directdb-1.1.6/
+-rw-rw-rw-   0        0        0    35182 2023-07-31 07:28:41.000000 directdb-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2604 2024-05-27 16:02:41.533452 directdb-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2023-08-05 11:08:18.000000 directdb-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 16:02:41.524447 directdb-1.1.6/directdb/
+-rw-rw-rw-   0        0        0      605 2023-08-05 11:05:15.000000 directdb-1.1.6/directdb/__init__.py
+-rw-rw-rw-   0        0        0     2212 2024-05-27 15:56:00.000000 directdb-1.1.6/directdb/exceptions.py
+-rw-rw-rw-   0        0        0     5828 2023-08-05 11:04:58.000000 directdb-1.1.6/directdb/main.py
+-rw-rw-rw-   0        0        0     6473 2023-10-22 02:55:32.000000 directdb-1.1.6/directdb/sqlite.py
+drwxrwxrwx   0        0        0        0 2024-05-27 16:02:41.531453 directdb-1.1.6/directdb.egg-info/
+-rw-rw-rw-   0        0        0     2604 2024-05-27 16:02:41.000000 directdb-1.1.6/directdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-27 16:02:41.000000 directdb-1.1.6/directdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 16:02:41.000000 directdb-1.1.6/directdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-27 16:02:41.000000 directdb-1.1.6/directdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 16:02:41.000000 directdb-1.1.6/directdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 16:02:41.535485 directdb-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1157 2024-05-27 16:02:02.000000 directdb-1.1.6/setup.py
```

### Comparing `directdb-1.1.5/LICENSE` & `directdb-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `directdb-1.1.5/PKG-INFO` & `directdb-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directdb
-Version: 1.1.5
+Version: 1.1.6
 Summary: An async package that makes database handling extremely easy!
 Author: Cannonball Chris
 Author-email: cannonballchris8@gmail.com
 Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite,aiosqlite,discord.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `directdb-1.1.5/README.md` & `directdb-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `directdb-1.1.5/directdb/__init__.py` & `directdb-1.1.6/directdb/__init__.py`

 * *Files identical despite different names*

### Comparing `directdb-1.1.5/directdb/exceptions.py` & `directdb-1.1.6/directdb/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,68 +14,63 @@
 	Parameters
 	----------
 	message: str
 		The error message.
 	"""
 
 	def __init__(self, message):
-		with open("./log.txt", "a") as f:
-			f.write(f"- ERROR {datetime.datetime.now()} | {self.__class__.__name__} | {message} \n")
+		print(f"- ERROR {datetime.datetime.now()} | {self.__class__.__name__} | {message} \n")
 		super().__init__(message)
 
 class DatabaseTableException(Exception):
 	"""Class for exceptions when table creation fails.
 	
 	Parameters
 	----------
 	message: str
 		The error message.
 	"""
 
 	def __init__(self, message):
-		with open("./log.txt", "a") as f:
-			f.write(f"- ERROR {datetime.datetime.now()} | {self.__class__.__name__} | {message} \n")
+		print(f"- ERROR {datetime.datetime.now()} | {self.__class__.__name__} | {message} \n")
 		super().__init__(message)
 
 class DatabaseFetchException(Exception):
 	"""Class for exceptions when table fetching fails.
 	
 	Parameters
 	----------
 	message: str
 		The error message.
 	"""
 
 	def __init__(self, message):
-		with open("./log.txt", "a") as f:
-			f.write(f"- ERROR {datetime.datetime.now()} | {self.__class__.__name__} | {message} \n")
+		print(f"- ERROR {datetime.datetime.now()} | {self.__class__.__name__} | {message} \n")
 		super().__init__(message)
 
 class DatabaseUpdateException(Exception):
 	"""Class for exceptions when table fetching fails.
 	
 	Parameters
 	----------
 	message: str
 		The error message.
 	"""
 
 	def __init__(self, message):
-		with open("./log.txt", "a") as f:
-			f.write(f"- ERROR {datetime.datetime.now()} | {self.__class__.__name__} | {message} \n")
+		print(f"- ERROR {datetime.datetime.now()} | {self.__class__.__name__} | {message} \n")
 		super().__init__(message)
 
 class DatabaseDeleteException(Exception):
 	"""Class for exceptions when table fetching fails.
 	
 	Parameters
 	----------
 	message: str
 		The error message.
 	"""
 
 	def __init__(self, message):
 		self.message = message
-		with open("./log.txt", "a") as f:
-			f.write(f"- ERROR {datetime.datetime.now()} | {self.__class__.__name__} | {message} \n")
+		print(f"- ERROR {datetime.datetime.now()} | {self.__class__.__name__} | {message} \n")
 		super().__init__(message)
```

### Comparing `directdb-1.1.5/directdb/main.py` & `directdb-1.1.6/directdb/main.py`

 * *Files identical despite different names*

### Comparing `directdb-1.1.5/directdb/sqlite.py` & `directdb-1.1.6/directdb/sqlite.py`

 * *Files identical despite different names*

### Comparing `directdb-1.1.5/directdb.egg-info/PKG-INFO` & `directdb-1.1.6/directdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directdb
-Version: 1.1.5
+Version: 1.1.6
 Summary: An async package that makes database handling extremely easy!
 Author: Cannonball Chris
 Author-email: cannonballchris8@gmail.com
 Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite,aiosqlite,discord.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `directdb-1.1.5/setup.py` & `directdb-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.5'
+VERSION = '1.1.6'
 DESCRIPTION = 'An async package that makes database handling extremely easy!'
 
 # Setting up
 setup(
     name="directdb",
     version=VERSION,
     author="Cannonball Chris",
```

