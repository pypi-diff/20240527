# Comparing `tmp/arrow_mssql-0.0.82.tar.gz` & `tmp/arrow_mssql-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrow_mssql-0.0.82.tar", max compression
+gzip compressed data, was "arrow_mssql-0.0.83.tar", max compression
```

## Comparing `arrow_mssql-0.0.82.tar` & `arrow_mssql-0.0.83.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      188 2024-04-10 19:20:44.547505 arrow_mssql-0.0.82/arrow_mssql/__init__.py
--rw-r--r--   0        0        0     1355 2024-05-13 19:47:30.898739 arrow_mssql-0.0.82/arrow_mssql/connector.py
--rw-r--r--   0        0        0     3609 2024-04-02 19:13:05.501619 arrow_mssql-0.0.82/arrow_mssql/export.py
--rw-r--r--   0        0        0        0 2024-04-02 17:17:13.445964 arrow_mssql-0.0.82/arrow_mssql/input/__init__.py
--rw-r--r--   0        0        0     3608 2024-04-10 18:24:20.692624 arrow_mssql-0.0.82/arrow_mssql/input/datatypes.py
--rw-r--r--   0        0        0     1568 2024-04-10 19:18:55.641653 arrow_mssql-0.0.82/arrow_mssql/input/schema.py
--rw-r--r--   0        0        0     1288 2024-04-10 18:36:45.564350 arrow_mssql-0.0.82/arrow_mssql/iport.py
--rw-r--r--   0        0        0        0 2024-04-02 17:15:34.399775 arrow_mssql-0.0.82/arrow_mssql/output/__init__.py
--rw-r--r--   0        0        0     2553 2024-04-02 19:07:18.402978 arrow_mssql-0.0.82/arrow_mssql/output/datatypes.py
--rw-r--r--   0        0        0     3435 2024-04-02 17:14:32.689965 arrow_mssql-0.0.82/arrow_mssql/output/schemas.py
--rw-r--r--   0        0        0      718 2024-03-18 12:53:20.396252 arrow_mssql-0.0.82/arrow_mssql/utils.py
--rw-r--r--   0        0        0      755 2024-05-13 19:42:58.634364 arrow_mssql-0.0.82/pyproject.toml
--rw-r--r--   0        0        0     1691 2024-05-13 19:45:26.619629 arrow_mssql-0.0.82/README.md
--rw-r--r--   0        0        0     2427 1970-01-01 00:00:00.000000 arrow_mssql-0.0.82/PKG-INFO
+-rw-r--r--   0        0        0      188 2024-05-27 17:56:55.897440 arrow_mssql-0.0.83/arrow_mssql/__init__.py
+-rw-r--r--   0        0        0     1425 2024-05-27 17:31:29.732859 arrow_mssql-0.0.83/arrow_mssql/connector.py
+-rw-r--r--   0        0        0     3649 2024-05-27 17:56:59.114932 arrow_mssql-0.0.83/arrow_mssql/export.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:17:13.445964 arrow_mssql-0.0.83/arrow_mssql/input/__init__.py
+-rw-r--r--   0        0        0     3600 2024-05-27 17:30:02.243740 arrow_mssql-0.0.83/arrow_mssql/input/datatypes.py
+-rw-r--r--   0        0        0     1568 2024-05-27 16:34:31.830782 arrow_mssql-0.0.83/arrow_mssql/input/schema.py
+-rw-r--r--   0        0        0     2240 2024-05-27 17:55:00.270584 arrow_mssql-0.0.83/arrow_mssql/iport.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:15:34.399775 arrow_mssql-0.0.83/arrow_mssql/output/__init__.py
+-rw-r--r--   0        0        0     2553 2024-04-02 19:07:18.402978 arrow_mssql-0.0.83/arrow_mssql/output/datatypes.py
+-rw-r--r--   0        0        0     3435 2024-04-02 17:14:32.689965 arrow_mssql-0.0.83/arrow_mssql/output/schemas.py
+-rw-r--r--   0        0        0      718 2024-03-18 12:53:20.396252 arrow_mssql-0.0.83/arrow_mssql/utils.py
+-rw-r--r--   0        0        0      755 2024-05-27 15:40:06.339505 arrow_mssql-0.0.83/pyproject.toml
+-rw-r--r--   0        0        0     1942 2024-05-27 17:56:52.708336 arrow_mssql-0.0.83/README.md
+-rw-r--r--   0        0        0     2666 1970-01-01 00:00:00.000000 arrow_mssql-0.0.83/PKG-INFO
```

### Comparing `arrow_mssql-0.0.82/arrow_mssql/connector.py` & `arrow_mssql-0.0.83/arrow_mssql/connector.py`

 * *Files 21% similar despite different names*

```diff
@@ -42,32 +42,36 @@
     )
 
     con.add_output_converter(
         -155, 
         datetimeoffset_to_datetime
     )
     
-    if 'autocommit' not in kwargs:
-        con.execute(
-            'set transaction '
-            'isolation level '
-            'read uncommitted;'
-        )
+    con.execute(
+        'set transaction '
+        'isolation level '
+        'read uncommitted;'
+    )
 
     with closing(con.cursor()) as cur:
         cur.execute("SET DATEFIRST 1")
 
     return con
 
 
 @contextlib.contextmanager
 def raw_sql(*args,**kwargs):
 
     con = do_connect(*args, **kwargs)
     cursor = con.cursor()
 
+    # NOTE: Adicionado o commit na conexao !
     try:
         yield cursor
-    except Exception:
+    except Exception:  
+        con.rollback()
         raise
+    else:
+        con.commit()
     finally:
-        cursor.close()
+        cursor.close()
+        con.close()
```

### Comparing `arrow_mssql-0.0.82/arrow_mssql/export.py` & `arrow_mssql-0.0.83/arrow_mssql/export.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def cursor_arrow(
     driver: str,
     name: str,
     database: str,
     schema: str = 'dbo',
-    limit: int = 1_000_000
+    chunk_size: int = 1_000_000
 ) -> Iterable[list]:
     
     with raw_sql(driver) as cursor:
         stmt = (
             sg.select('*')
             .from_(
                 sg.table(
@@ -30,24 +30,24 @@
             .sql('tsql')
         )
 
         if is_query(name):
             stmt = dedent(name)
 
         cursor.execute(stmt)
-        while batch := cursor.fetchmany(limit):
+        while batch := cursor.fetchmany(chunk_size):
             yield batch
 
 
 def to_arrow_lotes(
     driver: str,
     name: str,
     database: str,
     schema: str = 'dbo',
-    limit: int = 1_000_000
+    chunk_size: int = 1_000_000
 ) -> pa.ipc.RecordBatchReader:
     
     schema_arrow = get_schema(
         driver, 
         name, 
         database, 
         schema
@@ -57,15 +57,15 @@
     arrays = (
         pa.array(map(tuple, lote), type=array_type)
         for lote in cursor_arrow(
             driver, 
             name, 
             database, 
             schema,
-            limit   
+            chunk_size   
         )
     )
 
     lotes = map(
         pa.RecordBatch.from_struct_array, 
         arrays
     )
@@ -80,15 +80,15 @@
     driver: str,
     name: str,
     *,
     path: str,
     database: str,
     schema: str = 'dbo',
     row_group_size: int = 1_000_000,
-    limit: int = 1_000_000
+    chunk_size: int = 1_000_000
 ) -> None:
     """
     ### Exporta tabela ou consulta para .parquet
     
     ----
     driver: String de conexao `pyodbc`
     name: Tabela ou consulta
@@ -102,15 +102,15 @@
     import pyarrow.parquet as pq
     
     with to_arrow_lotes(
         driver, 
         name, 
         database, 
         schema, 
-        limit
+        chunk_size
     ) as lotes:
         
         with pq.ParquetWriter(path, lotes.schema) as writer:
             for lote in lotes:
                 writer.write_batch(
                     lote, 
                     row_group_size=row_group_size
@@ -121,15 +121,15 @@
     driver: str,
     name: str,
     *,
     path: str,
     database: str,
     schema: str = 'dbo',
     delimiter: str = ';',
-    limit: int = 1_000_000
+    chunk_size: int = 1_000_000
 ) -> None:
     """
     ### Exporta tabela ou consulta para .csv
     
     ----
     driver: String de conexao `pyodbc`
     name: Tabela ou consulta
@@ -143,15 +143,15 @@
     from pyarrow import csv
     
     with to_arrow_lotes(
         driver, 
         name, 
         database, 
         schema, 
-        limit
+        chunk_size
     ) as lotes:
         
         write_options = csv.WriteOptions(
             include_header=True,
             delimiter=delimiter, 
             quoting_style='all_valid'
         )
```

### Comparing `arrow_mssql-0.0.82/arrow_mssql/input/datatypes.py` & `arrow_mssql-0.0.83/arrow_mssql/input/datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,11 +130,11 @@
     pa.int64(): pyodbc.SQL_BIGINT,
     pa.bool_(): pyodbc.SQL_BIGINT,
     pa.float16(): pyodbc.SQL_REAL,
     pa.float32(): pyodbc.SQL_REAL,
     pa.float64(): pyodbc.SQL_FLOAT,
     pa.date32(): pyodbc.SQL_TYPE_DATE,
     pa.date64(): pyodbc.SQL_TYPE_DATE,
-    pa.string(): (pyodbc.SQL_VARCHAR, 8_000, 0),
-    pa.utf8(): (pyodbc.SQL_VARCHAR, 8_000, 0),
+    pa.string(): (pyodbc.SQL_VARCHAR, 0, 0),
+    pa.utf8(): (pyodbc.SQL_VARCHAR, 0, 0),
     pa.binary(): pyodbc.SQL_BINARY,
 }
```

### Comparing `arrow_mssql-0.0.82/arrow_mssql/input/schema.py` & `arrow_mssql-0.0.83/arrow_mssql/input/schema.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.82/arrow_mssql/output/datatypes.py` & `arrow_mssql-0.0.83/arrow_mssql/output/datatypes.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.82/arrow_mssql/output/schemas.py` & `arrow_mssql-0.0.83/arrow_mssql/output/schemas.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.82/arrow_mssql/utils.py` & `arrow_mssql-0.0.83/arrow_mssql/utils.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.82/pyproject.toml` & `arrow_mssql-0.0.83/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arrow-mssql"
-version = "0.0.82"
+version = "0.0.83"
 description = "Arrow-mssql exporta tabela ou consulta para .parquet ou .csv, e também faz a leitura de .parquet para tabela do sql server"
 authors = ["Marcus Holanda <mvsh777@hotmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Natural Language :: Portuguese (Brazilian)",
     "Programming Language :: PL/SQL",
```

### Comparing `arrow_mssql-0.0.82/README.md` & `arrow_mssql-0.0.83/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -64,8 +64,20 @@
 with write_parquet(
     DRIVER, 
     '##teste', 
     path='origem.parquet'
 ) as C:
 
     ...
+
+# AGORA é possivel importar um numero limite de linhas
+# e selecionar as colunas no arquivo parquet
+with write_parquet(
+    DRIVER, 
+    '##teste', 
+    path='origem.parquet',
+    limit=100,
+    columns=['col1', 'col2']
+) as C:
+
+    ...
 ```
```

### Comparing `arrow_mssql-0.0.82/PKG-INFO` & `arrow_mssql-0.0.83/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrow-mssql
-Version: 0.0.82
+Version: 0.0.83
 Summary: Arrow-mssql exporta tabela ou consulta para .parquet ou .csv, e também faz a leitura de .parquet para tabela do sql server
 Author: Marcus Holanda
 Author-email: mvsh777@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Programming Language :: PL/SQL
@@ -83,8 +83,20 @@
 with write_parquet(
     DRIVER, 
     '##teste', 
     path='origem.parquet'
 ) as C:
 
     ...
+
+# AGORA é possivel importar um numero limite de linhas
+# e selecionar as colunas no arquivo parquet
+with write_parquet(
+    DRIVER, 
+    '##teste', 
+    path='origem.parquet',
+    limit=100,
+    columns=['col1', 'col2']
+) as C:
+
+    ...
 ```
```

