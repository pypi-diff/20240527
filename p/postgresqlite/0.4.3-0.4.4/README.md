# Comparing `tmp/postgresqlite-0.4.3.tar.gz` & `tmp/postgresqlite-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgresqlite-0.4.3.tar", max compression
+gzip compressed data, was "postgresqlite-0.4.4.tar", max compression
```

## Comparing `postgresqlite-0.4.3.tar` & `postgresqlite-0.4.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    15321 2023-09-18 08:02:44.103406 postgresqlite-0.4.3/README.md
--rw-r--r--   0        0        0    19628 2023-09-18 08:08:16.706347 postgresqlite-0.4.3/postgresqlite/__init__.py
--rw-r--r--   0        0        0       27 2022-10-12 06:58:47.552893 postgresqlite-0.4.3/postgresqlite/__main__.py
--rw-r--r--   0        0        0      822 2023-09-18 08:08:27.702861 postgresqlite-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    16362 1970-01-01 00:00:00.000000 postgresqlite-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    15321 2023-09-18 08:02:44.103406 postgresqlite-0.4.4/README.md
+-rw-r--r--   0        0        0    19948 2024-05-27 06:51:31.617437 postgresqlite-0.4.4/postgresqlite/__init__.py
+-rw-r--r--   0        0        0       27 2022-10-12 06:58:47.552893 postgresqlite-0.4.4/postgresqlite/__main__.py
+-rw-r--r--   0        0        0      822 2024-05-27 06:52:54.860912 postgresqlite-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    16413 1970-01-01 00:00:00.000000 postgresqlite-0.4.4/PKG-INFO
```

### Comparing `postgresqlite-0.4.3/README.md` & `postgresqlite-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `postgresqlite-0.4.3/postgresqlite/__init__.py` & `postgresqlite-0.4.4/postgresqlite/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,20 @@
                 '-U', config.user,
                 f'--pwfile={password_file}'
             ], check=True, stderr=log_fd, stdout=log_fd)
 
             os.remove(password_file)
 
         print("Starting PostgreSQL..", file=sys.stderr)
+        try:
+            import pydevd
+            print("Unable to start the PostgreSQL server when running within the Python debugger. When running your program for the first time in a while, please do so without the debugger. (Ctrl-F5 in VSCode)")
+            sys.exit(1)
+        except ImportError:
+            pass
         _run_as_daemon(lambda: _run_server(daemon_fd, log_fd, config), keep_fds={daemon_fd,log_fd}, change_cwd=False)
 
     client_file = lockdir + "/" + _make_random_word()
     global client_fd # to make sure the GC doesn't close our file
     client_fd = open(client_file, "w")
     fcntl.flock(client_fd, fcntl.LOCK_EX)
```

### Comparing `postgresqlite-0.4.3/pyproject.toml` & `postgresqlite-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postgresqlite"
-version = "0.4.3"
+version = "0.4.4"
 description = "Python package that gives you the power of a PostgreSQL server, with the convenience of the sqlite3 package."
 authors = ["Frank van Viegen <pp@vanviegen.net>"]
 readme = "README.md"
 repository = "https://github.com/vanviegen/postgresqlite"
 documentation = "https://github.com/vanviegen/postgresqlite/blob/master/README.md#Documentation"
 classifiers = [
     'Development Status :: 4 - Beta',
```

### Comparing `postgresqlite-0.4.3/PKG-INFO` & `postgresqlite-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: postgresqlite
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python package that gives you the power of a PostgreSQL server, with the convenience of the sqlite3 package.
 Home-page: https://github.com/vanviegen/postgresqlite
 Author: Frank van Viegen
 Author-email: pp@vanviegen.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
 Requires-Dist: pg8000 (>=1.24.1,<2.0.0)
 Project-URL: Documentation, https://github.com/vanviegen/postgresqlite/blob/master/README.md#Documentation
 Project-URL: Repository, https://github.com/vanviegen/postgresqlite
 Description-Content-Type: text/markdown
 
 # PostgreSQLite
```

