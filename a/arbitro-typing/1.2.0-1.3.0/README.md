# Comparing `tmp/arbitro_typing-1.2.0.tar.gz` & `tmp/arbitro_typing-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arbitro_typing-1.2.0.tar", max compression
+gzip compressed data, was "arbitro_typing-1.3.0.tar", max compression
```

## Comparing `arbitro_typing-1.2.0.tar` & `arbitro_typing-1.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-08 16:38:06.133912 arbitro_typing-1.2.0/arbitro_typing/__init__.py
--rw-r--r--   0        0        0      979 2024-05-27 16:16:55.338502 arbitro_typing-1.2.0/arbitro_typing/data_types.py
--rw-r--r--   0        0        0     5510 2024-05-27 16:16:26.249331 arbitro_typing-1.2.0/arbitro_typing/models/operations.py
--rw-r--r--   0        0        0     1097 2024-05-08 16:52:49.200238 arbitro_typing-1.2.0/LICENSE
--rw-r--r--   0        0        0      332 2024-05-27 16:28:43.361645 arbitro_typing-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      159 2024-05-08 17:22:18.452296 arbitro_typing-1.2.0/README.md
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 arbitro_typing-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-08 16:38:06.133912 arbitro_typing-1.3.0/arbitro_typing/__init__.py
+-rw-r--r--   0        0        0      979 2024-05-27 16:16:55.338502 arbitro_typing-1.3.0/arbitro_typing/data_types.py
+-rw-r--r--   0        0        0     5553 2024-05-27 20:22:19.379298 arbitro_typing-1.3.0/arbitro_typing/models/operations.py
+-rw-r--r--   0        0        0     1097 2024-05-08 16:52:49.200238 arbitro_typing-1.3.0/LICENSE
+-rw-r--r--   0        0        0      332 2024-05-27 20:22:44.381266 arbitro_typing-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      159 2024-05-08 17:22:18.452296 arbitro_typing-1.3.0/README.md
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 arbitro_typing-1.3.0/PKG-INFO
```

### Comparing `arbitro_typing-1.2.0/arbitro_typing/data_types.py` & `arbitro_typing-1.3.0/arbitro_typing/data_types.py`

 * *Files identical despite different names*

### Comparing `arbitro_typing-1.2.0/arbitro_typing/models/operations.py` & `arbitro_typing-1.3.0/arbitro_typing/models/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     client: Optional[Bank] = None
     product: Optional[Product] = None
     receive_pay: Optional[ReceivePay] = None
     counterparty: Optional[Bank] = None
     amount: Optional[int] = None
     maturity: Optional[int] = None
     rate: Optional[float] = None
+    exchange_rate: Optional[float] = None
     client_confirmed_status: Optional[bool] = None
     confirmed_status: Optional[bool] = None
     operation_pair: Optional[PyObjectId] = None
     model_config = ConfigDict(
         json_encoders={ObjectId: str},
     )
```

### Comparing `arbitro_typing-1.2.0/LICENSE` & `arbitro_typing-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arbitro_typing-1.2.0/PKG-INFO` & `arbitro_typing-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arbitro-typing
-Version: 1.2.0
+Version: 1.3.0
 Summary: 
 Author: Diego Villegas
 Author-email: dvillegas@creasys.cl
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

