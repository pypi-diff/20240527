# Comparing `tmp/generate_temp_table_sql-0.2.tar.gz` & `tmp/generate_temp_table_sql-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate_temp_table_sql-0.2.tar", last modified: Sun May 26 16:40:56 2024, max compression
+gzip compressed data, was "generate_temp_table_sql-0.3.tar", last modified: Mon May 27 16:51:46 2024, max compression
```

## Comparing `generate_temp_table_sql-0.2.tar` & `generate_temp_table_sql-0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-26 16:40:56.814706 generate_temp_table_sql-0.2/
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     1068 2024-05-26 15:44:57.000000 generate_temp_table_sql-0.2/LICENSE.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       37 2024-05-26 15:46:01.000000 generate_temp_table_sql-0.2/MANIFEST.in
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     3202 2024-05-26 16:40:56.814611 generate_temp_table_sql-0.2/PKG-INFO
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2680 2024-05-26 15:31:53.000000 generate_temp_table_sql-0.2/README.md
-drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-26 16:40:56.813712 generate_temp_table_sql-0.2/generate_temp_table_sql/
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)        0 2024-05-25 15:54:27.000000 generate_temp_table_sql-0.2/generate_temp_table_sql/__init__.py
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     1930 2024-05-26 15:27:09.000000 generate_temp_table_sql-0.2/generate_temp_table_sql/cli.py
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     3032 2024-05-26 16:37:11.000000 generate_temp_table_sql-0.2/generate_temp_table_sql/sql_generator.py
-drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-26 16:40:56.814284 generate_temp_table_sql-0.2/generate_temp_table_sql.egg-info/
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     3202 2024-05-26 16:40:56.000000 generate_temp_table_sql-0.2/generate_temp_table_sql.egg-info/PKG-INFO
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)      480 2024-05-26 16:40:56.000000 generate_temp_table_sql-0.2/generate_temp_table_sql.egg-info/SOURCES.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)        1 2024-05-26 16:40:56.000000 generate_temp_table_sql-0.2/generate_temp_table_sql.egg-info/dependency_links.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       70 2024-05-26 16:40:56.000000 generate_temp_table_sql-0.2/generate_temp_table_sql.egg-info/entry_points.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)        7 2024-05-26 16:40:56.000000 generate_temp_table_sql-0.2/generate_temp_table_sql.egg-info/requires.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       30 2024-05-26 16:40:56.000000 generate_temp_table_sql-0.2/generate_temp_table_sql.egg-info/top_level.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       38 2024-05-26 16:40:56.814744 generate_temp_table_sql-0.2/setup.cfg
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)      818 2024-05-26 16:39:52.000000 generate_temp_table_sql-0.2/setup.py
-drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-26 16:40:56.814456 generate_temp_table_sql-0.2/tests/
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)        0 2024-05-25 16:57:00.000000 generate_temp_table_sql-0.2/tests/__init__.py
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2151 2024-05-26 15:03:16.000000 generate_temp_table_sql-0.2/tests/test_sql_generator.py
+drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-27 16:51:46.673646 generate_temp_table_sql-0.3/
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     1068 2024-05-26 15:44:57.000000 generate_temp_table_sql-0.3/LICENSE.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       37 2024-05-26 15:46:01.000000 generate_temp_table_sql-0.3/MANIFEST.in
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     3205 2024-05-27 16:51:46.673502 generate_temp_table_sql-0.3/PKG-INFO
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2683 2024-05-27 13:31:42.000000 generate_temp_table_sql-0.3/README.md
+drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-27 16:51:46.672503 generate_temp_table_sql-0.3/generate_temp_table_sql/
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)        0 2024-05-25 15:54:27.000000 generate_temp_table_sql-0.3/generate_temp_table_sql/__init__.py
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2127 2024-05-27 16:33:51.000000 generate_temp_table_sql-0.3/generate_temp_table_sql/cli.py
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       88 2024-05-27 13:29:03.000000 generate_temp_table_sql-0.3/generate_temp_table_sql/constants.py
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2559 2024-05-27 16:41:04.000000 generate_temp_table_sql-0.3/generate_temp_table_sql/sql_generator.py
+drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-27 16:51:46.673127 generate_temp_table_sql-0.3/generate_temp_table_sql.egg-info/
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     3205 2024-05-27 16:51:46.000000 generate_temp_table_sql-0.3/generate_temp_table_sql.egg-info/PKG-INFO
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)      517 2024-05-27 16:51:46.000000 generate_temp_table_sql-0.3/generate_temp_table_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)        1 2024-05-27 16:51:46.000000 generate_temp_table_sql-0.3/generate_temp_table_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       70 2024-05-27 16:51:46.000000 generate_temp_table_sql-0.3/generate_temp_table_sql.egg-info/entry_points.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)        7 2024-05-27 16:51:46.000000 generate_temp_table_sql-0.3/generate_temp_table_sql.egg-info/requires.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       30 2024-05-27 16:51:46.000000 generate_temp_table_sql-0.3/generate_temp_table_sql.egg-info/top_level.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       38 2024-05-27 16:51:46.673686 generate_temp_table_sql-0.3/setup.cfg
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)      818 2024-05-27 16:49:13.000000 generate_temp_table_sql-0.3/setup.py
+drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-27 16:51:46.673347 generate_temp_table_sql-0.3/tests/
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)        0 2024-05-25 16:57:00.000000 generate_temp_table_sql-0.3/tests/__init__.py
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     5435 2024-05-27 16:45:56.000000 generate_temp_table_sql-0.3/tests/test_sql_generator.py
```

### Comparing `generate_temp_table_sql-0.2/LICENSE.txt` & `generate_temp_table_sql-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `generate_temp_table_sql-0.2/PKG-INFO` & `generate_temp_table_sql-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate_temp_table_sql
-Version: 0.2
+Version: 0.3
 Summary: A package to generate SQL statements from CSV files
 Home-page: https://github.com/yourusername/generate_temp_table_sql
 Author: Ryan Waldorf
 Author-email: ryan@ryanwaldorf.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -51,15 +51,15 @@
 
 After installing the package, you can use the `generate-tt-sql` command to generate SQL statements from a CSV file.
 
 #### Basic Usage
 
 To generate SQL statements and save them to a file:
 ```sh
-generate-sql path/to/your/file.csv
+generate-tt-sql path/to/your/file.csv
 ```
 
 #### Additional Options
 ```sh
 
 --o The path to the output SQL file.  Defaults to the director you call the command in.
 --overwrite: Allow overwriting the output file if it exists.
```

### Comparing `generate_temp_table_sql-0.2/README.md` & `generate_temp_table_sql-0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 After installing the package, you can use the `generate-tt-sql` command to generate SQL statements from a CSV file.
 
 #### Basic Usage
 
 To generate SQL statements and save them to a file:
 ```sh
-generate-sql path/to/your/file.csv
+generate-tt-sql path/to/your/file.csv
 ```
 
 #### Additional Options
 ```sh
 
 --o The path to the output SQL file.  Defaults to the director you call the command in.
 --overwrite: Allow overwriting the output file if it exists.
```

### Comparing `generate_temp_table_sql-0.2/generate_temp_table_sql/cli.py` & `generate_temp_table_sql-0.3/generate_temp_table_sql/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import argparse
 import os
 from generate_temp_table_sql.sql_generator import SQLGenerator
 
 def main():
     parser = argparse.ArgumentParser(description='Process a CSV file to generate SQL statements.')
     parser.add_argument('csv_file', type=str, help='The path to the CSV file')
-    parser.add_argument('-o', '--output_file', type=str, help='The path to the output SQL file.  Defaults to the director you call the command in.', default=None)
+    parser.add_argument('-o', '--output_file', type=str, help='The path to the output SQL file.  Defaults to the director you call the command in.')
     parser.add_argument('--overwrite', action='store_true', help='Allow overwriting the output file if it exists')
     parser.add_argument('--table_name', type=str, help='The name of the temp table you will create')
     parser.add_argument('--column_type', type=str, help='The data type of the columns in the temp table.  Defaults to TEXT which works for Redshift and Snowflake.  BigQuery requires STRING.')
+    parser.add_argument('--batch_size', type=int, help='The number of rows inserted per insert statement.  If present, it creates multiple insert statements based on the batch size specified.')
 
     args = parser.parse_args()
     
     # Use specified output file name or generate a default one
     if args.output_file is None:
         base_name = os.path.splitext(os.path.basename(args.csv_file))[0]
         args.output_file = os.path.join(os.getcwd(), base_name + '_temp_table.sql')
@@ -22,15 +23,15 @@
         print(f"Error: The file '{args.output_file}' already exists. Use --overwrite to allow overwriting.")
         return
 
     sql_generator = SQLGenerator(args.csv_file)
     
     sql_generator.load_csv()
     
-    create_table_sql, insert_data_sql = sql_generator.generate_sql(args.table_name, args.column_type)
+    create_table_sql, insert_data_sql = sql_generator.generate_sql(args.table_name, args.column_type, args.batch_size)
     
     with open(args.output_file, 'w') as f:
         f.write("--Create Table SQL:\n")
         f.write(create_table_sql + "\n\n")
         f.write("--Insert Data SQL:\n")
         for query in insert_data_sql:
             f.write(query + "\n")
```

### Comparing `generate_temp_table_sql-0.2/generate_temp_table_sql/sql_generator.py` & `generate_temp_table_sql-0.3/generate_temp_table_sql/sql_generator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,66 @@
 import pandas as pd
-
+from .constants import Constants
 class SQLGenerator:
+
+    #defaults if not specified
+
+
     def __init__(self, csv_file_path):
         self.csv_file_path = csv_file_path
         self.dataframe = None
 
     def load_csv(self):
-        self.dataframe = pd.read_csv(self.csv_file_path)
+        # converts all values to string so processing can be done on the warehouse side
+        self.dataframe = pd.read_csv(self.csv_file_path, dtype=str)
 
-    def create_temp_table_sql(self, table_name='temp_table', column_type='TEXT'):
+    def create_temp_table_sql(self, table_name, column_type):
         if self.dataframe is None:
             raise ValueError("Dataframe is not loaded. Call load_csv() first.")
         
         columns = self.dataframe.columns
-        # Join columns with a newline and tab for better formatting
-        column_definitions = ",\n\t".join([f"{col.strip()} {column_type}" for col in columns])
+        column_definitions = ",\n\t".join([f"\"{col.strip()}\" {column_type}" for col in columns])
         
         create_table_query = (
             f"CREATE TEMP TABLE {table_name} (\n"
             f"\t{column_definitions}\n"
             ");"
         )
         return create_table_query.strip()
 
-    def insert_data_sql(self, table_name='temp_table'):
+    def insert_data_sql(self, table_name, batch_size):
         if self.dataframe is None:
             raise ValueError("Dataframe is not loaded. Call load_csv() first.")
         
         insert_statements = []
         counter = 1
-        total_rows = self.dataframe.shape[0]
+        overall_counter = 1
+        total_rows = self.dataframe.shape[0] 
+        if batch_size == None:
+            batch_size = total_rows
         for _, row in self.dataframe.iterrows():
             columns = ', '.join(self.dataframe.columns)
             values = ', '.join([f"'{str(value).strip()}'" if not pd.isna(value) else 'NULL' for value in row])
-            if counter == total_rows:
-                punctuation = ";"
-            else:
-                punctuation = ','
             if counter == 1:
-                insert_statement = f"INSERT INTO {table_name} ({columns}) VALUES \n\t({values}){punctuation}"
+                insert_clause = f"INSERT INTO {table_name} VALUES"
+                insert_statements.append(insert_clause)
+            # adds a semicolon for the end of the batch, comma otherwise
+            if counter == batch_size or overall_counter == total_rows:
+                insert_statement = f"\t({values});\n"
+                counter = 0
             else:
-                insert_statement = f"\t({values}){punctuation}"
+                insert_statement = f"\t({values}),"
             insert_statements.append(insert_statement)
             counter += 1
+            overall_counter += 1
         return insert_statements
 
-
-    # def insert_data_sql(self, table_name='temp_table'):
-    #     if self.dataframe is None:
-    #         raise ValueError("Dataframe is not loaded. Call load_csv() first.")
-        
-    #     insert_statements = []
-    #     counter = 1
-    #     total_rows = self.dataframe.shape[0]
-    #     for _, row in self.dataframe.iterrows():
-    #         # columns = ', '.join(self.dataframe.columns)
-    #         values = ', '.join([f"'{str(value)}'" for value in row])
-    #         if counter == total_rows:
-    #             punctuation = ";"
-    #         else:
-    #             punctuation = ','
-    #         if counter == 1:
-    #             insert_statement = f"INSERT INTO {table_name} VALUES\n\t({values}){punctuation}"
-    #         else:
-    #             insert_statement = f"\t({values}){punctuation}"
-    #         insert_statements.append(insert_statement)
-    #         counter = counter + 1
-    #     return insert_statements
-
-    def generate_sql(self, table_name='temp_table', column_type = 'TEXT'):
+    def generate_sql(self, table_name, column_type, rows):
         self.load_csv()
+        if table_name == None:
+            table_name = Constants.DEFAULT_TABLE_NAME
+        if column_type == None:
+            column_type = Constants.DEFAULT_COLUMN_TYPE
         create_table_sql = self.create_temp_table_sql(table_name, column_type)
-        insert_data_sql = self.insert_data_sql(table_name)
+        insert_data_sql = self.insert_data_sql(table_name, rows)
         return create_table_sql, insert_data_sql
```

### Comparing `generate_temp_table_sql-0.2/generate_temp_table_sql.egg-info/PKG-INFO` & `generate_temp_table_sql-0.3/generate_temp_table_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-temp-table-sql
-Version: 0.2
+Version: 0.3
 Summary: A package to generate SQL statements from CSV files
 Home-page: https://github.com/yourusername/generate_temp_table_sql
 Author: Ryan Waldorf
 Author-email: ryan@ryanwaldorf.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -51,15 +51,15 @@
 
 After installing the package, you can use the `generate-tt-sql` command to generate SQL statements from a CSV file.
 
 #### Basic Usage
 
 To generate SQL statements and save them to a file:
 ```sh
-generate-sql path/to/your/file.csv
+generate-tt-sql path/to/your/file.csv
 ```
 
 #### Additional Options
 ```sh
 
 --o The path to the output SQL file.  Defaults to the director you call the command in.
 --overwrite: Allow overwriting the output file if it exists.
```

### Comparing `generate_temp_table_sql-0.2/setup.py` & `generate_temp_table_sql-0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='generate_temp_table_sql',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         'pandas',
     ],
     entry_points={
         'console_scripts': [
             'generate-tt-sql=generate_temp_table_sql.cli:main',
```

