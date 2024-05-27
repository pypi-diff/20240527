# Comparing `tmp/rcplus_alloy_common-5.0.0.tar.gz` & `tmp/rcplus_alloy_common-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcplus_alloy_common-5.0.0.tar", max compression
+gzip compressed data, was "rcplus_alloy_common-5.1.0.tar", max compression
```

## Comparing `rcplus_alloy_common-5.0.0.tar` & `rcplus_alloy_common-5.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       77 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/LICENSE
--rw-r--r--   0        0        0      571 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/README.md
--rw-r--r--   0        0        0     3013 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     2668 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/__init__.py
--rw-r--r--   0        0        0     1072 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/__init__.py
--rw-r--r--   0        0        0     4256 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/dag.py
--rw-r--r--   0        0        0     2998 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/decorators.py
--rw-r--r--   0        0        0      703 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/hooks.py
--rw-r--r--   0        0        0     8258 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/locking.py
--rw-r--r--   0        0        0    11749 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/observability.py
--rw-r--r--   0        0        0    26534 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/operators.py
--rw-r--r--   0        0        0        0 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/py.typed
--rw-r--r--   0        0        0     2186 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/sensors.py
--rw-r--r--   0        0        0     5997 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/utils.py
--rw-r--r--   0        0        0       98 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/__init__.py
--rw-r--r--   0        0        0     4051 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/dynamodb.py
--rw-r--r--   0        0        0     2720 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/utils.py
--rw-r--r--   0        0        0    12430 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/wr.py
--rw-r--r--   0        0        0     2750 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/wr_utils.py
--rw-r--r--   0        0        0     2475 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/constants.py
--rw-r--r--   0        0        0      710 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/encoder.py
--rw-r--r--   0        0        0      616 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/__init__.py
--rw-r--r--   0        0        0     7223 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/audience.py
--rw-r--r--   0        0        0       80 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/constants.py
--rw-r--r--   0        0        0    10291 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/keyvalues.py
--rw-r--r--   0        0        0        0 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/mock/__init__.py
--rw-r--r--   0        0        0    18267 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/mock/services.py
--rw-r--r--   0        0        0     2170 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/network.py
--rw-r--r--   0        0        0        0 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/py.typed
--rw-r--r--   0        0        0      494 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/utils.py
--rw-r--r--   0        0        0     8397 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/logging.py
--rw-r--r--   0        0        0     6968 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/metrics.py
--rw-r--r--   0        0        0     1250 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/multitenancy.py
--rw-r--r--   0        0        0        0 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/py.typed
--rw-r--r--   0        0        0     3925 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/retry.py
--rw-r--r--   0        0        0       19 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/version.py
--rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 rcplus_alloy_common-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0       77 2024-05-27 15:15:15.527532 rcplus_alloy_common-5.1.0/LICENSE
+-rw-r--r--   0        0        0      571 2024-05-27 15:15:15.527532 rcplus_alloy_common-5.1.0/README.md
+-rw-r--r--   0        0        0     3013 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2668 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/__init__.py
+-rw-r--r--   0        0        0     1072 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/__init__.py
+-rw-r--r--   0        0        0     4256 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/dag.py
+-rw-r--r--   0        0        0     2998 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/decorators.py
+-rw-r--r--   0        0        0      703 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/hooks.py
+-rw-r--r--   0        0        0     8258 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/locking.py
+-rw-r--r--   0        0        0    11749 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/observability.py
+-rw-r--r--   0        0        0    26742 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/operators.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/py.typed
+-rw-r--r--   0        0        0     2186 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/sensors.py
+-rw-r--r--   0        0        0     5997 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/utils.py
+-rw-r--r--   0        0        0       98 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/aws/__init__.py
+-rw-r--r--   0        0        0     4051 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/aws/dynamodb.py
+-rw-r--r--   0        0        0     2720 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/aws/utils.py
+-rw-r--r--   0        0        0    14246 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/aws/wr.py
+-rw-r--r--   0        0        0     2839 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/aws/wr_utils.py
+-rw-r--r--   0        0        0     2475 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/constants.py
+-rw-r--r--   0        0        0      710 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/encoder.py
+-rw-r--r--   0        0        0      616 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/__init__.py
+-rw-r--r--   0        0        0     7223 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/audience.py
+-rw-r--r--   0        0        0       80 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/constants.py
+-rw-r--r--   0        0        0    10291 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/keyvalues.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/mock/__init__.py
+-rw-r--r--   0        0        0    18267 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/mock/services.py
+-rw-r--r--   0        0        0     2170 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/network.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/py.typed
+-rw-r--r--   0        0        0      494 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/utils.py
+-rw-r--r--   0        0        0     8397 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/logging.py
+-rw-r--r--   0        0        0     6968 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/metrics.py
+-rw-r--r--   0        0        0     1350 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/multitenancy.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/py.typed
+-rw-r--r--   0        0        0     3925 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/retry.py
+-rw-r--r--   0        0        0       19 2024-05-27 15:15:15.531532 rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/version.py
+-rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 rcplus_alloy_common-5.1.0/PKG-INFO
```

### Comparing `rcplus_alloy_common-5.0.0/README.md` & `rcplus_alloy_common-5.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v5.0.0**
+Current version: **v5.1.0**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

### Comparing `rcplus_alloy_common-5.0.0/pyproject.toml` & `rcplus_alloy_common-5.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 max-args = 11
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.poetry]
 name = "rcplus_alloy_common"
-version = "5.0.0"
+version = "5.1.0"
 description = "RC+/Alloy helpers functions for Python"
 readme = "README.md"
 authors = [
     "Ringier AG <info@rcplus.io>",
 ]
 license = "Proprietary"
 repository = "https://github.com/alloy-ch/rcplus-alloy-lib-py-common"
```

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/__init__.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/__init__.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/dag.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/decorators.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/decorators.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/hooks.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/hooks.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/locking.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/locking.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/observability.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/observability.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/operators.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
                             "command": command or [],
                         },
                     ],
                 }
             else:
                 overrides = {}
         elif environment_variables is not None or command is not None:
-                raise ValueError("Overrides are provided. Environment variables and command are not allowed.")
+            raise ValueError("Overrides are provided. Environment variables and command are not allowed.")
 
         super().__init__(
             task_definition=task_definition,
             cluster=cluster,
             overrides=overrides,
             reattach=reattach,
             **kwargs
@@ -268,14 +268,18 @@
                 raise AirflowException(f"No tenant config for {self.tenant}")
 
             primary_container["environment"] = [
                 *(primary_container["environment"] if primary_container.get("environment") is not None else []),
                 *[
                     {"name": "TENANT", "value": self.tenant},
                     {"name": "FEATURES", "value": json.dumps(vars(tenant_config.features))},
+                    {
+                        "name": "PREDICTIONS",
+                        "value": json.dumps([vars(prediction) for prediction in tenant_config.predictions])
+                    },
                     {"name": "WR_DATABASE", "value": self.tenant},
                 ]
             ]
 
     def execute(self, context, session=None):
         """
         Inject environment variables DAG_TASK_ID, DAG_RUN_ID, DAG_ID as logging context into both containers
@@ -589,15 +593,16 @@
             database=database,
             output_location=output_location,
             workgroup=workgroup,
             **kwargs,
         )
         self.query_timeout_ms = query_timeout_ms
 
-    def athena_query_execution(self, client, execution_id):
+    @staticmethod
+    def athena_query_execution(client, execution_id):
         return client.get_query_execution(QueryExecutionId=execution_id)
 
     def read_sql_query(self, query, client):
 
         # This will get ignored if workgroup enforces output location
         result_configuration = {"OutputLocation": f"{self.output_location}"}
         execution = client.start_query_execution(
```

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/sensors.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/sensors.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/utils.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/airflow/utils.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/dynamodb.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/utils.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/aws/utils.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/wr.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/aws/wr.py`

 * *Files 21% similar despite different names*

```diff
@@ -262,27 +262,25 @@
         glue_table_settings=glue_table_settings,
         partition_cols=partition_cols,
         dataset=dataset,
         **kwargs,
     )
 
 
-def create_parquet_table(
+def extract_table_creation_params(
     table: str,
     path: str,
-    database: str,
-    columns_types: dict[str, str] | None = None,
-    partitions_types: dict[str, str] | None = None,
-    description: str | None = None,
-    columns_comments: dict[str, str] | None = None,
-    schema_file_path: str | None = None,
-    skip_path_validation: bool = False,
-    **kwargs,
-) -> None:
-    """A wrapper for the awswrangler catalog create_parquet_table method to read schema."""
+    database: str | None,
+    columns_types: dict[str, str] | None,
+    partitions_types: dict[str, str] | None,
+    description: str | None,
+    columns_comments: dict[str, str] | None,
+    schema_file_path: str | None,
+    skip_path_validation: bool,
+) -> tuple[str, dict[str, str] | None, dict[str, str] | None, str | None, dict[str, str] | None]:
 
     database = database if database is not None else get_database()
     if database is None:
         raise ValueError("Database is not set")
 
     validate_table_input(
         schema_file_path=schema_file_path,
@@ -296,14 +294,43 @@
     if schema_file_path is not None:
         table_schema = read_table_from_yaml_schema(schema_file_path, table)
         columns_types = get_columns_with_types(table_schema, include_partition=False)
         partitions_types = get_partition_columns_with_type(table_schema)
         description = table_schema["description"]
         columns_comments = get_columns_with_comments(table_schema)
 
+    return database, columns_types, partitions_types, description, columns_comments
+
+
+def create_parquet_table(
+    table: str,
+    path: str,
+    database: str | None,
+    columns_types: dict[str, str] | None = None,
+    partitions_types: dict[str, str] | None = None,
+    description: str | None = None,
+    columns_comments: dict[str, str] | None = None,
+    schema_file_path: str | None = None,
+    skip_path_validation: bool = False,
+    **kwargs,
+) -> None:
+    """A wrapper for the awswrangler catalog create_parquet_table method to read schema."""
+
+    database, columns_types, partitions_types, description, columns_comments = extract_table_creation_params(
+        table=table,
+        path=path,
+        database=database,
+        columns_types=columns_types,
+        partitions_types=partitions_types,
+        description=description,
+        columns_comments=columns_comments,
+        schema_file_path=schema_file_path,
+        skip_path_validation=skip_path_validation,
+    )
+
     wr.catalog.create_parquet_table(
         database=database,
         table=table,
         path=path,
         columns_types=columns_types, # type: ignore[arg-type]
         partitions_types=partitions_types,
         description=description,
@@ -311,46 +338,76 @@
         **kwargs,
     )
 
 
 def create_json_table(
     table: str,
     path: str,
-    database: str,
+    database: str | None,
     columns_types: dict[str, str] | None = None,
     partitions_types: dict[str, str] | None = None,
     description: str | None = None,
     columns_comments: dict[str, str] | None = None,
     schema_file_path: str | None = None,
     skip_path_validation: bool = False,
     **kwargs,
 ) -> None:
     """A wrapper for the awswrangler catalog create_json_table method to read schema."""
 
-    database = database if database is not None else get_database()
-    if database is None:
-        raise ValueError("Database is not set")
-
-    validate_table_input(
-        schema_file_path=schema_file_path,
+    database, columns_types, partitions_types, description, columns_comments = extract_table_creation_params(
+        table=table,
+        path=path,
+        database=database,
         columns_types=columns_types,
         partitions_types=partitions_types,
+        description=description,
+        columns_comments=columns_comments,
+        schema_file_path=schema_file_path,
+        skip_path_validation=skip_path_validation,
     )
 
-    if not skip_path_validation:
-        validate_path(table, database, path)
+    wr.catalog.create_json_table(
+        database=database,
+        table=table,
+        path=path,
+        columns_types=columns_types, # type: ignore[arg-type]
+        partitions_types=partitions_types,
+        description=description,
+        columns_comments=columns_comments,
+        **kwargs,
+    )
 
-    if schema_file_path is not None:
-        table_schema = read_table_from_yaml_schema(schema_file_path, table)
-        columns_types = get_columns_with_types(table_schema, include_partition=False)
-        partitions_types = get_partition_columns_with_type(table_schema)
-        description = table_schema["description"]
-        columns_comments = get_columns_with_comments(table_schema)
 
-    wr.catalog.create_json_table(
+def create_csv_table(
+    table: str,
+    path: str,
+    database: str,
+    columns_types: dict[str, str] | None = None,
+    partitions_types: dict[str, str] | None = None,
+    description: str | None = None,
+    columns_comments: dict[str, str] | None = None,
+    schema_file_path: str | None = None,
+    skip_path_validation: bool = False,
+    **kwargs,
+) -> None:
+    """A wrapper for the awswrangler catalog create_csv_table method to read schema."""
+
+    database, columns_types, partitions_types, description, columns_comments = extract_table_creation_params(
+        table=table,
+        path=path,
+        database=database,
+        columns_types=columns_types,
+        partitions_types=partitions_types,
+        description=description,
+        columns_comments=columns_comments,
+        schema_file_path=schema_file_path,
+        skip_path_validation=skip_path_validation,
+    )
+
+    wr.catalog.create_csv_table(
         database=database,
         table=table,
         path=path,
         columns_types=columns_types, # type: ignore[arg-type]
         partitions_types=partitions_types,
         description=description,
         columns_comments=columns_comments,
```

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/wr_utils.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/aws/wr_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 import yaml
 
-def read_table_from_yaml_schema(file_path, table_name):
+def read_table_from_yaml_schema(file_path, table_name) -> dict:
     """Reads the YAML schema file and returns tables configuration."""
     with open(file_path, "r") as file:
         schema = yaml.safe_load(file)
         # Assume unique table names within a schema file
         for source in schema["sources"]:
             for table in source["tables"]:
                 if table["name"] == table_name:
                     return table
 
     raise KeyError(f"{table_name} not found from {file_path}")
 
 
-def get_partition_columns_with_type(schema):
+def get_partition_columns_with_type(schema: dict) -> dict:
     """Returns dict of partition columns with their types."""
     return {
         col["name"]: col["type"] for col in schema.get("external", {}).get("partitions", [])
     }
 
 
-def get_partition_columns_list(schema):
+def get_partition_columns_list(schema: dict) -> list[str]:
     """Returns list of partition columns."""
     return list(get_partition_columns_with_type(schema))
 
 
-def get_columns_with_types(schema, include_partition = True):
+def get_columns_with_types(schema: dict, include_partition: bool = True ) -> dict:
     """
     Returns dict of columns with their types.
     include_partitions defines whether partitioned columns are included or not.
     """
     partition_columns = get_partition_columns_with_type(schema) if include_partition else {}
     return {
         col["name"]: col["type"]
         for col in schema["columns"]
     } | partition_columns
 
 
-def get_columns_with_comments(schema):
+def get_columns_with_comments(schema: dict) -> dict:
     """Returns dict of all columns with their comments"""
     partition_columns = {
         col["name"]: col["description"]
         for col in schema.get("external", {}).get("partitions", [])
     }
     return {
         col["name"]: col["description"]
         for col in schema["columns"]
     } | partition_columns
 
 
-def get_sql_columns_with_comments(schema):
+def get_sql_columns_with_comments(schema: dict) -> str:
     """Returns string of all columns with type and comments"""
     columns = []
     for col in schema["columns"]:
         name = str(col["name"]).strip()
         type = str(col["type"]).strip()
         description = str(col["description"])
         if " " in name or "'" in description:
```

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/constants.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/constants.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/encoder.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/encoder.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/exceptions.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/audience.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/audience.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/keyvalues.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/keyvalues.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/mock/services.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/mock/services.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/network.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/gam/network.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/logging.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/logging.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/metrics.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/metrics.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/multitenancy.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/multitenancy.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,14 +21,19 @@
     sso_data: bool = False
     enterprise: bool = False
     dcr: bool = False
     byok: bool = False
     gotom: bool = False
 
 
+class Prediction(BaseModel):
+    name: str
+    params_path: str
+
+
 class Taxonomies(BaseModel):
     name: str
     score: float
 
 
 class CanonicalIdExtraction(BaseModel):
     uri_prefix: str
@@ -46,14 +51,15 @@
     is_uri_extracted_id_external_id: bool | None = None
 
 
 class TenantConfig(BaseModel):
     name: str
     activation_channels: ActivationChannels
     features: Features
+    predictions: List[Prediction]
     kropka_tenants: List[str]
     content_providers: List[ContentProvider]
 
 
 def get_json_schema():
     adapter = TypeAdapter(List[TenantConfig])
     return adapter.json_schema()
```

### Comparing `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/retry.py` & `rcplus_alloy_common-5.1.0/src/rcplus_alloy_common/retry.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-5.0.0/PKG-INFO` & `rcplus_alloy_common-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcplus_alloy_common
-Version: 5.0.0
+Version: 5.1.0
 Summary: RC+/Alloy helpers functions for Python
 Home-page: https://github.com/alloy-ch/rcplus-alloy-lib-py-common
 License: Proprietary
 Keywords: rcplus,alloy,logging,metrics,utilities
 Author: Ringier AG
 Author-email: info@rcplus.io
 Requires-Python: >=3.10,<4
@@ -37,15 +37,15 @@
 
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v5.0.0**
+Current version: **v5.1.0**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

