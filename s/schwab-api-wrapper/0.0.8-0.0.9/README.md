# Comparing `tmp/schwab_api_wrapper-0.0.8.tar.gz` & `tmp/schwab_api_wrapper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_api_wrapper-0.0.8.tar", last modified: Sun May 26 22:27:05 2024, max compression
+gzip compressed data, was "schwab_api_wrapper-0.0.9.tar", last modified: Mon May 27 15:06:37 2024, max compression
```

## Comparing `schwab_api_wrapper-0.0.8.tar` & `schwab_api_wrapper-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-26 22:27:05.699656 schwab_api_wrapper-0.0.8/
--rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/LICENSE
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-26 22:27:05.699456 schwab_api_wrapper-0.0.8/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/README.md
--rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-26 22:26:39.000000 schwab_api_wrapper-0.0.8/pyproject.toml
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-26 22:27:05.695696 schwab_api_wrapper-0.0.8/schwab_api_wrapper/
--rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/__main__.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-26 22:27:05.697173 schwab_api_wrapper-0.0.8/schwab_api_wrapper/market_data/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/market_data/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/market_data/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/market_data/market_hours_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/market_data/price_history_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/market_data/quotes_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/response_aware_retry.py
--rw-r--r--   0 owengordon   (501) staff       (20)    36931 2024-05-26 22:26:28.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/schwab.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-26 22:27:05.698294 schwab_api_wrapper-0.0.8/schwab_api_wrapper/trader_api/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/trader_api/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/trader_api/accounts_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/trader_api/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     9122 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/trader_api/orders_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     5497 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/trader_api/transactions_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper/utils.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-26 22:27:05.699251 schwab_api_wrapper-0.0.8/schwab_api_wrapper.egg-info/
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-26 22:27:05.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)      879 2024-05-26 22:27:05.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-26 22:27:05.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-26 22:27:05.000000 schwab_api_wrapper-0.0.8/schwab_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-26 22:27:05.699698 schwab_api_wrapper-0.0.8/setup.cfg
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-26 22:27:05.698687 schwab_api_wrapper-0.0.8/tests/
--rw-r--r--   0 owengordon   (501) staff       (20)    45372 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.8/tests/test_schawb_api.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 15:06:37.973269 schwab_api_wrapper-0.0.9/
+-rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/LICENSE
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 15:06:37.973048 schwab_api_wrapper-0.0.9/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/README.md
+-rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-27 15:05:58.000000 schwab_api_wrapper-0.0.9/pyproject.toml
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 15:06:37.969459 schwab_api_wrapper-0.0.9/schwab_api_wrapper/
+-rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/__main__.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 15:06:37.970861 schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/market_hours_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/price_history_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/quotes_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/response_aware_retry.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    36931 2024-05-26 22:26:28.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/schwab.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 15:06:37.972001 schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/accounts_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/orders_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     5497 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/transactions_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/utils.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 15:06:37.972798 schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 15:06:37.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)      879 2024-05-27 15:06:37.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-27 15:06:37.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-27 15:06:37.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-27 15:06:37.973318 schwab_api_wrapper-0.0.9/setup.cfg
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 15:06:37.972270 schwab_api_wrapper-0.0.9/tests/
+-rw-r--r--   0 owengordon   (501) staff       (20)    45372 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/tests/test_schawb_api.py
```

### Comparing `schwab_api_wrapper-0.0.8/LICENSE` & `schwab_api_wrapper-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.8/PKG-INFO` & `schwab_api_wrapper-0.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.0.8
+Version: 0.0.9
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.0.8/pyproject.toml` & `schwab_api_wrapper-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schwab_api_wrapper"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Owen Gordon", email="owengordon330@outlook.com" },
 ]
 description = "A wrapper package around the schwab http api"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper/__main__.py` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper/market_data/errors_schema.py` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/errors_schema.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper/market_data/market_hours_schemas.py` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/market_hours_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper/market_data/price_history_schemas.py` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/price_history_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper/market_data/quotes_schemas.py` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/quotes_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper/response_aware_retry.py` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper/response_aware_retry.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper/schwab.py` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper/schwab.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper/trader_api/accounts_schemas.py` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/accounts_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper/trader_api/orders_schemas.py` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/orders_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,14 +233,15 @@
 class ActivityType(Enum):
     EXECUTION = "EXECUTION"
     ORDER_ACTION = "ORDER_ACTION"
 
 
 class ExecutionType(Enum):
     FILL = "FILL"
+    CANCELED = "CANCELED"
 
 
 class ExecutionLeg(BaseModel):
     legId: int
     price: float
     quantity: float
     mismarkedQuantity: float
```

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper/trader_api/transactions_schemas.py` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/transactions_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper/utils.py` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper.egg-info/PKG-INFO` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.0.8
+Version: 0.0.9
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.0.8/schwab_api_wrapper.egg-info/SOURCES.txt` & `schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.8/tests/test_schawb_api.py` & `schwab_api_wrapper-0.0.9/tests/test_schawb_api.py`

 * *Files identical despite different names*

