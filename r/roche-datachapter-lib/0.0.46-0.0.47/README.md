# Comparing `tmp/roche_datachapter_lib-0.0.46.tar.gz` & `tmp/roche_datachapter_lib-0.0.47.tar.gz`

## Comparing `roche_datachapter_lib-0.0.46.tar` & `roche_datachapter_lib-0.0.47.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/requirements_for_build.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/requirements_for_test.txt
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/setup_build_upload.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/__domain__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/__init__.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/data_transformer.py
--rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/db_config.py
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/google_services.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/google_services_enums.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/job_manager.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/logger.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/query_manager.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/result_type.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/tests/simple_test.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/tests/test_db_config.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/tests/test_google_services.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/tests/test_job_manager.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/tests/test_query_manager.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/tests/test_redshift_connection.py
--rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/tests/queries/ej_godw.sql
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/tests/queries/ej_rexis.sql
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/tests/queries/ej_sap.sql
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/tests/queries/ej_sql_server.sql
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/tests/queries/stock_sap.sql
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/LICENSE
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/README.md
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/pyproject.toml
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.46/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/requirements_for_build.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/requirements_for_test.txt
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/setup_build_upload.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/__domain__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/data_transformer.py
+-rw-r--r--   0        0        0     8533 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/db_config.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/google_services.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/google_services_enums.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/job_manager.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/logger.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/query_manager.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/result_type.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/tests/simple_test.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/tests/test_db_config.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/tests/test_google_services.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/tests/test_job_manager.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/tests/test_query_manager.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/tests/test_redshift_connection.py
+-rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/tests/queries/ej_godw.sql
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/tests/queries/ej_rexis.sql
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/tests/queries/ej_sap.sql
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/tests/queries/ej_sql_server.sql
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/tests/queries/stock_sap.sql
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/LICENSE
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/README.md
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/pyproject.toml
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.47/PKG-INFO
```

### Comparing `roche_datachapter_lib-0.0.46/setup_build_upload.py` & `roche_datachapter_lib-0.0.47/setup_build_upload.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/__domain__.py` & `roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/__domain__.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/data_transformer.py` & `roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/data_transformer.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/db_config.py` & `roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/db_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .result_type import ResultType
 
 ENV_VAR_NAMES = ["SQLSERVER_SERVER", "SQLSERVER_USER", "SQLSERVER_PWD",
                  "SQLSERVER_LATAM_AR_DB", "SQLSERVER_LATAM_AR_DEV_DB",
                  "SQLSERVER_LATAM_AR_FARMADB_DB", "SQLSERVER_LATAM_AR_SAND_DB",
                  "SQLSERVER_LATAM_AR_STAGING_DB", "SQLSERVER_LATAM_UY_DB",
                  "SQLSERVER_LATAM_UY_STAGING_DB", "GODW_SERVER", "GODW_PORT",
-                 "GODW_USER", "GODW_PASSWORD", "GODW_SERVICENAME", "GODW_ORACLE_INSTANT_CLIENT_PATH",
+                 "GODW_USER", "GODW_PASSWORD", "GODW_SERVICENAME",
                  "SAPDWP06_SERVER", "SAPDWP06_PORT", "SAPDWP06_USER", "SAPDWP06_PASSWORD", "SAPDWP06_DB",
                  "REXIS_SALES_SERVER", "REXIS_SALES_DB", "REXIS_SERVICES_SERVER", "REXIS_SERVICES_DB",
                  "NEXUS_HOST", "NEXUS_DB", "NEXUS_PORT", "NEXUS_USER", "NEXUS_PASSWORD",
                  "RDI_LATAM_AR_USER", "RDI_LATAM_AR_PASSWORD", "RDI_LATAM_AR_HOST",
                  "RDI_LATAM_AR_PORT", "RDI_LATAM_AR_DB"]
 
 for env_var_name in ENV_VAR_NAMES:
```

### Comparing `roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/google_services.py` & `roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/google_services.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/job_manager.py` & `roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/job_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/logger.py` & `roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/logger.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/src/roche_datachapter_lib/query_manager.py` & `roche_datachapter_lib-0.0.47/src/roche_datachapter_lib/query_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/tests/test_google_services.py` & `roche_datachapter_lib-0.0.47/tests/test_google_services.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/tests/test_job_manager.py` & `roche_datachapter_lib-0.0.47/tests/test_job_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/tests/test_redshift_connection.py` & `roche_datachapter_lib-0.0.47/tests/test_redshift_connection.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/tests/queries/ej_godw.sql` & `roche_datachapter_lib-0.0.47/tests/queries/ej_godw.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/tests/queries/ej_sap.sql` & `roche_datachapter_lib-0.0.47/tests/queries/ej_sap.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/tests/queries/ej_sql_server.sql` & `roche_datachapter_lib-0.0.47/tests/queries/ej_sql_server.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/tests/queries/stock_sap.sql` & `roche_datachapter_lib-0.0.47/tests/queries/stock_sap.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/.gitignore` & `roche_datachapter_lib-0.0.47/.gitignore`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/LICENSE` & `roche_datachapter_lib-0.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/README.md` & `roche_datachapter_lib-0.0.47/README.md`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.46/pyproject.toml` & `roche_datachapter_lib-0.0.47/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "roche_datachapter_lib"
-version = "0.0.46"
+version = "0.0.47"
 authors = [{ name = "Lucas Frías", email = "lucasmatiasfrias@live.com" }]
 description = "Esta biblioteca de código esta pensada para compartir funcionalidades entre todos los procesos ETL que desarrollemos con Python"
 readme = "README.md"
 requires-python = ">=3.12"
 dependencies = [
     "Flask==2.3.1",
     "Flask-SQLAlchemy==3.0.3",
```

### Comparing `roche_datachapter_lib-0.0.46/PKG-INFO` & `roche_datachapter_lib-0.0.47/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: roche_datachapter_lib
-Version: 0.0.46
+Version: 0.0.47
 Summary: Esta biblioteca de código esta pensada para compartir funcionalidades entre todos los procesos ETL que desarrollemos con Python
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Lucas Frías <lucasmatiasfrias@live.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

