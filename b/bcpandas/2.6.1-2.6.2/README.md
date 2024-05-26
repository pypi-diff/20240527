# Comparing `tmp/bcpandas-2.6.1.tar.gz` & `tmp/bcpandas-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcpandas-2.6.1.tar", max compression
+gzip compressed data, was "bcpandas-2.6.2.tar", max compression
```

## Comparing `bcpandas-2.6.1.tar` & `bcpandas-2.6.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2024-04-04 02:40:58.560387 bcpandas-2.6.1/LICENSE
--rw-r--r--   0        0        0    19148 2024-04-04 02:40:58.560387 bcpandas-2.6.1/README.md
--rw-r--r--   0        0        0      563 2024-04-04 02:40:58.560387 bcpandas-2.6.1/bcpandas/__init__.py
--rw-r--r--   0        0        0     2339 2024-04-04 02:40:58.560387 bcpandas-2.6.1/bcpandas/constants.py
--rw-r--r--   0        0        0    17835 2024-04-04 02:40:58.560387 bcpandas-2.6.1/bcpandas/main.py
--rw-r--r--   0        0        0     8576 2024-04-04 02:40:58.560387 bcpandas-2.6.1/bcpandas/utils.py
--rw-r--r--   0        0        0     2545 2024-04-04 02:41:11.984529 bcpandas-2.6.1/pyproject.toml
--rw-r--r--   0        0        0    20256 1970-01-01 00:00:00.000000 bcpandas-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-26 23:31:17.678450 bcpandas-2.6.2/LICENSE
+-rw-r--r--   0        0        0    19148 2024-05-26 23:31:17.678450 bcpandas-2.6.2/README.md
+-rw-r--r--   0        0        0      563 2024-05-26 23:31:17.678450 bcpandas-2.6.2/bcpandas/__init__.py
+-rw-r--r--   0        0        0     2339 2024-05-26 23:31:17.678450 bcpandas-2.6.2/bcpandas/constants.py
+-rw-r--r--   0        0        0    18070 2024-05-26 23:31:17.678450 bcpandas-2.6.2/bcpandas/main.py
+-rw-r--r--   0        0        0     8666 2024-05-26 23:31:17.678450 bcpandas-2.6.2/bcpandas/utils.py
+-rw-r--r--   0        0        0     2494 2024-05-26 23:31:31.798656 bcpandas-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0    20256 1970-01-01 00:00:00.000000 bcpandas-2.6.2/PKG-INFO
```

### Comparing `bcpandas-2.6.1/LICENSE` & `bcpandas-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bcpandas-2.6.1/README.md` & `bcpandas-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `bcpandas-2.6.1/bcpandas/__init__.py` & `bcpandas-2.6.2/bcpandas/__init__.py`

 * *Files identical despite different names*

### Comparing `bcpandas-2.6.1/bcpandas/constants.py` & `bcpandas-2.6.2/bcpandas/constants.py`

 * *Files identical despite different names*

### Comparing `bcpandas-2.6.1/bcpandas/main.py` & `bcpandas-2.6.2/bcpandas/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -351,14 +351,15 @@
     process_dest_table: bool = True,
     print_output: bool = True,
     delimiter: Optional[str] = None,
     quotechar: Optional[str] = None,
     encoding: Optional[str] = None,
     work_directory: Optional[Path] = None,
     collation: str = sql_collation,
+    identity_insert: bool = False,
 ):
     """
     Writes the pandas DataFrame to a SQL table or view.
 
     Will write all columns to the table or view. If the destination table/view doesn't exist, will create it.
     Assumes the SQL table/view has the same number, name, and type of columns.
     To only write parts of the DataFrame, filter it beforehand and pass that to this function.
@@ -411,14 +412,16 @@
     quotechar: str, default None
         Optional quotechar to use, otherwise will use the result of `constants.get_quotechar`
     encoding: str, default None
         Optional encoding to use for writing the BCP data-file. Defaults to `utf-8`.
     work_directory: pathlib.Path, default None
         Optional directory where temporary files are written to. If not provided, defaults to the
         system-default for temporary files.
+    identity_insert: bool, default False
+        Specifies that identity value or values in the imported data file are to be used for the identity column.
 
     Notes
     -----
     If `delimiter` and/or `quotechar` are specified, you must ensure that those characters
     are not present in the actual data.
     """
     # validation
@@ -495,14 +498,15 @@
             creds=creds,
             print_output=print_output,
             sql_type=sql_type,
             schema=schema,
             batch_size=batch_size,
             use_tablock=use_tablock,
             bcp_path=bcp_path,
+            identity_insert=identity_insert,
         )
     finally:
         if not debug:
             logger.debug("Deleting temp CSV and format files")
             os.remove(csv_file_path)
             os.remove(fmt_file_path)
         else:
```

### Comparing `bcpandas-2.6.1/bcpandas/utils.py` & `bcpandas-2.6.2/bcpandas/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     schema: str = "dbo",
     format_file_path: Optional[Path] = None,
     batch_size: Optional[int] = None,
     use_tablock: bool = False,
     col_delimiter: Optional[str] = None,
     row_terminator: Optional[str] = None,
     bcp_path: Optional[Union[str, Path]] = None,
+    identity_insert: bool = False,
 ):
     """
     See https://docs.microsoft.com/en-us/sql/tools/bcp-utility
     """
     combos = {TABLE: [IN, OUT], QUERY: [QUERYOUT], VIEW: [IN, OUT]}
     direc = direction.lower()
     # validation
@@ -106,14 +107,17 @@
 
     if batch_size:
         bcp_command += ["-b", str(batch_size)]
 
     if use_tablock:
         bcp_command += ["-h", "TABLOCK"]
 
+    if identity_insert:
+        bcp_command += ["-E"]
+
     # formats
     if direc == IN and format_file_path is not None:
         bcp_command += ["-f", str(format_file_path)]
     elif direc in (OUT, QUERYOUT):
         bcp_command += [
             "-c",  # marking as character data, not Unicode (maybe make as param?)
             quote_this(
```

### Comparing `bcpandas-2.6.1/pyproject.toml` & `bcpandas-2.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 description = "High-level wrapper around BCP for high performance data transfers between pandas and SQL Server. No knowledge of BCP required!!"
 keywords = ["bcp", "mssql", "pandas"]
 license = "MIT"
 maintainers = ["Oliver Borchert <me@borchero.com>"]
 name = "bcpandas"
 readme = "README.md"
 repository = "https://github.com/yehoshuadimarsky/bcpandas"
-version = "v2.6.1"
+version = "2.6.2"
 
 [tool.poetry.plugins."pandas.sql.engine"]
 bcpandas = "bcpandas.main:to_sql"
 
 [tool.poetry.dependencies]
 pandas = ">=1.5"
 pyodbc = "*"
@@ -33,23 +33,22 @@
 pre-commit = "*"
 black = "*"
 mypy = "*"
 ruff = "^0"
 types-setuptools = "*"
 
 [tool.poetry.group.test.dependencies]
-codetiming = "1.4.0"
-docker = "6.0.1"
-hypothesis = "6.64.0"
+codetiming = "*"
+docker = "*"
+hypothesis = "*"
 ipython = "8.10.0"
-matplotlib = "3.6.3"
-pytest = "7.2.1"
-pytest-cov = "4.0.0"
-requests = "2.31.0"
-urllib3 = "1.26.18"
+matplotlib = "*"
+pytest = "*"
+pytest-cov = "*"
+requests = "*"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 # Example configuration for Black.
```

### Comparing `bcpandas-2.6.1/PKG-INFO` & `bcpandas-2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcpandas
-Version: 2.6.1
+Version: 2.6.2
 Summary: High-level wrapper around BCP for high performance data transfers between pandas and SQL Server. No knowledge of BCP required!!
 Home-page: https://github.com/yehoshuadimarsky/bcpandas
 License: MIT
 Keywords: bcp,mssql,pandas
 Author: yehoshuadimarsky
 Maintainer: Oliver Borchert
 Maintainer-email: me@borchero.com
```

