# Comparing `tmp/pyextrica-17.2.0.tar.gz` & `tmp/pyextrica-17.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyextrica-17.2.0.tar", last modified: Tue May 14 05:36:16 2024, max compression
+gzip compressed data, was "pyextrica-17.2.1.tar", last modified: Mon May 27 12:43:42 2024, max compression
```

## Comparing `pyextrica-17.2.0.tar` & `pyextrica-17.2.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 05:36:16.062306 pyextrica-17.2.0/
--rw-rw-rw-   0        0        0     6464 2024-05-14 05:36:16.061316 pyextrica-17.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4210 2024-05-13 12:56:16.000000 pyextrica-17.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 05:36:16.028119 pyextrica-17.2.0/pyextrica/
--rw-rw-rw-   0        0        0      546 2024-04-30 12:13:31.000000 pyextrica-17.2.0/pyextrica/__init__.py
--rw-rw-rw-   0        0        0      241 2024-05-14 05:34:53.000000 pyextrica-17.2.0/pyextrica/_version.py
--rw-rw-rw-   0        0        0     1939 2024-03-28 08:25:23.000000 pyextrica-17.2.0/pyextrica/auth.py
--rw-rw-rw-   0        0        0    47797 2024-03-28 08:34:43.000000 pyextrica-17.2.0/pyextrica/client.py
--rw-rw-rw-   0        0        0     1531 2024-03-28 11:09:57.000000 pyextrica-17.2.0/pyextrica/constants.py
--rw-rw-rw-   0        0        0    25183 2024-03-28 11:11:29.000000 pyextrica-17.2.0/pyextrica/dbapi.py
--rw-rw-rw-   0        0        0     2776 2024-03-28 11:11:29.000000 pyextrica-17.2.0/pyextrica/exceptions.py
--rw-rw-rw-   0        0        0    14837 2024-03-28 08:34:43.000000 pyextrica-17.2.0/pyextrica/extrica_rest_handler.py
--rw-rw-rw-   0        0        0      577 2024-03-28 08:34:43.000000 pyextrica-17.2.0/pyextrica/logging.py
--rw-rw-rw-   0        0        0     8821 2024-05-13 13:05:37.000000 pyextrica-17.2.0/pyextrica/pyextrica_functions.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:36:16.052808 pyextrica-17.2.0/pyextrica/sqlalchemy/
--rw-rw-rw-   0        0        0      153 2024-03-28 08:23:52.000000 pyextrica-17.2.0/pyextrica/sqlalchemy/__init__.py
--rw-rw-rw-   0        0        0     6725 2024-03-28 08:23:52.000000 pyextrica-17.2.0/pyextrica/sqlalchemy/compiler.py
--rw-rw-rw-   0        0        0     7887 2024-03-28 08:23:52.000000 pyextrica-17.2.0/pyextrica/sqlalchemy/datatype.py
--rw-rw-rw-   0        0        0    13927 2024-03-28 08:23:52.000000 pyextrica-17.2.0/pyextrica/sqlalchemy/dialect.py
--rw-rw-rw-   0        0        0      559 2024-03-28 08:25:23.000000 pyextrica-17.2.0/pyextrica/sqlalchemy/error.py
--rw-rw-rw-   0        0        0     3459 2024-03-22 10:22:46.000000 pyextrica-17.2.0/pyextrica/sqlalchemy/util.py
--rw-rw-rw-   0        0        0     3094 2024-05-13 13:11:42.000000 pyextrica-17.2.0/pyextrica/transaction.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:36:16.055812 pyextrica-17.2.0/pyextrica.egg-info/
--rw-rw-rw-   0        0        0     6464 2024-05-14 05:36:15.000000 pyextrica-17.2.0/pyextrica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      679 2024-05-14 05:36:15.000000 pyextrica-17.2.0/pyextrica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 05:36:15.000000 pyextrica-17.2.0/pyextrica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-05-14 05:36:15.000000 pyextrica-17.2.0/pyextrica.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      357 2024-05-14 05:36:15.000000 pyextrica-17.2.0/pyextrica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-14 05:36:15.000000 pyextrica-17.2.0/pyextrica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      432 2024-05-14 05:36:16.065299 pyextrica-17.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2625 2024-05-13 06:42:43.000000 pyextrica-17.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:43:42.095489 pyextrica-17.2.1/
+-rw-rw-rw-   0        0        0     6526 2024-05-27 12:43:42.093491 pyextrica-17.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4235 2024-05-15 07:23:34.000000 pyextrica-17.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 12:43:42.010927 pyextrica-17.2.1/pyextrica/
+-rw-rw-rw-   0        0        0      546 2024-05-27 11:43:53.000000 pyextrica-17.2.1/pyextrica/__init__.py
+-rw-rw-rw-   0        0        0      241 2024-05-27 11:43:20.000000 pyextrica-17.2.1/pyextrica/_version.py
+-rw-rw-rw-   0        0        0     1939 2024-03-28 08:25:24.000000 pyextrica-17.2.1/pyextrica/auth.py
+-rw-rw-rw-   0        0        0    48111 2024-05-27 10:51:36.000000 pyextrica-17.2.1/pyextrica/client.py
+-rw-rw-rw-   0        0        0     1531 2024-03-28 11:09:58.000000 pyextrica-17.2.1/pyextrica/constants.py
+-rw-rw-rw-   0        0        0    25191 2024-05-10 05:56:08.000000 pyextrica-17.2.1/pyextrica/dbapi.py
+-rw-rw-rw-   0        0        0     2776 2024-03-28 11:11:30.000000 pyextrica-17.2.1/pyextrica/exceptions.py
+-rw-rw-rw-   0        0        0    16338 2024-05-27 11:13:23.000000 pyextrica-17.2.1/pyextrica/extrica_rest_handler.py
+-rw-rw-rw-   0        0        0      577 2024-03-28 08:34:44.000000 pyextrica-17.2.1/pyextrica/logging.py
+-rw-rw-rw-   0        0        0     8821 2024-05-27 11:47:25.000000 pyextrica-17.2.1/pyextrica/pyextrica_functions.py
+-rw-rw-rw-   0        0        0     2103 2024-05-15 12:51:14.000000 pyextrica-17.2.1/pyextrica/query_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:43:42.077487 pyextrica-17.2.1/pyextrica/sqlalchemy/
+-rw-rw-rw-   0        0        0      153 2024-03-28 08:23:54.000000 pyextrica-17.2.1/pyextrica/sqlalchemy/__init__.py
+-rw-rw-rw-   0        0        0     6725 2024-03-28 08:23:54.000000 pyextrica-17.2.1/pyextrica/sqlalchemy/compiler.py
+-rw-rw-rw-   0        0        0     8054 2024-05-27 11:52:48.000000 pyextrica-17.2.1/pyextrica/sqlalchemy/datatype.py
+-rw-rw-rw-   0        0        0    16550 2024-05-27 11:56:02.000000 pyextrica-17.2.1/pyextrica/sqlalchemy/dialect.py
+-rw-rw-rw-   0        0        0      559 2024-03-28 08:25:24.000000 pyextrica-17.2.1/pyextrica/sqlalchemy/error.py
+-rw-rw-rw-   0        0        0     3459 2024-03-22 10:22:48.000000 pyextrica-17.2.1/pyextrica/sqlalchemy/util.py
+-rw-rw-rw-   0        0        0     3094 2024-05-27 11:00:43.000000 pyextrica-17.2.1/pyextrica/transaction.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:43:42.084491 pyextrica-17.2.1/pyextrica.egg-info/
+-rw-rw-rw-   0        0        0     6526 2024-05-27 12:43:41.000000 pyextrica-17.2.1/pyextrica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2024-05-27 12:43:41.000000 pyextrica-17.2.1/pyextrica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 12:43:41.000000 pyextrica-17.2.1/pyextrica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-27 12:43:41.000000 pyextrica-17.2.1/pyextrica.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      378 2024-05-27 12:43:41.000000 pyextrica-17.2.1/pyextrica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-27 12:43:41.000000 pyextrica-17.2.1/pyextrica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      432 2024-05-27 12:43:42.100487 pyextrica-17.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2657 2024-05-27 12:38:37.000000 pyextrica-17.2.1/setup.py
```

### Comparing `pyextrica-17.2.0/PKG-INFO` & `pyextrica-17.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyextrica
-Version: 17.2.0
+Version: 17.2.1
 Summary: Python client library for Extrica
 Home-page: https://github.com/extricatrianz/pyextrica
 Author: Extrica Team
 Author-email: extricaproductionsupport@trianz.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,14 +25,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: backports.zoneinfo; python_version < "3.9"
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: requests>=2.31.0
 Requires-Dist: tzlocal
 Requires-Dist: sqlalchemy>=1.3
+Requires-Dist: sql_metadata==2.11.0
 Provides-Extra: all
 Requires-Dist: requests_kerberos; extra == "all"
 Requires-Dist: sqlalchemy>=1.3; extra == "all"
 Provides-Extra: kerberos
 Requires-Dist: requests_kerberos; extra == "kerberos"
 Provides-Extra: sqlalchemy
 Requires-Dist: sqlalchemy>=1.3; extra == "sqlalchemy"
@@ -46,15 +47,15 @@
 Requires-Dist: black; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Provides-Extra: external-authentication-token-cache
 Requires-Dist: keyring; extra == "external-authentication-token-cache"
 
 # PyExtrica Library for Extrica Product
 
-PyExtrica allows you to query and transform data in Extrica (Data To AI) platform directly without having to download the data locally. This library provides seamless access to the Extrica platform, allowing users to execute SQL queries and retrieve metadata such as catalog names, schema names, table names, and column information.
+PyExtrica allows you to query and transform data in [Extrica](https://extrica.ai/) (Data To AI) platform directly without having to download the data locally. This library provides seamless access to the Extrica platform, allowing users to execute SQL queries and retrieve metadata such as catalog names, schema names, table names, and column information.
 
 ## Getting Started
 
 ### Installation
 You can install PyExtrica via pip:
 
 ```bash
@@ -132,15 +133,15 @@
 print(joined_df.head())
 ```
 
 ### Available Methods
 PyExtrica provides the following methods for interacting with the Extrica platform:
 
 - extrica_engine: Connects to the Extrica platform.
-execute_sql_query: Executes SQL queries.
+- execute_sql_query: Executes SQL queries.
 - get_catalog_names: Retrieves catalog names. (Requires platform=data_products for data products or platform=data_sources for data sources). For data products, catalog name represents the domain name, and schema name represents the subdomain name. For data sources, it is similar to Trino catalog and schema.
 - get_schema_names: Retrieves schema names. (Requires platform=data_products for data products or platform=data_sources for data sources)
 - get_table_names: Retrieves table names. (Requires platform=data_products for data products or platform=data_sources for data sources)
 - get_table_columns: Retrieves column information for a specified table. (Requires platform=data_products for data products or platform=data_sources for data sources)
 
 ```python
 # Retrieve catalog names
```

### Comparing `pyextrica-17.2.0/README.md` & `pyextrica-17.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PyExtrica Library for Extrica Product
 
-PyExtrica allows you to query and transform data in Extrica (Data To AI) platform directly without having to download the data locally. This library provides seamless access to the Extrica platform, allowing users to execute SQL queries and retrieve metadata such as catalog names, schema names, table names, and column information.
+PyExtrica allows you to query and transform data in [Extrica](https://extrica.ai/) (Data To AI) platform directly without having to download the data locally. This library provides seamless access to the Extrica platform, allowing users to execute SQL queries and retrieve metadata such as catalog names, schema names, table names, and column information.
 
 ## Getting Started
 
 ### Installation
 You can install PyExtrica via pip:
 
 ```bash
@@ -82,15 +82,15 @@
 print(joined_df.head())
 ```
 
 ### Available Methods
 PyExtrica provides the following methods for interacting with the Extrica platform:
 
 - extrica_engine: Connects to the Extrica platform.
-execute_sql_query: Executes SQL queries.
+- execute_sql_query: Executes SQL queries.
 - get_catalog_names: Retrieves catalog names. (Requires platform=data_products for data products or platform=data_sources for data sources). For data products, catalog name represents the domain name, and schema name represents the subdomain name. For data sources, it is similar to Trino catalog and schema.
 - get_schema_names: Retrieves schema names. (Requires platform=data_products for data products or platform=data_sources for data sources)
 - get_table_names: Retrieves table names. (Requires platform=data_products for data products or platform=data_sources for data sources)
 - get_table_columns: Retrieves column information for a specified table. (Requires platform=data_products for data products or platform=data_sources for data sources)
 
 ```python
 # Retrieve catalog names
```

### Comparing `pyextrica-17.2.0/pyextrica/__init__.py` & `pyextrica-17.2.1/pyextrica/__init__.py`

 * *Files identical despite different names*

### Comparing `pyextrica-17.2.0/pyextrica/auth.py` & `pyextrica-17.2.1/pyextrica/auth.py`

 * *Files identical despite different names*

### Comparing `pyextrica-17.2.0/pyextrica/client.py` & `pyextrica-17.2.1/pyextrica/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 from dateutil import tz
 from tzlocal import get_localzone_name 
 
 from pyextrica.extrica_rest_handler import ExtricaHTTPHandler
 import pyextrica.logging
 from pyextrica import constants, exceptions
 from pyextrica._version import __version__
+from pyextrica.query_parser import QueryParser
 
 __all__ = ["ClientSession", "TrinoQuery", "TrinoRequest", "PROXIES"]
 
 logger = pyextrica.logging.get_logger(__name__)
 
 MAX_ATTEMPTS = constants.DEFAULT_MAX_ATTEMPTS
 SOCKS_PROXY = os.environ.get("SOCKS_PROXY")
@@ -734,14 +735,15 @@
         self._update_count = None
         self._next_uri = None
         self._query = query
         self._result: Optional[TrinoResult] = None
         self._legacy_primitive_types = legacy_primitive_types
         self._row_mapper: Optional[RowMapper] = None
         self._extrica_http_handler = ExtricaHTTPHandler("https://"+request._host, self._request._client_session.access_token)
+        self._query_parser = QueryParser()
 
     @property
     def query_id(self) -> Optional[str]:
         return self._query_id
 
     @property
     def query(self) -> Optional[str]:
@@ -789,22 +791,24 @@
         """
         if self.cancelled:
             raise exceptions.TrinoUserError("Query has been cancelled", self.query_id)
 
         try:
             session = self._request._client_session
             # QUERY TYPE, QUERY_FOR, IS_TABLE_QUERY, SCHEMA_NAME/VALUES, MODIFIED_QUERY
-           
+            is_capability_query = self._query_parser.parse_query(self._query, session.platform)
             #API to fetch modified query : calling pyextrica query engine API
-            modified_response = self._extrica_http_handler._get_modified_query(session.user, self._query,session.access_token)
-            if not modified_response.ok:
-                self._request.raise_response_error(modified_response)
-           
-            modified_extrica_query = modified_response.text
-            #Modified query to be passed to trion query engine to get resultset
+            if not is_capability_query:
+                self._query = self._query_parser.remove_schema_from_query(self._query, session.platform)
+                modified_response = self._extrica_http_handler._get_modified_query(session.user, self._query,session.access_token)
+                if not modified_response.ok:
+                    self._request.raise_response_error(modified_response)
+                modified_extrica_query = modified_response.text
+            else:
+                modified_extrica_query = self._query
             response = self._request.post(modified_extrica_query, additional_http_headers)
              
         except requests.exceptions.RequestException as e:
             raise pyextrica.exceptions.TrinoConnectionError("failed to execute: {}".format(e))
         status = self._request.process(response)
         self._info_uri = status.info_uri
         self._query_id = status.id
```

### Comparing `pyextrica-17.2.0/pyextrica/constants.py` & `pyextrica-17.2.1/pyextrica/constants.py`

 * *Files identical despite different names*

### Comparing `pyextrica-17.2.0/pyextrica/dbapi.py` & `pyextrica-17.2.1/pyextrica/dbapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,18 +267,18 @@
     def _use_legacy_prepared_statements(self):
         if self.legacy_prepared_statements is not None:
             return self.legacy_prepared_statements
 
         value = must_use_legacy_prepared_statements.get((self.host, self.port))
         if value is None:
             try:
-                query = pyextrica.client.TrinoQuery(
-                    self._create_request(),
-                    query="EXECUTE IMMEDIATE 'SELECT 1'")
-                query.execute()
+                # query = pyextrica.client.TrinoQuery(
+                #     self._create_request(),
+                #     query="EXECUTE IMMEDIATE 'SELECT 1'")
+                # query.execute()
                 value = False
             except Exception as e:
                 logger.warning(
                     "EXECUTE IMMEDIATE not available for %s:%s; defaulting to legacy prepared statements (%s)",
                     self.host, self.port, e)
                 value = True
             must_use_legacy_prepared_statements.put((self.host, self.port), value)
```

### Comparing `pyextrica-17.2.0/pyextrica/exceptions.py` & `pyextrica-17.2.1/pyextrica/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyextrica-17.2.0/pyextrica/extrica_rest_handler.py` & `pyextrica-17.2.1/pyextrica/extrica_rest_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 from urllib.parse import quote
 import requests
+from pyextrica.sqlalchemy import datatype
 
 __all__ = ["ExtricaHTTPHandler"]
 
 class ExtricaHTTPHandler:
 
     def __init__(self, base_url, access_token):
         self._base_url = base_url
@@ -126,14 +127,30 @@
             data = response.json()
             schemas = [item['domain'] for item in data]
             return schemas
         except requests.exceptions.RequestException as e:
             print(f"Error occurred while fetching schemas: {e}")
             return []
         
+    def _get_schemas_dp_1(email, token, host, params):
+        encoded_params = "&".join([f"{key}={quote(str(value))}" for key, value in params.items()])
+        url = f"https://{host}/core/python/schemas/{email}"
+        headers = {"Authorization": f"Bearer {token}"}
+
+        url_with_params = f"{url}?{encoded_params}"
+        try:
+            response = requests.get(url_with_params, headers=headers)
+            response.raise_for_status()
+            data = response.json()
+            return data["data"]
+        except requests.exceptions.RequestException as e:
+                print(f"Error occurred while fetching schemas: {e}")
+                return []
+    
+        
     def _get_tables_dp(userEmail, domainName, token, host, subDomainName):
         """
         Function to retrieve data product names from the Extrica Data Product platform.
         
         This function makes a request to the specified host with provided user email, domain name, token, and subdomain name
         to fetch data product names from the Extrica Data Product platform.
         
@@ -158,15 +175,29 @@
             tables = []
             for key in data:
                 tables.extend(data[key])
             return tables
         except requests.exceptions.RequestException as e:
             print(f"Error occurred while fetching tables: {e}")
             return []
-        
+    
+    def _get_tables_dp_1(email, token, host, params=None):
+        encoded_params = "&".join([f"{key}={quote(str(value))}" for key, value in params.items()])
+        # endpoint = f"/core/python/tables/sreekanth.gude"
+        endpoint = f"https://{host}/core/python/tables/{email}"
+        url_with_params = f"{endpoint}?{encoded_params}"
+        headers = {'Authorization': 'Bearer '+token}
+        try:
+            response = requests.get(url=url_with_params,headers=headers)
+            data = response.json()
+            return data["data"]
+        except requests.exceptions.RequestException as e:
+            print(f"Error occurred while fetching tables: {e}")
+            return []  
+          
     def _get_columns_dp(userEmail, token, host, dataproduct):
         """
         Function to retrieve columns of a data product from the Extrica Data Product platform and return as a dictionary.
         
         This function makes a request to the specified host with provided user email, token, and data product
         to fetch columns from the Extrica Data Product platform.
         
@@ -186,17 +217,17 @@
             headers = {'Authorization': f'Bearer {token}', 'Content-Type': 'application/json'}
             response = requests.get(url, headers=headers)
             data = response.json()
             dataproduct = data.get('dataproduct', {})
             columns = dataproduct.get('columns', [])
             for column in columns:
                 name = column.get('name')
-                column_type = column.get('type')
+                column_type = datatype.parse_sqltype(column.get('type'))
                 if name and column_type:
-                    columns_list.append({'name': name, 'dataType': column_type})
+                    columns_list.append({'name': name, 'type': column_type, 'nullable':'YES'})
         except Exception as e:
             print(f"Error occurred while extracting columns: {e}")
         return columns_list
     
     def _get_catalogs_ds(host, userEmail, token):
         """
         Function to retrieve catalogs of data sources from the Extrica platform.
@@ -312,15 +343,15 @@
             columns_info = []
             response = requests.get(url, headers=headers)
             data = response.json()
             for column_data in data:
                 column_name = column_data.get('name')
                 data_type = column_data.get('dataType')
                 if column_name and data_type:
-                    column_info = {'name': column_name, 'dataType': data_type}
+                    column_info = {'name': column_name, 'type': data_type, 'nullable':'YES'}
                     columns_info.append(column_info)
             return columns_info
         except Exception as e:
             print(f"Error occurred while extracting columns: {e}")
             return []
```

### Comparing `pyextrica-17.2.0/pyextrica/logging.py` & `pyextrica-17.2.1/pyextrica/logging.py`

 * *Files identical despite different names*

### Comparing `pyextrica-17.2.0/pyextrica/pyextrica_functions.py` & `pyextrica-17.2.1/pyextrica/pyextrica_functions.py`

 * *Files identical despite different names*

### Comparing `pyextrica-17.2.0/pyextrica/sqlalchemy/compiler.py` & `pyextrica-17.2.1/pyextrica/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `pyextrica-17.2.0/pyextrica/sqlalchemy/datatype.py` & `pyextrica-17.2.1/pyextrica/sqlalchemy/datatype.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import re
 from typing import Any, Dict, Iterator, List, Optional, Tuple, Type, Union
-
 import sqlalchemy
 from sqlalchemy import func, util
 from sqlalchemy.sql import sqltypes
 from sqlalchemy.sql.type_api import TypeDecorator, TypeEngine
 from sqlalchemy.types import JSON
 
 SQLType = Union[TypeEngine, Type[TypeEngine]]
@@ -124,30 +123,35 @@
     "boolean": sqltypes.BOOLEAN,
     # === Integer ===
     "tinyint": sqltypes.SMALLINT,
     "smallint": sqltypes.SMALLINT,
     "int": sqltypes.INTEGER,
     "integer": sqltypes.INTEGER,
     "bigint": sqltypes.BIGINT,
+    "number": sqltypes.NUMERIC,
     # === Floating-point ===
     "real": sqltypes.REAL,
     "double": DOUBLE,
     # === Fixed-precision ===
     "decimal": sqltypes.DECIMAL,
     # === String ===
     "varchar": sqltypes.VARCHAR,
     "char": sqltypes.CHAR,
+    "text": sqltypes.VARCHAR,
+    "varchar2":sqltypes.VARCHAR,
+    "character varying":sqltypes.VARCHAR,
     "varbinary": sqltypes.VARBINARY,
     "json": JSON,
     # === Date and time ===
     "date": sqltypes.DATE,
     "time": TIME,
     "time with time zone": TIME,
     "timestamp": TIMESTAMP,
-    "timestamp with time zone": TIMESTAMP
+    "timestamp with time zone": TIMESTAMP,
+    "timestamp_ntz":TIMESTAMP
 }
 
 if hasattr(sqlalchemy, "Uuid"):
     _type_map["uuid"] = sqlalchemy.Uuid
 
 
 def unquote(string: str, quote: str = '"', escape: str = "\\") -> str:
```

### Comparing `pyextrica-17.2.0/pyextrica/sqlalchemy/dialect.py` & `pyextrica-17.2.1/pyextrica/sqlalchemy/dialect.py`

 * *Files 12% similar despite different names*

```diff
@@ -156,15 +156,14 @@
             if schema is None:
                 schema = self._get_default_schema_name(connection)
             if schema is None:
                 raise ValueError("Please provide a schema.")
             catalog=self._get_default_catalog_name(connection)
             columns = ExtricaHTTPHandler._get_columns_ds(user,token, host,catalog,schema,table)
             return columns
-            
 
     def get_catalog_names(self, connection: Connection, **kw) -> List[str]:
         """
         Retrieve catalog names from the specified platform using REST API calls.
 
         This method first determines the platform (Data Products or Data Sources) associated with the provided connection.
         It then retrieves authentication details, such as token and host, from the connection.
@@ -219,16 +218,21 @@
             if not catalog:
                 raise ValueError("Please provide a catalog name.")
         auth = self._get_default_auth(connection)
         token = auth.token
         host=self._get_default_host(connection)
         user=self._get_default_user(connection)
         if platform == 'data_products':
-            schemas = ExtricaHTTPHandler._get_schemas_dp(user, catalog, token, host)
-            return schemas
+            if catalog == 'system':
+                params = {"platform": platform, "catalog": catalog}
+                schemas = ExtricaHTTPHandler._get_schemas_dp_1(user, token, host, params)
+                return schemas
+            else:
+                schemas = ExtricaHTTPHandler._get_schemas_dp(user, catalog, token, host)
+                return schemas
         else:
             schemas = ExtricaHTTPHandler._get_schemas_ds(user, catalog, token, host)
             return schemas
 
 
     def get_table_names(self, connection: Connection, schema: str = None, **kw) -> List[str]:
         """
@@ -259,20 +263,62 @@
         auth = self._get_default_auth(connection)
         token = auth.token
         host=self._get_default_host(connection)
         catalog=self._get_default_catalog_name(connection)
         user=self._get_default_user(connection)
         schema=schema
         if platform == 'data_products':
-            tables = ExtricaHTTPHandler._get_tables_dp(user, catalog, token, host, schema)
-            return tables
+            if catalog == 'system':
+                params = {"platform": platform, "catalog": catalog, "schema": schema}
+                tables = ExtricaHTTPHandler._get_tables_dp_1(user, token, host, params)
+                table_names = [table[0] for table in tables]  
+                return table_names
+            else:
+                tables = ExtricaHTTPHandler._get_tables_dp(user, catalog, token, host, schema)
+                return tables
+
         else:
             tables = ExtricaHTTPHandler._get_tables_ds(user, catalog, token, host, schema)
             return tables
 
+    def get_pk_constraint(self, connection: Connection, table_name: str, schema: str = None, **kw) -> Dict[str, Any]:
+        """Trino has no support for primary keys. Returns a dummy"""
+        return dict(name=None, constrained_columns=[])
+
+    def get_primary_keys(self, connection: Connection, table_name: str, schema: str = None, **kw) -> List[str]:
+        pk = self.get_pk_constraint(connection, table_name, schema)
+        return pk.get("constrained_columns") 
+
+    def get_foreign_keys(
+        self, connection: Connection, table_name: str, schema: str = None, **kw
+    ) -> List[Dict[str, Any]]:
+        """Trino has no support for foreign keys. Returns an empty list."""
+        return []
+
+    def get_sequence_names(self, connection: Connection, schema: str = None, **kw) -> List[str]:
+        """Trino has no support for sequences. Returns an empty list."""
+        return []
+
+    def get_unique_constraints(
+        self, connection: Connection, table_name: str, schema: str = None, **kw
+    ) -> List[Dict[str, Any]]:
+        """Trino has no support for unique constraints. Returns an empty list."""
+        return []
+
+    def get_check_constraints(
+        self, connection: Connection, table_name: str, schema: str = None, **kw
+    ) -> List[Dict[str, Any]]:
+        """Trino has no support for check constraints. Returns an empty list."""
+        return []
+    
+    def get_indexes(self, connection: Connection, table_name: str, schema: str = None, **kw) -> List[Dict[str, Any]]:
+        """Extrica has no support for indexes."""
+        return []
+
+
     def _raw_connection(self, connection: Union[Engine, Connection]) -> trino_dbapi.Connection:
         if isinstance(connection, Engine):
             return connection.raw_connection()
         return connection.connection
 
     def _get_default_catalog_name(self, connection: Connection) -> Optional[str]:
         dbapi_connection: trino_dbapi.Connection = self._raw_connection(connection)
@@ -323,7 +369,18 @@
     def _get_full_table(self, table_name: str, schema: str = None, quote: bool = True) -> str:
         table_part = self.identifier_preparer.quote_identifier(table_name) if quote else table_name
         if schema:
             schema_part = self.identifier_preparer.quote_identifier(schema) if quote else schema
             return f"{schema_part}.{table_part}"
 
         return table_part
+    
+    def has_table(self, connection: Connection, table_name: str, schema: str = None, **kw) -> bool:
+        get_table_names = self.get_table_names(connection, schema)
+        return len(get_table_names) > 0
+
+    def get_view_names(self, connection: Connection, schema: str = None, **kw) -> List[str]:
+        schema = schema or self._get_default_schema_name(connection)
+        if schema is None:
+            raise exc.NoSuchTableError("schema is required")
+
+        return []
```

### Comparing `pyextrica-17.2.0/pyextrica/sqlalchemy/error.py` & `pyextrica-17.2.1/pyextrica/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `pyextrica-17.2.0/pyextrica/sqlalchemy/util.py` & `pyextrica-17.2.1/pyextrica/sqlalchemy/util.py`

 * *Files identical despite different names*

### Comparing `pyextrica-17.2.0/pyextrica/transaction.py` & `pyextrica-17.2.1/pyextrica/transaction.py`

 * *Files identical despite different names*

### Comparing `pyextrica-17.2.0/pyextrica.egg-info/PKG-INFO` & `pyextrica-17.2.1/pyextrica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyextrica
-Version: 17.2.0
+Version: 17.2.1
 Summary: Python client library for Extrica
 Home-page: https://github.com/extricatrianz/pyextrica
 Author: Extrica Team
 Author-email: extricaproductionsupport@trianz.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,14 +25,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: backports.zoneinfo; python_version < "3.9"
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: requests>=2.31.0
 Requires-Dist: tzlocal
 Requires-Dist: sqlalchemy>=1.3
+Requires-Dist: sql_metadata==2.11.0
 Provides-Extra: all
 Requires-Dist: requests_kerberos; extra == "all"
 Requires-Dist: sqlalchemy>=1.3; extra == "all"
 Provides-Extra: kerberos
 Requires-Dist: requests_kerberos; extra == "kerberos"
 Provides-Extra: sqlalchemy
 Requires-Dist: sqlalchemy>=1.3; extra == "sqlalchemy"
@@ -46,15 +47,15 @@
 Requires-Dist: black; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Provides-Extra: external-authentication-token-cache
 Requires-Dist: keyring; extra == "external-authentication-token-cache"
 
 # PyExtrica Library for Extrica Product
 
-PyExtrica allows you to query and transform data in Extrica (Data To AI) platform directly without having to download the data locally. This library provides seamless access to the Extrica platform, allowing users to execute SQL queries and retrieve metadata such as catalog names, schema names, table names, and column information.
+PyExtrica allows you to query and transform data in [Extrica](https://extrica.ai/) (Data To AI) platform directly without having to download the data locally. This library provides seamless access to the Extrica platform, allowing users to execute SQL queries and retrieve metadata such as catalog names, schema names, table names, and column information.
 
 ## Getting Started
 
 ### Installation
 You can install PyExtrica via pip:
 
 ```bash
@@ -132,15 +133,15 @@
 print(joined_df.head())
 ```
 
 ### Available Methods
 PyExtrica provides the following methods for interacting with the Extrica platform:
 
 - extrica_engine: Connects to the Extrica platform.
-execute_sql_query: Executes SQL queries.
+- execute_sql_query: Executes SQL queries.
 - get_catalog_names: Retrieves catalog names. (Requires platform=data_products for data products or platform=data_sources for data sources). For data products, catalog name represents the domain name, and schema name represents the subdomain name. For data sources, it is similar to Trino catalog and schema.
 - get_schema_names: Retrieves schema names. (Requires platform=data_products for data products or platform=data_sources for data sources)
 - get_table_names: Retrieves table names. (Requires platform=data_products for data products or platform=data_sources for data sources)
 - get_table_columns: Retrieves column information for a specified table. (Requires platform=data_products for data products or platform=data_sources for data sources)
 
 ```python
 # Retrieve catalog names
```

### Comparing `pyextrica-17.2.0/pyextrica.egg-info/SOURCES.txt` & `pyextrica-17.2.1/pyextrica.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pyextrica/client.py
 pyextrica/constants.py
 pyextrica/dbapi.py
 pyextrica/exceptions.py
 pyextrica/extrica_rest_handler.py
 pyextrica/logging.py
 pyextrica/pyextrica_functions.py
+pyextrica/query_parser.py
 pyextrica/transaction.py
 pyextrica.egg-info/PKG-INFO
 pyextrica.egg-info/SOURCES.txt
 pyextrica.egg-info/dependency_links.txt
 pyextrica.egg-info/entry_points.txt
 pyextrica.egg-info/requires.txt
 pyextrica.egg-info/top_level.txt
```

### Comparing `pyextrica-17.2.0/setup.py` & `pyextrica-17.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,16 @@
     install_requires=[
         "backports.zoneinfo;python_version<'3.9'",
         "python-dateutil",
         "pytz",
         # requests CVE https://github.com/advisories/GHSA-j8r2-6x86-q33q
         "requests>=2.31.0",
         "tzlocal",
-        "sqlalchemy >= 1.3"
+        "sqlalchemy >= 1.3",
+        "sql_metadata==2.11.0"
     ],
     extras_require={
         "all": all_require,
         "kerberos": kerberos_require,
         "sqlalchemy": sqlalchemy_require,
         "tests": tests_require,
         "external-authentication-token-cache": external_authentication_token_cache_require,
```

