# Comparing `tmp/pynonymizer-2.2.0.tar.gz` & `tmp/pynonymizer-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynonymizer-2.2.0.tar", last modified: Sun Apr 14 16:33:37 2024, max compression
+gzip compressed data, was "pynonymizer-2.2.1.tar", last modified: Tue Apr 30 21:35:40 2024, max compression
```

## Comparing `pynonymizer-2.2.0.tar` & `pynonymizer-2.2.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.302275 pynonymizer-2.2.0/
--rw-r--r--   0 root         (0) root         (0)     1050 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6537 2024-04-14 16:33:37.302275 pynonymizer-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5684 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.294275 pynonymizer-2.2.0/pynonymizer/
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/__main__.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.294275 pynonymizer-2.2.0/pynonymizer/database/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/__init__.py
--rw-r--r--   0 root         (0) root         (0)      934 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2791 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/pynonymizer/database/mssql/
--rw-r--r--   0 root         (0) root         (0)    16778 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8518 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/mssql/connectionstring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/pynonymizer/database/mysql/
--rw-r--r--   0 root         (0) root         (0)     7478 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5214 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/mysql/execution.py
--rw-r--r--   0 root         (0) root         (0)     4560 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/mysql/query_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/pynonymizer/database/postgres/
--rw-r--r--   0 root         (0) root         (0)     7321 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4305 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/postgres/execution.py
--rw-r--r--   0 root         (0) root         (0)     5252 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/postgres/query_factory.py
--rw-r--r--   0 root         (0) root         (0)       48 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/provider.py
--rw-r--r--   0 root         (0) root         (0)      317 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/pynonymizer/fake/
--rw-r--r--   0 root         (0) root         (0)     3823 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/fake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3848 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/process_steps.py
--rw-r--r--   0 root         (0) root         (0)     4750 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/pynonymize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/pynonymizer/strategy/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      543 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/config.py
--rw-r--r--   0 root         (0) root         (0)     1910 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/database.py
--rw-r--r--   0 root         (0) root         (0)      797 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8132 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/parser.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/table.py
--rw-r--r--   0 root         (0) root         (0)     3283 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/update_column.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/pynonymizer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6537 2024-04-14 16:33:37.000000 pynonymizer-2.2.0/pynonymizer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1144 2024-04-14 16:33:37.000000 pynonymizer-2.2.0/pynonymizer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 16:33:37.000000 pynonymizer-2.2.0/pynonymizer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-14 16:33:37.000000 pynonymizer-2.2.0/pynonymizer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-14 16:33:37.000000 pynonymizer-2.2.0/pynonymizer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-14 16:33:37.000000 pynonymizer-2.2.0/pynonymizer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      122 2024-04-14 16:33:37.302275 pynonymizer-2.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1235 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)      462 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/tests/test_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:35:40.953166 pynonymizer-2.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1050 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6537 2024-04-30 21:35:40.953166 pynonymizer-2.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5684 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:35:40.945166 pynonymizer-2.2.1/pynonymizer/
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    10092 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:35:40.949166 pynonymizer-2.2.1/pynonymizer/database/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/database/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      934 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/database/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/database/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:35:40.949166 pynonymizer-2.2.1/pynonymizer/database/mssql/
+-rw-r--r--   0 root         (0) root         (0)    16778 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/database/mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8518 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/database/mssql/connectionstring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:35:40.949166 pynonymizer-2.2.1/pynonymizer/database/mysql/
+-rw-r--r--   0 root         (0) root         (0)     7478 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/database/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5214 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/database/mysql/execution.py
+-rw-r--r--   0 root         (0) root         (0)     4560 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/database/mysql/query_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:35:40.949166 pynonymizer-2.2.1/pynonymizer/database/postgres/
+-rw-r--r--   0 root         (0) root         (0)     7321 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/database/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/database/postgres/execution.py
+-rw-r--r--   0 root         (0) root         (0)     5252 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/database/postgres/query_factory.py
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/database/provider.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:35:40.949166 pynonymizer-2.2.1/pynonymizer/fake/
+-rw-r--r--   0 root         (0) root         (0)     3823 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/fake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/process_steps.py
+-rw-r--r--   0 root         (0) root         (0)     4750 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/pynonymize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:35:40.953166 pynonymizer-2.2.1/pynonymizer/strategy/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/strategy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      543 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/strategy/config.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/strategy/database.py
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/strategy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8132 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/strategy/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/strategy/table.py
+-rw-r--r--   0 root         (0) root         (0)     3283 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/pynonymizer/strategy/update_column.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:35:40.953166 pynonymizer-2.2.1/pynonymizer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6537 2024-04-30 21:35:40.000000 pynonymizer-2.2.1/pynonymizer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-30 21:35:40.000000 pynonymizer-2.2.1/pynonymizer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 21:35:40.000000 pynonymizer-2.2.1/pynonymizer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-30 21:35:40.000000 pynonymizer-2.2.1/pynonymizer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-30 21:35:40.000000 pynonymizer-2.2.1/pynonymizer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-30 21:35:40.000000 pynonymizer-2.2.1/pynonymizer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2024-04-30 21:35:40.953166 pynonymizer-2.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:35:40.953166 pynonymizer-2.2.1/tests/
+-rw-r--r--   0 root         (0) root         (0)      462 2024-04-30 21:35:33.000000 pynonymizer-2.2.1/tests/test_meta.py
```

### Comparing `pynonymizer-2.2.0/LICENSE` & `pynonymizer-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/PKG-INFO` & `pynonymizer-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynonymizer
-Version: 2.2.0
+Version: 2.2.1
 Summary: An anonymization tool for production databases
 Home-page: https://github.com/rwnx/pynonymizer
 Author: Rowan Twell
 Author-email: rowantwell@gmail.com
 License: MIT
 Keywords: anonymization gdpr database mysql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pynonymizer-2.2.0/README.md` & `pynonymizer-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/cli.py` & `pynonymizer-2.2.1/pynonymizer/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,18 @@
             "-i",
             help="The source dump filepath to read from. Use `-` for stdin.",
         ),
     ] = None,
     strategyfile: Annotated[
         str,
         typer.Option(
-            "--strategy", "-s", help="A strategyfile to use during anonymization."
+            "--strategy",
+            "-s",
+            help="A strategyfile to use during anonymization.",
+            envvar=["PYNONYMIZER_STRATEGY", "PYNONYMIZER_STRATEGYFILE"],
         ),
     ] = None,
     output: Annotated[
         str,
         typer.Option(
             "--output",
             "-o",
@@ -53,30 +56,36 @@
     db_name: Annotated[str, typer.Option("--db-name", "-n")] = None,
     db_user: Annotated[str, typer.Option("--db-user", "-u")] = None,
     db_password: Annotated[str, typer.Option("--db-password", "-p")] = None,
     db_workers: Annotated[int, typer.Option("--workers", "-w")] = 1,
     start_at_step: Annotated[
         str,
         typer.Option(
-            "--start-at", help="Choose a step to begin the process (inclusive)."
+            "--start-at",
+            help="Choose a step to begin the process (inclusive).",
+            envvar=["PYNONYMIZER_START_AT", "PYNONYMIZER_START_AT_STEP"],
         ),
     ] = "START",
     only_step: Annotated[str, typer.Option(help="Choose one step to perform.")] = None,
     skip_steps: Annotated[
         List[str],
         typer.Option(
             "--skip-steps",
             show_envvar=True,
             help="Choose one or more steps to skip",
             case_sensitive=False,
         ),
     ] = None,
     stop_at_step: Annotated[
         str,
-        typer.Option("--stop-at", help="Choose a step to stop at (inclusive)."),
+        typer.Option(
+            "--stop-at",
+            help="Choose a step to stop at (inclusive).",
+            envvar=["PYNONYMIZER_STOP_AT", "PYNONYMIZER_STOP_AT_STEP"],
+        ),
     ] = "END",
     seed_rows: Annotated[
         int,
         typer.Option(
             min=1,
             show_envvar=True,
             help="Number of rows to populate the fake data table used during anonymization",
@@ -89,15 +98,15 @@
             "-c",
             help="Pass additional options to the pyodbc connection. overrides existing connection arguments.",
         ),
     ] = None,
     mssql_driver: Annotated[
         str,
         typer.Option(
-            "--mssql-backup-compression",
+            "--mssql-driver",
             help="[mssql] ODBC driver to use for database connection.",
         ),
     ] = None,
     mssql_backup_compression: Annotated[
         bool,
         typer.Option(
             "--mssql-backup-compression",
@@ -117,29 +126,29 @@
             "--mysql-cmd-opts",
             help="[mysql] pass additional arguments to the restore process.",
         ),
     ] = None,
     mysql_dump_opts: Annotated[
         str,
         typer.Option(
-            "--mysql-cmd-opts",
+            "--mysql-dump-opts",
             help="[mysql] pass additional arguments to the dump process.",
         ),
     ] = None,
     postgres_cmd_opts: Annotated[
         str,
         typer.Option(
-            "--mysql-cmd-opts",
+            "--postgres-cmd-opts",
             help="[postgres] pass additional arguments to the restore process.",
         ),
     ] = None,
     postgres_dump_opts: Annotated[
         str,
         typer.Option(
-            "--mysql-cmd-opts",
+            "--postgres-dump-opts",
             help="[postgres] pass additional arguments to the dump process.",
         ),
     ] = None,
     dry_run: Annotated[
         bool,
         typer.Option(
             "--dry-run", help="Skip all process steps. Useful for testing safely."
@@ -232,58 +241,58 @@
             mssql_connection_string=mssql_connection_string,
             mssql_ansi_warnings_off=mssql_ansi_warnings_off,
         )
     except ModuleNotFoundError as error:
         if error.name == "pyodbc" and db_type == "mssql":
             root_logger.error("Missing Required Packages for database support.")
             root_logger.error("Install package extras: pip install pynonymizer[mssql]")
-            return typer.Exit(1)
+            raise typer.Exit(1)
         else:
             raise error
     except ImportError as error:
         if error.name == "pyodbc" and db_type == "mssql":
             root_logger.error(
                 "Error importing pyodbc (mssql). "
                 "The ODBC driver may not be installed on your system. See package `unixodbc`."
             )
-            return typer.Exit(1)
+            raise typer.Exit(1)
         else:
             raise error
     except DatabaseConnectionError as error:
         root_logger.error("Failed to connect to database.")
         if verbose:
             root_logger.error(error)
-        return typer.Exit(1)
+        raise typer.Exit(1)
     except ArgumentValidationError as error:
         root_logger.error(
             "Missing values for required arguments: \n"
             + "\n".join(error.validation_messages)
             + "\nSet these using the command-line options or with environment variables. \n"
             "For a complete list, See: `pynonymizer --help`.\n"
         )
-        return typer.Exit(2)
+        raise typer.Exit(2)
     except UnsupportedFakeArgumentsError as error:
         root_logger.error(
             f"There was an error while parsing the strategyfile. Unknown fake type: {error.fake_type} \n "
             + f"This happens when additional kwargs are passed to a fake type that it doesnt support. \n"
             + f"You can only configure generators using kwargs that Faker supports. \n"
             + f"See https://github.com/rwnx/pynonymizer/blob/main/doc/strategyfiles.md#column-strategy-fake_update for usage information."
         )
-        return typer.Exit(1)
+        raise typer.Exit(1)
     except UnsupportedFakeTypeError as error:
         root_logger.error(
             f"There was an error while parsing the strategyfile. Unknown fake type: {error.fake_type} \n "
             + f"This happens when an fake_update column strategy is used with a generator that doesn't exist. \n"
             + f"You can only use data types that Faker supports. \n"
             + f"See https://github.com/rwnx/pynonymizer/blob/main/doc/strategyfiles.md#column-strategy-fake_update for usage information."
         )
-        return typer.Exit(1)
+        raise typer.Exit(1)
     except CalledProcessError as error:
         root_logger.error(error)
-        return typer.Exit(1)
+        raise typer.Exit(1)
 
 
 def cli():
     app()
 
 
 if __name__ == "__main__":
```

### Comparing `pynonymizer-2.2.0/pynonymizer/database/exceptions.py` & `pynonymizer-2.2.1/pynonymizer/database/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/database/io.py` & `pynonymizer-2.2.1/pynonymizer/database/io.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/database/mssql/__init__.py` & `pynonymizer-2.2.1/pynonymizer/database/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/database/mssql/connectionstring.py` & `pynonymizer-2.2.1/pynonymizer/database/mssql/connectionstring.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/database/mysql/__init__.py` & `pynonymizer-2.2.1/pynonymizer/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/database/mysql/execution.py` & `pynonymizer-2.2.1/pynonymizer/database/mysql/execution.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/database/mysql/query_factory.py` & `pynonymizer-2.2.1/pynonymizer/database/mysql/query_factory.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/database/postgres/__init__.py` & `pynonymizer-2.2.1/pynonymizer/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/database/postgres/execution.py` & `pynonymizer-2.2.1/pynonymizer/database/postgres/execution.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/database/postgres/query_factory.py` & `pynonymizer-2.2.1/pynonymizer/database/postgres/query_factory.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/fake/__init__.py` & `pynonymizer-2.2.1/pynonymizer/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/process_steps.py` & `pynonymizer-2.2.1/pynonymizer/process_steps.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/pynonymize.py` & `pynonymizer-2.2.1/pynonymizer/pynonymize.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/strategy/config.py` & `pynonymizer-2.2.1/pynonymizer/strategy/config.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/strategy/database.py` & `pynonymizer-2.2.1/pynonymizer/strategy/database.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/strategy/exceptions.py` & `pynonymizer-2.2.1/pynonymizer/strategy/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/strategy/parser.py` & `pynonymizer-2.2.1/pynonymizer/strategy/parser.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/strategy/table.py` & `pynonymizer-2.2.1/pynonymizer/strategy/table.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer/strategy/update_column.py` & `pynonymizer-2.2.1/pynonymizer/strategy/update_column.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/pynonymizer.egg-info/PKG-INFO` & `pynonymizer-2.2.1/pynonymizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynonymizer
-Version: 2.2.0
+Version: 2.2.1
 Summary: An anonymization tool for production databases
 Home-page: https://github.com/rwnx/pynonymizer
 Author: Rowan Twell
 Author-email: rowantwell@gmail.com
 License: MIT
 Keywords: anonymization gdpr database mysql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pynonymizer-2.2.0/pynonymizer.egg-info/SOURCES.txt` & `pynonymizer-2.2.1/pynonymizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.2.0/setup.py` & `pynonymizer-2.2.1/setup.py`

 * *Files identical despite different names*

