# Comparing `tmp/ng_data_pipelines_sdk-1.6.0.tar.gz` & `tmp/ng_data_pipelines_sdk-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-1.6.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-1.7.0.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-1.6.0.tar` & `ng_data_pipelines_sdk-1.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-05-24 18:39:01.538544 ng_data_pipelines_sdk-1.6.0/README.md
--rw-r--r--   0        0        0        0 2024-05-24 18:39:01.575544 ng_data_pipelines_sdk-1.6.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-05-24 18:39:01.539544 ng_data_pipelines_sdk-1.6.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-05-24 18:39:01.539544 ng_data_pipelines_sdk-1.6.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    28057 2024-05-24 18:39:01.539544 ng_data_pipelines_sdk-1.6.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    22114 2024-05-24 18:39:01.539544 ng_data_pipelines_sdk-1.6.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     5406 2024-05-24 18:39:01.539544 ng_data_pipelines_sdk-1.6.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     4780 2024-05-24 18:39:01.539544 ng_data_pipelines_sdk-1.6.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      838 2024-05-24 18:39:01.542544 ng_data_pipelines_sdk-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-27 11:32:06.829753 ng_data_pipelines_sdk-1.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 11:32:06.863753 ng_data_pipelines_sdk-1.7.0/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-05-27 11:32:06.829753 ng_data_pipelines_sdk-1.7.0/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-05-27 11:32:06.829753 ng_data_pipelines_sdk-1.7.0/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    28029 2024-05-27 11:32:06.830754 ng_data_pipelines_sdk-1.7.0/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    22122 2024-05-27 11:32:06.830754 ng_data_pipelines_sdk-1.7.0/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5406 2024-05-27 11:32:06.830754 ng_data_pipelines_sdk-1.7.0/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     4780 2024-05-27 11:32:06.830754 ng_data_pipelines_sdk-1.7.0/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      838 2024-05-27 11:32:06.833753 ng_data_pipelines_sdk-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.7.0/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-1.6.0/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-1.7.0/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.6.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-1.7.0/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                 dates=input_df_params.read_date_params.read_dates,
                 year_partition=date_partitions.get(DatePartition.YEAR, "year"),
                 month_partition=date_partitions.get(DatePartition.MONTH, "month"),
                 day_partition=date_partitions.get(DatePartition.DAY, "day"),
             )
 
             # Prevent pyspark from adding date columns to the DataFrame
-            if not input_df_params.read_date_params.add_all_date_columns:
+            if input_df_params.read_date_params.do_not_include_date_columns:
                 full_base_path = None
         else:
             paths = f"{bucket_url}/{input_df_params.dataframe_base_path}"
 
         if input_df_params.pyspark_schema_struct:
             schema = self.convert_schema_object_to_pyspark_schema(
                 schema_object=input_df_params.pyspark_schema_struct
@@ -312,14 +312,20 @@
         Returns:
             None
         """
         bucket_url = self._get_bucket_url(output_df_params.dataframe_bucket_params)
         write_base_path_url = f"{bucket_url}/{output_df_params.dataframe_base_path}"
         logger.debug(f"Write base path: {write_base_path_url}")
 
+        write_info =  f"Writing DataFrame to base path {write_base_path_url}"
+        if output_df_params.partition_by:
+            write_info += f" with partitions {output_df_params.partition_by}"
+        else:
+            write_info += " without partitions"
+
         df_to_write = df
         if output_df_params.single_write_date_params:
             date_partition_path = ""
             for (
                 date_partition,
                 date_partition_name,
             ) in (
@@ -332,14 +338,16 @@
                 df_to_write = df_to_write.withColumn(
                     date_partition_name, lit(formatted_date_part_value)
                 )
                 date_partition_path += (
                     f"{date_partition_name}={formatted_date_part_value}/"
                 )
 
+            write_info += f". Single write date is being used, so all data will be written to a single path: {write_base_path_url}/{date_partition_path}"
+
             if output_df_params.overwrite:
                 full_path = f"{write_base_path_url}/{date_partition_path}"
                 logger.info(
                     f"Overwrite is set to True. Deleting existing objects under path {full_path}"
                 )
                 try:
                     self.aws_interface.delete_objects_aws(
@@ -348,23 +356,15 @@
                         path=f"{output_df_params.dataframe_base_path}/{date_partition_path}",
                     )
                 except Exception as e:
                     raise ValueError(f"Error deleting dataframe objects: {e}")
 
                 logger.info("Objects deleted successfully.")
 
-        info =  f"Writing DataFrame to base path {write_base_path_url}"
-        if output_df_params.partition_by:
-            info += f" with partitions {output_df_params.partition_by}"
-            if output_df_params.single_write_date_params:
-                info += f". Single write date is being used, so all data will be written to a single path: {write_base_path_url}/{date_partition_path}"
-        else:
-            info += " without partitions"
-
-        logger.info(info)
+        logger.info(write_info)
 
         self.spark_manager.write(
             env=output_df_params.dataframe_bucket_params.env,
             df=df_to_write,
             path=write_base_path_url,
             file_type=output_df_params.dataframe_file_type,
             partitions=output_df_params.partition_by,
```

### Comparing `ng_data_pipelines_sdk-1.6.0/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-1.7.0/ng_data_pipelines_sdk/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
     processing_date_offset_days: Optional[int] = None
     was_offset_applied: bool = False
     date_partitions: dict[DatePartition, str] = {
         DatePartition.YEAR: "year",
         DatePartition.MONTH: "month",
         DatePartition.DAY: "day",
     }
-    add_all_date_columns: bool = True
+    do_not_include_date_columns: bool = False
 
     @model_validator(mode="before")
     def validate_offset_and_read_dates(cls, data):
         read_dates = data.get("read_dates")
         processing_date_offset_days = data.get("processing_date_offset_days")
 
         if processing_date_offset_days is not None:
```

### Comparing `ng_data_pipelines_sdk-1.6.0/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-1.7.0/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.6.0/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-1.7.0/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.6.0/pyproject.toml` & `ng_data_pipelines_sdk-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "1.6.0"
+version = "1.7.0"
 description = "A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-1.6.0/PKG-INFO` & `ng_data_pipelines_sdk-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 1.6.0
+Version: 1.7.0
 Summary: A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

