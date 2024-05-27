# Comparing `tmp/sqlite_logging-0.0.2.tar.gz` & `tmp/sqlite_logging-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite_logging-0.0.2.tar", last modified: Mon Apr 15 19:10:23 2024, max compression
+gzip compressed data, was "sqlite_logging-0.0.3.tar", last modified: Mon May 27 21:41:33 2024, max compression
```

## Comparing `sqlite_logging-0.0.2.tar` & `sqlite_logging-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 brohrer   (1000) brohrer   (1000)        0 2024-04-15 19:10:23.752140 sqlite_logging-0.0.2/
--rw-rw-r--   0 brohrer   (1000) brohrer   (1000)     1071 2024-04-14 14:21:43.000000 sqlite_logging-0.0.2/LICENSE
--rw-r--r--   0 brohrer   (1000) brohrer   (1000)     4061 2024-04-15 19:10:23.752140 sqlite_logging-0.0.2/PKG-INFO
--rw-rw-r--   0 brohrer   (1000) brohrer   (1000)     3618 2024-04-15 19:08:50.000000 sqlite_logging-0.0.2/README.md
--rw-rw-r--   0 brohrer   (1000) brohrer   (1000)      523 2024-04-15 19:09:22.000000 sqlite_logging-0.0.2/pyproject.toml
--rw-rw-r--   0 brohrer   (1000) brohrer   (1000)       38 2024-04-15 19:10:23.752140 sqlite_logging-0.0.2/setup.cfg
-drwxrwxr-x   0 brohrer   (1000) brohrer   (1000)        0 2024-04-15 19:10:23.752140 sqlite_logging-0.0.2/sqlite_logging.egg-info/
--rw-r--r--   0 brohrer   (1000) brohrer   (1000)     4061 2024-04-15 19:10:23.000000 sqlite_logging-0.0.2/sqlite_logging.egg-info/PKG-INFO
--rw-rw-r--   0 brohrer   (1000) brohrer   (1000)      276 2024-04-15 19:10:23.000000 sqlite_logging-0.0.2/sqlite_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 brohrer   (1000) brohrer   (1000)        1 2024-04-15 19:10:23.000000 sqlite_logging-0.0.2/sqlite_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 brohrer   (1000) brohrer   (1000)       10 2024-04-15 19:10:23.000000 sqlite_logging-0.0.2/sqlite_logging.egg-info/top_level.txt
-drwxrwxr-x   0 brohrer   (1000) brohrer   (1000)        0 2024-04-15 19:10:23.752140 sqlite_logging-0.0.2/sqlogging/
--rw-rw-r--   0 brohrer   (1000) brohrer   (1000)        0 2024-04-14 14:46:18.000000 sqlite_logging-0.0.2/sqlogging/__init__.py
--rw-rw-r--   0 brohrer   (1000) brohrer   (1000)      672 2024-04-15 19:08:51.000000 sqlite_logging-0.0.2/sqlogging/benchmark.py
--rw-rw-r--   0 brohrer   (1000) brohrer   (1000)     3369 2024-04-15 19:08:50.000000 sqlite_logging-0.0.2/sqlogging/logging.py
--rw-rw-r--   0 brohrer   (1000) brohrer   (1000)     7223 2024-04-15 17:15:59.000000 sqlite_logging-0.0.2/sqlogging/test_logging.py
+drwxrwxr-x   0 brohrer   (1000) brohrer   (1000)        0 2024-05-27 21:41:33.810864 sqlite_logging-0.0.3/
+-rw-rw-r--   0 brohrer   (1000) brohrer   (1000)     1071 2024-04-14 14:21:43.000000 sqlite_logging-0.0.3/LICENSE
+-rw-r--r--   0 brohrer   (1000) brohrer   (1000)     4175 2024-05-27 21:41:33.810864 sqlite_logging-0.0.3/PKG-INFO
+-rw-rw-r--   0 brohrer   (1000) brohrer   (1000)     3732 2024-05-27 21:39:56.000000 sqlite_logging-0.0.3/README.md
+-rw-rw-r--   0 brohrer   (1000) brohrer   (1000)      523 2024-05-27 20:29:29.000000 sqlite_logging-0.0.3/pyproject.toml
+-rw-rw-r--   0 brohrer   (1000) brohrer   (1000)       38 2024-05-27 21:41:33.810864 sqlite_logging-0.0.3/setup.cfg
+drwxrwxr-x   0 brohrer   (1000) brohrer   (1000)        0 2024-05-27 21:41:33.810864 sqlite_logging-0.0.3/sqlite_logging.egg-info/
+-rw-r--r--   0 brohrer   (1000) brohrer   (1000)     4175 2024-05-27 21:41:33.000000 sqlite_logging-0.0.3/sqlite_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 brohrer   (1000) brohrer   (1000)      276 2024-05-27 21:41:33.000000 sqlite_logging-0.0.3/sqlite_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 brohrer   (1000) brohrer   (1000)        1 2024-05-27 21:41:33.000000 sqlite_logging-0.0.3/sqlite_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 brohrer   (1000) brohrer   (1000)       10 2024-05-27 21:41:33.000000 sqlite_logging-0.0.3/sqlite_logging.egg-info/top_level.txt
+drwxrwxr-x   0 brohrer   (1000) brohrer   (1000)        0 2024-05-27 21:41:33.810864 sqlite_logging-0.0.3/sqlogging/
+-rw-rw-r--   0 brohrer   (1000) brohrer   (1000)        0 2024-04-14 14:46:18.000000 sqlite_logging-0.0.3/sqlogging/__init__.py
+-rw-rw-r--   0 brohrer   (1000) brohrer   (1000)      672 2024-04-15 19:08:51.000000 sqlite_logging-0.0.3/sqlogging/benchmark.py
+-rw-rw-r--   0 brohrer   (1000) brohrer   (1000)     3980 2024-05-27 20:17:36.000000 sqlite_logging-0.0.3/sqlogging/logging.py
+-rw-rw-r--   0 brohrer   (1000) brohrer   (1000)     7560 2024-05-27 20:18:31.000000 sqlite_logging-0.0.3/sqlogging/test_logging.py
```

### Comparing `sqlite_logging-0.0.2/LICENSE` & `sqlite_logging-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite_logging-0.0.2/PKG-INFO` & `sqlite_logging-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: sqlite-logging
-Version: 0.0.2
+Version: 0.0.3
 Summary: SQLite3-based logging for Python
 Author-email: Brandon Rohrer <brohrer@gmail.com>
 Project-URL: Repository, https://github.com/brohrer/sqlogging
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sqlogging
 
 A logger that is based on Python's
 [sqlite3](https://docs.python.org/3/library/sqlite3.html)
-library. Log entries are stored in a sqlite table and can be accessed
+library. Log entries are stored in a SQLite table and can be accessed
 with SQL queries.
 It is inspired by the [logging](https://docs.python.org/3/library/logging.html)
 library, but does not stay strictly faithful to the API. 
 
 The strength of sqlogging isn't speed. It typically takes a few milliseconds
 to write a log entry (about 7 ms on my machine).
 But if that's not a blocker for you, the accessibility and flexibility of analysis
@@ -49,15 +49,15 @@
 ```
 
 ## API
 
 ### `create_logger()`
 `logging.create_logger(name="log", dir_name=".", level="info", columns=["ts", "data"])`
 
-For creating a new Logger from scratch. If you try to open a Logger by the same name
+For creating a new Logger from scratch. If you try to create a Logger by the same name
 as a pre-existing logger you'll get a `sqlite3.OperationalError`.
 
 * Parameters
   * `name`(`str`) - The name of the Logger. This will be both the name of the
   name of the table and the name of the sqlite3 database file (`<name>.db`).
   * `dir_name`(`str`) - The directory in which the database file will be stored.
   If it doesn't already exist, it will be created.
@@ -67,23 +67,24 @@
   * `columns`(`List` of `str`) - The names of the columns to be created in the
   sqlite database.
 * Return type: `Logger`
 * Raises:
   * `ValueError`: If `level` is not one of the 5 allowed levels.
 
 ### `open_logger()`
-`logging.open_logger(name="log", dir_name=".")`
+`logging.open_logger(name="log", dir_name=".", level="info")`
 
-For re-opening an existing Logger.
+For re-opening an existing Logger. If you try to open a Logger
+that doesn't already exist you'll get a `sqlite3.OperationalError`.
 
 * Parameters: as in `create_logger()`
 * Return type: `Logger`
 
 ### `Logger`
-*class* `logging.Logger(name, dir_name, level=None, columns=None, create=True)`
+*class* `logging.Logger(name, dir_name, level="info", columns=None, create=True)`
 * Parameters: as in `create_logger()`
   * `create`(`bool`) - Whether a new Logger should be created or an existing
   one re-opened.
 
 #### `close()`
 Close the connection to the logger database. Can be reopened later with
 `logging.open_logger()`.
```

### Comparing `sqlite_logging-0.0.2/README.md` & `sqlite_logging-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # sqlogging
 
 A logger that is based on Python's
 [sqlite3](https://docs.python.org/3/library/sqlite3.html)
-library. Log entries are stored in a sqlite table and can be accessed
+library. Log entries are stored in a SQLite table and can be accessed
 with SQL queries.
 It is inspired by the [logging](https://docs.python.org/3/library/logging.html)
 library, but does not stay strictly faithful to the API. 
 
 The strength of sqlogging isn't speed. It typically takes a few milliseconds
 to write a log entry (about 7 ms on my machine).
 But if that's not a blocker for you, the accessibility and flexibility of analysis
@@ -36,15 +36,15 @@
 ```
 
 ## API
 
 ### `create_logger()`
 `logging.create_logger(name="log", dir_name=".", level="info", columns=["ts", "data"])`
 
-For creating a new Logger from scratch. If you try to open a Logger by the same name
+For creating a new Logger from scratch. If you try to create a Logger by the same name
 as a pre-existing logger you'll get a `sqlite3.OperationalError`.
 
 * Parameters
   * `name`(`str`) - The name of the Logger. This will be both the name of the
   name of the table and the name of the sqlite3 database file (`<name>.db`).
   * `dir_name`(`str`) - The directory in which the database file will be stored.
   If it doesn't already exist, it will be created.
@@ -54,23 +54,24 @@
   * `columns`(`List` of `str`) - The names of the columns to be created in the
   sqlite database.
 * Return type: `Logger`
 * Raises:
   * `ValueError`: If `level` is not one of the 5 allowed levels.
 
 ### `open_logger()`
-`logging.open_logger(name="log", dir_name=".")`
+`logging.open_logger(name="log", dir_name=".", level="info")`
 
-For re-opening an existing Logger.
+For re-opening an existing Logger. If you try to open a Logger
+that doesn't already exist you'll get a `sqlite3.OperationalError`.
 
 * Parameters: as in `create_logger()`
 * Return type: `Logger`
 
 ### `Logger`
-*class* `logging.Logger(name, dir_name, level=None, columns=None, create=True)`
+*class* `logging.Logger(name, dir_name, level="info", columns=None, create=True)`
 * Parameters: as in `create_logger()`
   * `create`(`bool`) - Whether a new Logger should be created or an existing
   one re-opened.
 
 #### `close()`
 Close the connection to the logger database. Can be reopened later with
 `logging.open_logger()`.
```

### Comparing `sqlite_logging-0.0.2/pyproject.toml` & `sqlite_logging-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqlite-logging"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Brandon Rohrer", email="brohrer@gmail.com" },
 ]
 description = "SQLite3-based logging for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `sqlite_logging-0.0.2/sqlite_logging.egg-info/PKG-INFO` & `sqlite_logging-0.0.3/sqlite_logging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: sqlite-logging
-Version: 0.0.2
+Version: 0.0.3
 Summary: SQLite3-based logging for Python
 Author-email: Brandon Rohrer <brohrer@gmail.com>
 Project-URL: Repository, https://github.com/brohrer/sqlogging
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sqlogging
 
 A logger that is based on Python's
 [sqlite3](https://docs.python.org/3/library/sqlite3.html)
-library. Log entries are stored in a sqlite table and can be accessed
+library. Log entries are stored in a SQLite table and can be accessed
 with SQL queries.
 It is inspired by the [logging](https://docs.python.org/3/library/logging.html)
 library, but does not stay strictly faithful to the API. 
 
 The strength of sqlogging isn't speed. It typically takes a few milliseconds
 to write a log entry (about 7 ms on my machine).
 But if that's not a blocker for you, the accessibility and flexibility of analysis
@@ -49,15 +49,15 @@
 ```
 
 ## API
 
 ### `create_logger()`
 `logging.create_logger(name="log", dir_name=".", level="info", columns=["ts", "data"])`
 
-For creating a new Logger from scratch. If you try to open a Logger by the same name
+For creating a new Logger from scratch. If you try to create a Logger by the same name
 as a pre-existing logger you'll get a `sqlite3.OperationalError`.
 
 * Parameters
   * `name`(`str`) - The name of the Logger. This will be both the name of the
   name of the table and the name of the sqlite3 database file (`<name>.db`).
   * `dir_name`(`str`) - The directory in which the database file will be stored.
   If it doesn't already exist, it will be created.
@@ -67,23 +67,24 @@
   * `columns`(`List` of `str`) - The names of the columns to be created in the
   sqlite database.
 * Return type: `Logger`
 * Raises:
   * `ValueError`: If `level` is not one of the 5 allowed levels.
 
 ### `open_logger()`
-`logging.open_logger(name="log", dir_name=".")`
+`logging.open_logger(name="log", dir_name=".", level="info")`
 
-For re-opening an existing Logger.
+For re-opening an existing Logger. If you try to open a Logger
+that doesn't already exist you'll get a `sqlite3.OperationalError`.
 
 * Parameters: as in `create_logger()`
 * Return type: `Logger`
 
 ### `Logger`
-*class* `logging.Logger(name, dir_name, level=None, columns=None, create=True)`
+*class* `logging.Logger(name, dir_name, level="info", columns=None, create=True)`
 * Parameters: as in `create_logger()`
   * `create`(`bool`) - Whether a new Logger should be created or an existing
   one re-opened.
 
 #### `close()`
 Close the connection to the logger database. Can be reopened later with
 `logging.open_logger()`.
```

### Comparing `sqlite_logging-0.0.2/sqlogging/benchmark.py` & `sqlite_logging-0.0.3/sqlogging/benchmark.py`

 * *Files identical despite different names*

### Comparing `sqlite_logging-0.0.2/sqlogging/test_logging.py` & `sqlite_logging-0.0.3/sqlogging/test_logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,14 +161,30 @@
     )
     table_info = logger.query(f"PRAGMA table_info({logger.name});")
     assert len(table_info) == 5
 
     teardown_logger(logger)
 
 
+def test_open_nonexistent_log():
+    logger_name = "nonexistent_log"
+
+    allowed = True
+    try:
+        logger = logging.open_logger(
+            name=logger_name,
+            dir_name=TMP_LOGGER_DIR,
+        )
+        teardown_logger(logger)
+    except sqlite3.OperationalError:
+        allowed = False
+
+    assert allowed == False
+
+
 def test_writing_debug():
     logger = logging.create_logger(
         name="writing_debug",
         dir_name=TMP_LOGGER_DIR,
     )
     logger.info({"ts": 23874.2234, "data": "flurpy"})
     result = logger.query(f"SELECT * FROM {logger.name};")
```

