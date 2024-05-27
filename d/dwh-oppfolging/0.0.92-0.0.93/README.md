# Comparing `tmp/dwh_oppfolging-0.0.92.tar.gz` & `tmp/dwh_oppfolging-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwh_oppfolging-0.0.92.tar", max compression
+gzip compressed data, was "dwh_oppfolging-0.0.93.tar", max compression
```

## Comparing `dwh_oppfolging-0.0.92.tar` & `dwh_oppfolging-0.0.93.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/LICENSE
--rw-r--r--   0        0        0      325 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/README.md
--rw-r--r--   0        0        0       22 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/README.md
--rw-r--r--   0        0        0        0 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/__init__.py
--rw-r--r--   0        0        0       14 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/airflow_api_v1.py
--rw-r--r--   0        0        0     8543 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/brreg_api_v1.py
--rw-r--r--   0        0        0     4051 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/brreg_api_v1_types.py
--rw-r--r--   0        0        0    17798 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/brreg_api_v2.py
--rw-r--r--   0        0        0     2297 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/dbt_oracle_api_v1.py
--rw-r--r--   0        0        0      422 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/generic_api_v1.py
--rw-r--r--   0        0        0      741 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/kafka_api_v1.py
--rw-r--r--   0        0        0    24608 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/kafka_api_v1_types.py
--rw-r--r--   0        0        0    11838 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/oracle_api_v1.py
--rw-r--r--   0        0        0      125 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/oracle_api_v1_types.py
--rw-r--r--   0        0        0     2371 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/secrets_api_v1.py
--rw-r--r--   0        0        0     6831 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/ssb_api_v1.py
--rw-r--r--   0        0        0    11693 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/ssb_api_v1_types.py
--rw-r--r--   0        0        0        0 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/transforms/__init__.py
--rw-r--r--   0        0        0     9224 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/transforms/datatypes.py
--rw-r--r--   0        0        0     9521 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/transforms/functions.py
--rw-r--r--   0        0        0     1661 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/pyproject.toml
--rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.92/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/LICENSE
+-rw-r--r--   0        0        0      325 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/README.md
+-rw-r--r--   0        0        0       22 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/__init__.py
+-rw-r--r--   0        0        0       14 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/airflow_api_v1.py
+-rw-r--r--   0        0        0     8543 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/brreg_api_v1.py
+-rw-r--r--   0        0        0     4051 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/brreg_api_v1_types.py
+-rw-r--r--   0        0        0    17798 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/brreg_api_v2.py
+-rw-r--r--   0        0        0     2297 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/dbt_oracle_api_v1.py
+-rw-r--r--   0        0        0      422 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/generic_api_v1.py
+-rw-r--r--   0        0        0      741 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/kafka_api_v1.py
+-rw-r--r--   0        0        0    24608 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/kafka_api_v1_types.py
+-rw-r--r--   0        0        0    11838 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/oracle_api_v1.py
+-rw-r--r--   0        0        0      125 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/oracle_api_v1_types.py
+-rw-r--r--   0        0        0     2371 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/secrets_api_v1.py
+-rw-r--r--   0        0        0     6831 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/ssb_api_v1.py
+-rw-r--r--   0        0        0    11843 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/ssb_api_v1_types.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/transforms/__init__.py
+-rw-r--r--   0        0        0     9224 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/transforms/datatypes.py
+-rw-r--r--   0        0        0     9521 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/transforms/functions.py
+-rw-r--r--   0        0        0     1644 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/pyproject.toml
+-rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.93/PKG-INFO
```

### Comparing `dwh_oppfolging-0.0.92/LICENSE` & `dwh_oppfolging-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/brreg_api_v1.py` & `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/brreg_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/brreg_api_v1_types.py` & `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/brreg_api_v1_types.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/brreg_api_v2.py` & `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/brreg_api_v2.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/dbt_oracle_api_v1.py` & `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/dbt_oracle_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/kafka_api_v1.py` & `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/kafka_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/kafka_api_v1_types.py` & `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/kafka_api_v1_types.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/oracle_api_v1.py` & `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/oracle_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/secrets_api_v1.py` & `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/secrets_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/ssb_api_v1.py` & `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/ssb_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/ssb_api_v1_types.py` & `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/ssb_api_v1_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,17 +58,17 @@
     """Link to source version"""
     target_url: str
     """Link to target version"""
 
     @classmethod
     def from_json(cls, data: dict):
         """Constructs CorrespondenceHeader from an entry in the json-version's correspondenceTables"""
-        self_url = data["_links"]["self"]["href"]
-        source_url = data["_links"]["source"]["href"]
-        target_url = data["_links"]["target"]["href"]
+        self_url = data["_links"]["self"]["href"].replace("http", "https")
+        source_url = data["_links"]["source"]["href"].replace("http", "https")
+        target_url = data["_links"]["target"]["href"].replace("http", "https")
         last_modified = string_to_naive_norwegian_datetime(data["lastModified"])
         return CorrespondenceHeader(
             data["name"], data["owningSection"], data["source"], data["sourceId"], data["target"],
             data["targetId"], data["changeTable"], last_modified, self_url, source_url, target_url
         )
 
 
@@ -137,15 +137,15 @@
     """URL to full version data"""
     version_id: int
     """Version identifier"""
 
     @classmethod
     def from_json(cls, data: dict) -> Self:
         """Constructs VersionHeader from an entry in the json-classification's versions list"""
-        url: str = data["_links"]["self"]["href"]
+        url: str = data["_links"]["self"]["href"].replace("http", "https")
         version_id: int = int(url[url.rfind("/")+1:])
         #valid_from = string_to_naive_norwegian_datetime(data["validFrom"])
         #valid_to = string_to_naive_norwegian_datetime(data["validTo"]) if "validTo" in data else None
         # trunc valid dates, these are in form yyyy-mm-dd, and should not have time of day
         valid_from = datetime.strptime(data["validFrom"], _VALID_DATE_FMT)
         valid_to = datetime.strptime(data["validTo"], _VALID_DATE_FMT) if "validTo" in data else None
         last_modified = string_to_naive_norwegian_datetime(data["lastModified"])
@@ -174,15 +174,15 @@
     """Classification identifier"""
 
     @classmethod
     def from_json(cls, data: dict) -> Self:
         """Constructs Classification from json-classification"""
         versions = [VersionHeader.from_json(version) for version in data["versions"]]
         last_modified =  string_to_naive_norwegian_datetime(data["lastModified"])
-        url = data["_links"]["self"]["href"]
+        url = data["_links"]["self"]["href"].replace("http", "https")
         classification_id = int(url[url.rindex("/") + 1 :])
         return cls(
             data["name"], last_modified, data["description"],
             data["includeShortName"], data["includeNotes"], data["statisticalUnits"],
             data["owningSection"], versions, classification_id
         )
     
@@ -226,15 +226,15 @@
         last_modified = string_to_naive_norwegian_datetime(data["lastModified"])
         #valid_from = string_to_naive_norwegian_datetime(data["validFrom"])
         #valid_to = string_to_naive_norwegian_datetime(data["validTo"]) if "validTo" in data else None
         # trunc valid dates, these are in form yyyy-mm-dd, and should not have time of day
         valid_from = datetime.strptime(data["validFrom"], _VALID_DATE_FMT)
         valid_to = datetime.strptime(data["validTo"], _VALID_DATE_FMT) if "validTo" in data else None
         corr_tables = [CorrespondenceHeader.from_json(corr) for corr in data["correspondenceTables"]]
-        url = data["_links"]["self"]["href"]
+        url = data["_links"]["self"]["href"].replace("http", "https")
         version_id = int(url[url.rindex("/") + 1 :])
         return cls(
             data["name"], valid_from, valid_to, last_modified, data["introduction"], classification_id,
             version_id, data["owningSection"], data.get("derivedFrom"), data.get("changelogs"), data["levels"],
             data["classificationItems"], corr_tables
             )
```

### Comparing `dwh_oppfolging-0.0.92/dwh_oppfolging/transforms/datatypes.py` & `dwh_oppfolging-0.0.93/dwh_oppfolging/transforms/datatypes.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.92/dwh_oppfolging/transforms/functions.py` & `dwh_oppfolging-0.0.93/dwh_oppfolging/transforms/functions.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.92/pyproject.toml` & `dwh_oppfolging-0.0.93/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "dwh-oppfolging"
-version = "0.0.92"
+version = "0.0.93"
 description = "Oppfolging python package for DWH ETL"
 authors = ["Team Oppfølging"]
 packages = [{include = "dwh_oppfolging"}]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "3.11.*"       # python 3.12 mangler distutils, som ødelegger installasjon av pendulum 2.1.2
                         # derfor låser vi oss til python 3.11
-requests = "2.31.0"
+requests = "2.32.2"
 pendulum = "3.0.0"      # fjernet airflow/dataverk i dev fordi den bruker en eldgammel versjon av pendulum
 ijson = "3.2.3"
-oracledb = "2.1.2"      # versjonen her begrenses av dbt-oracle, så dbt-oracle må oppgraderes først
-dbt-oracle = "1.7.4"    # denne krever cx_Oracle 8.3, som vi ikke klarer å bygge uten gcc
+oracledb = "2.2.0"      # versjonen her begrenses av dbt-oracle, så dbt-oracle må oppgraderes først
+dbt-oracle = "1.7.5"    # denne krever cx_Oracle 8.3, som vi ikke klarer å bygge uten gcc
                         # 3.11-slim har ikke gcc, men 3.11 har det, men den er +700 MB..
-google-cloud-secret-manager = "2.19.0"
-confluent-kafka = "2.3.0"
+google-cloud-secret-manager = "2.20.0"
+confluent-kafka = "2.4.0"
 fastavro = "1.9.4"
 
 [tool.poetry.group.dev.dependencies]
-black = "24.2.0"
-mypy = "1.8.0"
-pylint = "3.0.3"
-pytest = "8.0.1"
+black = "*"
+mypy = "*"
+pylint = "*"
+pytest = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # [tool.sqlfluff.core]
 # dialect = "oracle"
```

### Comparing `dwh_oppfolging-0.0.92/PKG-INFO` & `dwh_oppfolging-0.0.93/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dwh-oppfolging
-Version: 0.0.92
+Version: 0.0.93
 Summary: Oppfolging python package for DWH ETL
 Author: Team Oppfølging
 Requires-Python: ==3.11.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: confluent-kafka (==2.3.0)
-Requires-Dist: dbt-oracle (==1.7.4)
+Requires-Dist: confluent-kafka (==2.4.0)
+Requires-Dist: dbt-oracle (==1.7.5)
 Requires-Dist: fastavro (==1.9.4)
-Requires-Dist: google-cloud-secret-manager (==2.19.0)
+Requires-Dist: google-cloud-secret-manager (==2.20.0)
 Requires-Dist: ijson (==3.2.3)
-Requires-Dist: oracledb (==2.1.2)
+Requires-Dist: oracledb (==2.2.0)
 Requires-Dist: pendulum (==3.0.0)
-Requires-Dist: requests (==2.31.0)
+Requires-Dist: requests (==2.32.2)
 Description-Content-Type: text/markdown
 
 # dwh-oppfolging
 Public repository for the development of the dwh-oppfolging python package.
 
 ## Installation
 `pip install dwh-oppfolging`
```

