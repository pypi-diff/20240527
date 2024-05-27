# Comparing `tmp/data_ingestion_lib-1.0.2.tar.gz` & `tmp/data_ingestion_lib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ingestion_lib-1.0.2.tar", max compression
+gzip compressed data, was "data_ingestion_lib-1.0.3.tar", max compression
```

## Comparing `data_ingestion_lib-1.0.2.tar` & `data_ingestion_lib-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0        0 2024-05-22 08:36:12.337511 data_ingestion_lib-1.0.2/data_ingestion/aws_services/__init__.py
--rw-r--r--   0        0        0      781 2024-05-22 08:36:12.338115 data_ingestion_lib-1.0.2/data_ingestion/aws_services/eventbridge_service.py
--rw-r--r--   0        0        0     1088 2024-05-22 08:36:12.338469 data_ingestion_lib-1.0.2/data_ingestion/aws_services/s3_service.py
--rw-r--r--   0        0        0     1900 2024-05-22 08:36:12.338806 data_ingestion_lib-1.0.2/data_ingestion/aws_services/scheduler_service.py
--rw-r--r--   0        0        0        0 2024-05-22 08:36:12.338915 data_ingestion_lib-1.0.2/data_ingestion/crud/__init__.py
--rw-r--r--   0        0        0     4036 2024-05-22 08:36:12.339430 data_ingestion_lib-1.0.2/data_ingestion/crud/data_ingestion_metadata_table/DataIngestionConfig.py
--rw-r--r--   0        0        0     4061 2024-05-22 08:36:12.339790 data_ingestion_lib-1.0.2/data_ingestion/crud/data_ingestion_metadata_table/ExportStatus.py
--rw-r--r--   0        0        0        0 2024-05-22 08:36:12.339882 data_ingestion_lib-1.0.2/data_ingestion/crud/data_ingestion_metadata_table/__init__.py
--rw-r--r--   0        0        0     1627 2024-05-22 08:36:12.340374 data_ingestion_lib-1.0.2/data_ingestion/database/SetupDB.py
--rw-r--r--   0        0        0        0 2024-05-22 08:36:12.340461 data_ingestion_lib-1.0.2/data_ingestion/database/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 08:36:12.340726 data_ingestion_lib-1.0.2/data_ingestion/model/__init__.py
--rw-r--r--   0        0        0     1798 2024-05-22 08:36:12.341214 data_ingestion_lib-1.0.2/data_ingestion/model/data_ingestion_metadata_table/DataIngestionConfig.py
--rw-r--r--   0        0        0     3511 2024-05-22 08:36:12.341549 data_ingestion_lib-1.0.2/data_ingestion/model/data_ingestion_metadata_table/ExportStatus.py
--rw-r--r--   0        0        0        0 2024-05-22 08:36:12.341636 data_ingestion_lib-1.0.2/data_ingestion/model/data_ingestion_metadata_table/__init__.py
--rw-r--r--   0        0        0      816 2024-05-22 08:36:12.342104 data_ingestion_lib-1.0.2/data_ingestion/settings.py
--rw-r--r--   0        0        0        0 2024-05-22 08:36:12.342211 data_ingestion_lib-1.0.2/data_ingestion/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 08:36:12.342475 data_ingestion_lib-1.0.2/data_ingestion/tests/aws_services/__init__.py
--rw-r--r--   0        0        0     2126 2024-05-22 08:36:12.342968 data_ingestion_lib-1.0.2/data_ingestion/tests/aws_services/test_s3_service.py
--rw-r--r--   0        0        0     2048 2024-05-22 08:36:12.343292 data_ingestion_lib-1.0.2/data_ingestion/tests/aws_services/test_scheduler_service.py
--rw-r--r--   0        0        0     4456 2024-05-22 08:36:12.343642 data_ingestion_lib-1.0.2/data_ingestion/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-05-22 08:36:12.343771 data_ingestion_lib-1.0.2/data_ingestion/tests/crud/__init__.py
--rw-r--r--   0        0        0     2965 2024-05-22 08:36:12.344603 data_ingestion_lib-1.0.2/data_ingestion/tests/crud/test_data_ingestion_metadata_table.py
--rw-r--r--   0        0        0     2357 2024-05-22 08:36:12.345085 data_ingestion_lib-1.0.2/data_ingestion/tests/crud/test_export_status.py
--rw-r--r--   0        0        0        0 2024-05-22 08:36:12.345253 data_ingestion_lib-1.0.2/data_ingestion/tests/utils/__init__.py
--rw-r--r--   0        0        0     1535 2024-05-22 08:36:12.346753 data_ingestion_lib-1.0.2/data_ingestion/tests/utils/test_data_ingestion_utils.py
--rw-r--r--   0        0        0        0 2024-05-22 08:36:12.346960 data_ingestion_lib-1.0.2/data_ingestion/utils/__init__.py
--rw-r--r--   0        0        0      261 2024-05-22 08:36:12.347768 data_ingestion_lib-1.0.2/data_ingestion/utils/aws_session.py
--rw-r--r--   0        0        0      544 2024-05-22 08:36:12.348347 data_ingestion_lib-1.0.2/data_ingestion/utils/common.py
--rw-r--r--   0        0        0      484 2024-05-22 08:36:12.348937 data_ingestion_lib-1.0.2/data_ingestion/utils/datetime_util.py
--rw-r--r--   0        0        0      440 2024-05-22 08:36:12.349454 data_ingestion_lib-1.0.2/data_ingestion/utils/dynamodb_client.py
--rw-r--r--   0        0        0      235 2024-05-22 08:36:12.349969 data_ingestion_lib-1.0.2/data_ingestion/utils/eventbridge_client.py
--rw-r--r--   0        0        0       43 2024-05-22 08:36:12.350473 data_ingestion_lib-1.0.2/data_ingestion/utils/exception.py
--rw-r--r--   0        0        0     1726 2024-05-22 08:36:12.351000 data_ingestion_lib-1.0.2/data_ingestion/utils/logger.py
--rw-r--r--   0        0        0      404 2024-05-22 08:36:12.351503 data_ingestion_lib-1.0.2/data_ingestion/utils/s3_client.py
--rw-r--r--   0        0        0      239 2024-05-22 08:36:12.352026 data_ingestion_lib-1.0.2/data_ingestion/utils/scheduler_client.py
--rw-r--r--   0        0        0      221 2024-05-22 08:36:12.352543 data_ingestion_lib-1.0.2/data_ingestion/utils/sqs_client.py
--rw-r--r--   0        0        0      457 2024-05-22 08:36:12.353085 data_ingestion_lib-1.0.2/data_ingestion/utils/step_function_client.py
--rw-r--r--   0        0        0      361 2024-05-23 06:43:32.165645 data_ingestion_lib-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 data_ingestion_lib-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.337511 data_ingestion_lib-1.0.3/data_ingestion/aws_services/__init__.py
+-rw-r--r--   0        0        0      781 2024-05-22 08:36:12.338115 data_ingestion_lib-1.0.3/data_ingestion/aws_services/eventbridge_service.py
+-rw-r--r--   0        0        0     1088 2024-05-22 08:36:12.338469 data_ingestion_lib-1.0.3/data_ingestion/aws_services/s3_service.py
+-rw-r--r--   0        0        0     1900 2024-05-22 08:36:12.338806 data_ingestion_lib-1.0.3/data_ingestion/aws_services/scheduler_service.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.338915 data_ingestion_lib-1.0.3/data_ingestion/crud/__init__.py
+-rw-r--r--   0        0        0     3372 2024-05-27 02:07:41.497611 data_ingestion_lib-1.0.3/data_ingestion/crud/data_ingestion_metadata_table/DataIngestionConfig.py
+-rw-r--r--   0        0        0     4061 2024-05-22 08:36:12.339790 data_ingestion_lib-1.0.3/data_ingestion/crud/data_ingestion_metadata_table/ExportStatus.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.339882 data_ingestion_lib-1.0.3/data_ingestion/crud/data_ingestion_metadata_table/__init__.py
+-rw-r--r--   0        0        0     1481 2024-05-27 02:30:51.664329 data_ingestion_lib-1.0.3/data_ingestion/database/SetupDB.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.340461 data_ingestion_lib-1.0.3/data_ingestion/database/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.340726 data_ingestion_lib-1.0.3/data_ingestion/model/__init__.py
+-rw-r--r--   0        0        0     1368 2024-05-27 02:13:39.190533 data_ingestion_lib-1.0.3/data_ingestion/model/data_ingestion_metadata_table/DataIngestionConfig.py
+-rw-r--r--   0        0        0     3511 2024-05-22 08:36:12.341549 data_ingestion_lib-1.0.3/data_ingestion/model/data_ingestion_metadata_table/ExportStatus.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.341636 data_ingestion_lib-1.0.3/data_ingestion/model/data_ingestion_metadata_table/__init__.py
+-rw-r--r--   0        0        0      816 2024-05-22 08:36:12.342104 data_ingestion_lib-1.0.3/data_ingestion/settings.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.342211 data_ingestion_lib-1.0.3/data_ingestion/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.342475 data_ingestion_lib-1.0.3/data_ingestion/tests/aws_services/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-24 02:30:24.194563 data_ingestion_lib-1.0.3/data_ingestion/tests/aws_services/test_s3_service.py
+-rw-r--r--   0        0        0     2143 2024-05-27 02:24:03.207045 data_ingestion_lib-1.0.3/data_ingestion/tests/aws_services/test_scheduler_service.py
+-rw-r--r--   0        0        0     4416 2024-05-27 02:30:42.196750 data_ingestion_lib-1.0.3/data_ingestion/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.343771 data_ingestion_lib-1.0.3/data_ingestion/tests/crud/__init__.py
+-rw-r--r--   0        0        0     3137 2024-05-27 02:22:39.640576 data_ingestion_lib-1.0.3/data_ingestion/tests/crud/test_data_ingestion_metadata_table.py
+-rw-r--r--   0        0        0     2357 2024-05-22 08:36:12.345085 data_ingestion_lib-1.0.3/data_ingestion/tests/crud/test_export_status.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.345253 data_ingestion_lib-1.0.3/data_ingestion/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1535 2024-05-22 08:36:12.346753 data_ingestion_lib-1.0.3/data_ingestion/tests/utils/test_data_ingestion_utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.346960 data_ingestion_lib-1.0.3/data_ingestion/utils/__init__.py
+-rw-r--r--   0        0        0      261 2024-05-22 08:36:12.347768 data_ingestion_lib-1.0.3/data_ingestion/utils/aws_session.py
+-rw-r--r--   0        0        0      544 2024-05-22 08:36:12.348347 data_ingestion_lib-1.0.3/data_ingestion/utils/common.py
+-rw-r--r--   0        0        0      484 2024-05-22 08:36:12.348937 data_ingestion_lib-1.0.3/data_ingestion/utils/datetime_util.py
+-rw-r--r--   0        0        0      440 2024-05-22 08:36:12.349454 data_ingestion_lib-1.0.3/data_ingestion/utils/dynamodb_client.py
+-rw-r--r--   0        0        0      235 2024-05-22 08:36:12.349969 data_ingestion_lib-1.0.3/data_ingestion/utils/eventbridge_client.py
+-rw-r--r--   0        0        0       43 2024-05-22 08:36:12.350473 data_ingestion_lib-1.0.3/data_ingestion/utils/exception.py
+-rw-r--r--   0        0        0     1726 2024-05-22 08:36:12.351000 data_ingestion_lib-1.0.3/data_ingestion/utils/logger.py
+-rw-r--r--   0        0        0      404 2024-05-22 08:36:12.351503 data_ingestion_lib-1.0.3/data_ingestion/utils/s3_client.py
+-rw-r--r--   0        0        0      239 2024-05-22 08:36:12.352026 data_ingestion_lib-1.0.3/data_ingestion/utils/scheduler_client.py
+-rw-r--r--   0        0        0      221 2024-05-22 08:36:12.352543 data_ingestion_lib-1.0.3/data_ingestion/utils/sqs_client.py
+-rw-r--r--   0        0        0      457 2024-05-22 08:36:12.353085 data_ingestion_lib-1.0.3/data_ingestion/utils/step_function_client.py
+-rw-r--r--   0        0        0      314 2024-05-27 04:18:21.917672 data_ingestion_lib-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 data_ingestion_lib-1.0.3/PKG-INFO
```

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/aws_services/eventbridge_service.py` & `data_ingestion_lib-1.0.3/data_ingestion/aws_services/eventbridge_service.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/aws_services/s3_service.py` & `data_ingestion_lib-1.0.3/data_ingestion/aws_services/s3_service.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/aws_services/scheduler_service.py` & `data_ingestion_lib-1.0.3/data_ingestion/aws_services/scheduler_service.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/crud/data_ingestion_metadata_table/DataIngestionConfig.py` & `data_ingestion_lib-1.0.3/data_ingestion/crud/data_ingestion_metadata_table/DataIngestionConfig.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,58 +11,24 @@
 )
 from data_ingestion.utils.common import DATA_INGESTION_METADATA_TABLE
 from data_ingestion.utils.logger import configure_logging
 
 logger = configure_logging()
 
 
-def get_latest_config(table: str, dynamodb_client: DynamoDBClient):
+def get_config_by_pk(pk: str, dynamodb_client: DynamoDBClient):
+    """
+    Get data ingestion configuration from DynamoDB
+    """
     try:
         response = dynamodb_client.query(
             TableName=DATA_INGESTION_METADATA_TABLE,
             KeyConditionExpression="PK = :PK",
             ExpressionAttributeValues={
-                ":PK": {"S": f"TABLE_CONFIG#{table}"},
-            },
-            FilterExpression="attribute_not_exists(latest_timestamp)",
-            ScanIndexForward=False,
-            Limit=2,
-        )
-        item = response.get("Items")
-        if item:
-            return config_from_dynamodb_item(item[0])
-        return None
-    except Exception as ex:
-        logger.exception(ex)
-        raise ex
-
-
-def remove_is_active(item: DataIngestionConfig, dynamodb_client: DynamoDBClient):
-    try:
-        response = dynamodb_client.update_item(
-            TableName=DATA_INGESTION_METADATA_TABLE,
-            Key=item.primary_key(),
-            UpdateExpression="REMOVE is_active",
-            ConditionExpression="attribute_exists(is_active)",
-        )
-        return response["ResponseMetadata"]["HTTPStatusCode"]
-    except Exception as ex:
-        logger.exception(ex)
-        raise ex
-
-
-def get_active_config(domain: str, dynamodb_client: DynamoDBClient):
-    try:
-        response = dynamodb_client.query(
-            TableName=DATA_INGESTION_METADATA_TABLE,
-            IndexName="IsActiveIndex",
-            KeyConditionExpression="domain_file = :domain AND is_active = :active",
-            ExpressionAttributeValues={
-                ":domain": {"S": domain},
-                ":active": {"S": "true"},
+                ":PK": {"S": pk},
             },
         )
         items = response.get("Items")
         if items:
             return [config_from_dynamodb_item(item) for item in items]
         return []
     except Exception as ex:
@@ -74,46 +40,58 @@
     """
     Add data ingestion configuration item to DynamoDB
     """
     try:
         response = dynamodb_client.put_item(
             TableName=DATA_INGESTION_METADATA_TABLE,
             Item=item,
-            ConditionExpression="attribute_not_exists(SK)",
+            ConditionExpression="attribute_not_exists(config_timestamp) OR config_timestamp < :config_timestamp",
+            ExpressionAttributeValues={
+                ":config_timestamp": item["config_timestamp"],
+            },
         )
         return response["ResponseMetadata"]["HTTPStatusCode"]
     except ClientError as err:
         if err.response["Error"]["Code"] == "ConditionalCheckFailedException":
-            logger.info("add_config: the item already exists")
+            logger.info("add_config: timestamp is older than the current timestamp")
             return HTTPStatus.CONFLICT
         else:
             logger.exception(err)
             raise err
     except Exception as ex:
         logger.exception(ex)
         raise ex
 
 
-def add_latest_item(table: str, timestamp: str, dynamodb_client: DynamoDBClient):
+def update_config(item: DataIngestionConfig, dynamodb_client: DynamoDBClient):
+    """
+    Update data ingestion configuration item to DynamoDB
+    """
     try:
-        res = dynamodb_client.put_item(
+        response = dynamodb_client.update_item(
             TableName=DATA_INGESTION_METADATA_TABLE,
-            Item={
-                "PK": {
-                    "S": f"TABLE_CONFIG#{table}",
-                },
-                "SK": {"S": "CONFIGTIME#latest"},
-                "latest_timestamp": {"N": timestamp},
+            Key=item.primary_key(),
+            ExpressionAttributeNames={
+                "#C": "cron",
+                "#S": "status",
+                "#T": "config_timestamp",
             },
-            ConditionExpression="attribute_not_exists(latest_timestamp) OR latest_timestamp < :lt",
-            ExpressionAttributeValues={":lt": {"N": timestamp}},
+            ExpressionAttributeValues={
+                ":c": {"S": str(item.cron)},
+                ":s": {"S": item.status},
+                ":t": {"N": item.config_timestamp},
+                ":config_timestamp": {"N": item.config_timestamp},
+            },
+            UpdateExpression="SET #C = :c , #S = :s, #T = :t",
+            ConditionExpression="attribute_not_exists(config_timestamp) OR config_timestamp < :config_timestamp",
         )
-        return res["ResponseMetadata"]["HTTPStatusCode"]
-    except ClientError as ex:
-        if ex.response["Error"]["Code"] == "ConditionalCheckFailedException":
-            logger.info(
-                "add_latest_item: timestamp is older than the current timestamp"
-            )
+        return response["ResponseMetadata"]["HTTPStatusCode"]
+    except ClientError as err:
+        if err.response["Error"]["Code"] == "ConditionalCheckFailedException":
+            logger.info("update_config: timestamp is older than the current timestamp")
             return HTTPStatus.CONFLICT
         else:
-            logger.exception(ex)
-            raise ex
+            logger.exception(err)
+            raise err
+    except Exception as ex:
+        logger.exception(ex)
+        raise ex
```

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/crud/data_ingestion_metadata_table/ExportStatus.py` & `data_ingestion_lib-1.0.3/data_ingestion/crud/data_ingestion_metadata_table/ExportStatus.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/database/SetupDB.py` & `data_ingestion_lib-1.0.3/data_ingestion/database/SetupDB.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,27 +13,25 @@
             KeySchema=[
                 {"AttributeName": "PK", "KeyType": "HASH"},
                 {"AttributeName": "SK", "KeyType": "RANGE"},
             ],
             AttributeDefinitions=[
                 {"AttributeName": "PK", "AttributeType": "S"},
                 {"AttributeName": "SK", "AttributeType": "S"},
-                {"AttributeName": "is_active", "AttributeType": "S"},
                 {"AttributeName": "domain_file", "AttributeType": "S"},
             ],
             ProvisionedThroughput={
                 "ReadCapacityUnits": 5,
                 "WriteCapacityUnits": 5,
             },
             GlobalSecondaryIndexes=[
                 {
                     "IndexName": "IsActiveIndex",
                     "KeySchema": [
                         {"AttributeName": "domain_file", "KeyType": "HASH"},
-                        {"AttributeName": "is_active", "KeyType": "RANGE"},
                     ],
                     "Projection": {
                         "ProjectionType": "INCLUDE",
                         "NonKeyAttributes": ["PK", "SK"],
                     },
                 }
             ],
```

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/model/data_ingestion_metadata_table/DataIngestionConfig.py` & `data_ingestion_lib-1.0.3/data_ingestion/model/data_ingestion_metadata_table/DataIngestionConfig.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,47 @@
-from typing import Optional
-
-
 class DataIngestionConfig:
     def __init__(
         self,
         domain_name: str,
         table_name: str,
+        cron: str,
+        status: str,
         config_timestamp: str,
-        status: Optional[str],
-        cron: Optional[str],
-        is_active: Optional[str] = None,
     ):
         self.domain_name = domain_name
         self.table_name = table_name
         self.cron = cron
         self.status = status
         self.config_timestamp = config_timestamp
-        self.is_active = is_active
 
     def partition_key(self) -> dict:
-        return {"PK": {"S": f"TABLE_CONFIG#{self.table_name}"}}
+        return {"PK": {"S": f"CONFIG#{self.domain_name}"}}
 
     def sort_key(self) -> dict:
-        return {"SK": {"S": f"CONFIGTIME#{self.config_timestamp}"}}
+        return {"SK": {"S": f"TABLE#{self.table_name}"}}
 
     def primary_key(self) -> dict:
         return {**self.partition_key(), **self.sort_key()}
 
     def non_key_attributes(self) -> dict:
         return {
-            **({"cron": {"S": self.cron}} if self.cron is not None else {}),
-            **({"status": {"S": self.status}} if self.status is not None else {}),
-            "domain_file": {"S": self.domain_name},
-            **({"is_active": {"S": "true"}} if self.is_active is not None else {}),
+            "cron": {"S": self.cron},
+            "status": {"S": self.status},
+            "config_timestamp": {"N": self.config_timestamp},
         }
 
     def to_dynamodb_item(self) -> dict:
         return {
             **self.partition_key(),
             **self.sort_key(),
             **self.non_key_attributes(),
         }
 
 
 def config_from_dynamodb_item(item: dict) -> DataIngestionConfig:
     return DataIngestionConfig(
-        domain_name=item["domain_file"]["S"],
-        table_name=item["PK"]["S"].split("#")[1],
-        cron=(item["cron"]["S"] if "cron" in item else None),
-        status=(item["status"]["S"] if "status" in item else None),
-        config_timestamp=item["SK"]["S"].split("#")[1],
-        is_active=(item["is_active"]["S"] if "is_active" in item else None),
+        domain_name=item["PK"]["S"].split("#")[1],
+        table_name=item["SK"]["S"].split("#")[1],
+        cron=item["cron"]["S"],
+        status=item["status"]["S"],
+        config_timestamp=item["config_timestamp"]["N"],
     )
```

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/model/data_ingestion_metadata_table/ExportStatus.py` & `data_ingestion_lib-1.0.3/data_ingestion/model/data_ingestion_metadata_table/ExportStatus.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/settings.py` & `data_ingestion_lib-1.0.3/data_ingestion/settings.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/tests/aws_services/test_s3_service.py` & `data_ingestion_lib-1.0.3/data_ingestion/tests/aws_services/test_s3_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from data_ingestion.aws_services import s3_service
 
 import yaml
 import pytest
-from settings import DATA_INGESTION_BUCKET
+from data_ingestion.settings import DATA_INGESTION_BUCKET
 
 def test_get_s3_config(
     s3_client,
     mock_create_bucket,
 ):
     yaml_content = {
         "testing": {
```

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/tests/conftest.py` & `data_ingestion_lib-1.0.3/data_ingestion/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,14 @@
         TableName=DATA_INGESTION_METADATA_TABLE,
         Item={
             "PK": {"S": "TABLE_CONFIG#table"},
             "SK": {"S": "CONFIGTIME#122792905"},
             "domain_file": {"S": "test"},
             "cron": {"S": "0 0 * * ? *"},
             "status": {"S": "enabled"},
-            "is_active": {"S": "true"},
         },
     )
     dynamodb_client.put_item(
         TableName=DATA_INGESTION_METADATA_TABLE,
         Item={
             "PK": {"S": "TABLE_CONFIG#table"},
             "SK": {"S": "CONFIGTIME#latest"},
```

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/tests/crud/test_data_ingestion_metadata_table.py` & `data_ingestion_lib-1.0.3/data_ingestion/tests/crud/test_data_ingestion_metadata_table.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,124 @@
-from http import HTTPStatus
+from copy import deepcopy
 
 import pytest
+from pytest import MonkeyPatch
 
 from data_ingestion.crud.data_ingestion_metadata_table.DataIngestionConfig import (
     add_config,
-    add_latest_item,
-    get_active_config,
-    get_latest_config,
-    remove_is_active,
+    get_config_by_pk,
+    update_config,
 )
 from data_ingestion.model.data_ingestion_metadata_table.DataIngestionConfig import (
     DataIngestionConfig,
 )
 
-PK = "TABLE_CONFIG#table"
+PK = "CONFIG#TEST"
 table_name = "table"
-cron = "0 0 * * ? *"
-ITEM = DataIngestionConfig("test", table_name, "122792905", "enabled", cron)
+ITEM = DataIngestionConfig("TEST", table_name, "0 0 * * * *", "enabled", "122792905")
 
 
-def test_get_latest_config(dynamodb_client, mock_add_config_record):
-
-    result = get_latest_config(table_name, dynamodb_client)
-
-    assert result is not None
-    assert result.table_name == table_name
-    assert result.cron == cron
-
-
-def test_get_latest_config_none(
+def test_get_data_ingestion_config(
     dynamodb_client, mock_create_data_ingestion_metadata_table
 ):
 
-    result = get_latest_config(table_name, dynamodb_client)
+    add_config(
+        ITEM.to_dynamodb_item(),
+        dynamodb_client,
+    )
 
-    assert result is None
+    response = get_config_by_pk(PK, dynamodb_client)
 
+    assert response is not None
+    assert response[0].table_name == table_name
+    assert response[0].cron == "0 0 * * * *"
 
-def test_get_latest_config_exception(dynamodb_client):
-    with pytest.raises(Exception):
-        get_latest_config(table_name, dynamodb_client)
 
+def test_get_data_ingestion_config_no_config(
+    dynamodb_client, mock_create_data_ingestion_metadata_table
+):
+    response = get_config_by_pk(PK, dynamodb_client)
 
-def test_remove_is_active(dynamodb_client, mock_add_config_record):
-    result = remove_is_active(ITEM, dynamodb_client)
+    assert response == []
 
-    config = get_latest_config(table_name, dynamodb_client)
 
-    assert result == HTTPStatus.OK
-    assert config is not None
-    assert config.is_active is None
+def test_get_data_ingestion_exception(
+    dynamodb_client, mock_create_data_ingestion_metadata_table
+):
+    MonkeyPatch().setattr(dynamodb_client, "query", lambda *args, **kwargs: Exception)
+    with pytest.raises(Exception):
+        get_config_by_pk(PK, dynamodb_client)
 
 
-def test_is_active_exception(dynamodb_client):
+def test_update_data_ingestion_config(
+    dynamodb_client, mock_create_data_ingestion_metadata_table
+):
 
-    with pytest.raises(Exception):
-        remove_is_active(ITEM, dynamodb_client)
+    add_config(
+        ITEM.to_dynamodb_item(),
+        dynamodb_client,
+    )
 
+    updated_item = deepcopy(ITEM)
+    updated_item.cron = "0 1 * * * *"
+    updated_item.config_timestamp = "122792906"
 
-def test_get_active_config(dynamodb_client, mock_add_config_record):
+    update_config(updated_item, dynamodb_client)
 
-    result = get_active_config("test", dynamodb_client)
+    response = get_config_by_pk(PK, dynamodb_client)
 
-    assert result is not None
-    assert len(result) == 1
-    assert result[0].table_name == table_name
-    assert result[0].is_active == "true"
+    assert response is not None
+    assert response[0].table_name == table_name
+    assert response[0].cron == "0 1 * * * *"
 
 
-def test_get_active_config_none(
+def test_update_data_ingestion_conflict(
     dynamodb_client, mock_create_data_ingestion_metadata_table
 ):
+    add_config(
+        ITEM.to_dynamodb_item(),
+        dynamodb_client,
+    )
 
-    result = get_active_config("test", dynamodb_client)
+    updated_item = deepcopy(ITEM)
+    updated_item.cron = "0 1 * * * *"
+    updated_item.config_timestamp = "122792904"
 
-    assert result == []
+    response = update_config(updated_item, dynamodb_client)
 
+    assert response == 409
 
-def test_get_active_config_exception(dynamodb_client):
 
+def test_update_data_ingestion_exception(
+    dynamodb_client, mock_create_data_ingestion_metadata_table
+):
+    MonkeyPatch().setattr(
+        dynamodb_client, "update_item", lambda *args, **kwargs: Exception
+    )
     with pytest.raises(Exception):
-        get_active_config("test", dynamodb_client)
+        update_config(ITEM, dynamodb_client)
 
 
-def test_add_data_ingestion_conflict(dynamodb_client, mock_add_config_record):
+def test_add_data_ingestion_conflict(
+    dynamodb_client, mock_create_data_ingestion_metadata_table
+):
+    add_config(
+        ITEM.to_dynamodb_item(),
+        dynamodb_client,
+    )
+
     response = add_config(
         ITEM.to_dynamodb_item(),
         dynamodb_client,
     )
 
     assert response == 409
 
 
-def test_add_data_ingestion_exception(dynamodb_client):
+def test_add_data_ingestion_exception(
+    dynamodb_client, mock_create_data_ingestion_metadata_table
+):
+    MonkeyPatch().setattr(
+        dynamodb_client, "put_item", lambda *args, **kwargs: Exception
+    )
     with pytest.raises(Exception):
         add_config(ITEM.to_dynamodb_item(), dynamodb_client)
-
-
-def test_add_latest_item(dynamodb_client, mock_add_config_record):
-    result = add_latest_item(table_name, "122792906", dynamodb_client)
-
-    assert result == HTTPStatus.OK
-
-
-def test_add_latest_item_conflict(dynamodb_client, mock_add_config_record):
-
-    result = add_latest_item(table_name, "122792905", dynamodb_client)
-
-    assert result == HTTPStatus.CONFLICT
-
-
-def test_add_latest_item_exception(dynamodb_client):
-
-    with pytest.raises(Exception):
-        add_latest_item(table_name, "122792906", dynamodb_client)
```

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/tests/crud/test_export_status.py` & `data_ingestion_lib-1.0.3/data_ingestion/tests/crud/test_export_status.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/tests/utils/test_data_ingestion_utils.py` & `data_ingestion_lib-1.0.3/data_ingestion/tests/utils/test_data_ingestion_utils.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/utils/common.py` & `data_ingestion_lib-1.0.3/data_ingestion/utils/common.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.2/data_ingestion/utils/logger.py` & `data_ingestion_lib-1.0.3/data_ingestion/utils/logger.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.2/PKG-INFO` & `data_ingestion_lib-1.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: data-ingestion-lib
-Version: 1.0.2
+Version: 1.0.3
 Summary: Data ingestion module 
 Author: Dat Nguyen
 Author-email: dat.nguyen2@tyme.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: boto3 (>=1.34,<2.0)
-Requires-Dist: moto (==4.2.9)
 Requires-Dist: mypy_boto3_dynamodb (>=1.34,<2.0)
 Requires-Dist: mypy_boto3_s3 (>=1.34,<2.0)
-Requires-Dist: pytest (>=7.2,<8.0)
 Requires-Dist: python-json-logger (>=2.0,<3.0)
```

