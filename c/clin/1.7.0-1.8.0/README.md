# Comparing `tmp/clin-1.7.0.tar.gz` & `tmp/clin-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clin-1.7.0.tar", max compression
+gzip compressed data, was "clin-1.8.0.tar", max compression
```

## Comparing `clin-1.7.0.tar` & `clin-1.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1078 2024-02-05 11:01:03.989529 clin-1.7.0/LICENSE
--rw-r--r--   0        0        0     2389 2024-02-05 11:01:03.989529 clin-1.7.0/README.md
--rw-r--r--   0        0        0       22 2024-02-05 11:01:13.025464 clin-1.7.0/clin/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 11:01:03.989529 clin-1.7.0/clin/clients/__init__.py
--rw-r--r--   0        0        0     3302 2024-02-05 11:01:03.989529 clin-1.7.0/clin/clients/http_client.py
--rw-r--r--   0        0        0     8524 2024-02-05 11:01:03.989529 clin-1.7.0/clin/clients/nakadi.py
--rw-r--r--   0        0        0     5201 2024-02-05 11:01:03.989529 clin-1.7.0/clin/clients/nakadi_sql.py
--rw-r--r--   0        0        0     2251 2024-02-05 11:01:03.989529 clin-1.7.0/clin/clinfile.py
--rw-r--r--   0        0        0     1903 2024-02-05 11:01:03.989529 clin-1.7.0/clin/config.py
--rw-r--r--   0        0        0        0 2024-02-05 11:01:03.989529 clin-1.7.0/clin/models/__init__.py
--rw-r--r--   0        0        0     2323 2024-02-05 11:01:03.989529 clin-1.7.0/clin/models/auth.py
--rw-r--r--   0        0        0     2340 2024-02-05 11:01:03.989529 clin-1.7.0/clin/models/event_type.py
--rw-r--r--   0        0        0     4428 2024-02-05 11:01:03.989529 clin-1.7.0/clin/models/shared.py
--rw-r--r--   0        0        0     2792 2024-02-05 11:01:03.989529 clin-1.7.0/clin/models/sql_query.py
--rw-r--r--   0        0        0     1502 2024-02-05 11:01:03.989529 clin-1.7.0/clin/models/subscription.py
--rw-r--r--   0        0        0    10250 2024-02-05 11:01:03.989529 clin-1.7.0/clin/processor.py
--rw-r--r--   0        0        0     6852 2024-02-05 11:01:03.989529 clin-1.7.0/clin/run.py
--rw-r--r--   0        0        0     2254 2024-02-05 11:01:03.989529 clin-1.7.0/clin/utils.py
--rw-r--r--   0        0        0     5526 2024-02-05 11:01:03.989529 clin-1.7.0/clin/yamlops.py
--rw-r--r--   0        0        0      949 2024-02-05 11:01:12.989464 clin-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 clin-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-27 13:44:30.140195 clin-1.8.0/LICENSE
+-rw-r--r--   0        0        0     2389 2024-05-27 13:44:30.140195 clin-1.8.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-27 13:44:43.688204 clin-1.8.0/clin/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:44:30.140195 clin-1.8.0/clin/clients/__init__.py
+-rw-r--r--   0        0        0     3302 2024-05-27 13:44:30.140195 clin-1.8.0/clin/clients/http_client.py
+-rw-r--r--   0        0        0     8524 2024-05-27 13:44:30.140195 clin-1.8.0/clin/clients/nakadi.py
+-rw-r--r--   0        0        0     5201 2024-05-27 13:44:30.140195 clin-1.8.0/clin/clients/nakadi_sql.py
+-rw-r--r--   0        0        0     2251 2024-05-27 13:44:30.140195 clin-1.8.0/clin/clinfile.py
+-rw-r--r--   0        0        0     1903 2024-05-27 13:44:30.140195 clin-1.8.0/clin/config.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:44:30.140195 clin-1.8.0/clin/models/__init__.py
+-rw-r--r--   0        0        0     2323 2024-05-27 13:44:30.140195 clin-1.8.0/clin/models/auth.py
+-rw-r--r--   0        0        0     2340 2024-05-27 13:44:30.140195 clin-1.8.0/clin/models/event_type.py
+-rw-r--r--   0        0        0     4478 2024-05-27 13:44:30.140195 clin-1.8.0/clin/models/shared.py
+-rw-r--r--   0        0        0     2792 2024-05-27 13:44:30.140195 clin-1.8.0/clin/models/sql_query.py
+-rw-r--r--   0        0        0     1502 2024-05-27 13:44:30.140195 clin-1.8.0/clin/models/subscription.py
+-rw-r--r--   0        0        0    10250 2024-05-27 13:44:30.140195 clin-1.8.0/clin/processor.py
+-rw-r--r--   0        0        0     6852 2024-05-27 13:44:30.140195 clin-1.8.0/clin/run.py
+-rw-r--r--   0        0        0     2254 2024-05-27 13:44:30.140195 clin-1.8.0/clin/utils.py
+-rw-r--r--   0        0        0     5526 2024-05-27 13:44:30.140195 clin-1.8.0/clin/yamlops.py
+-rw-r--r--   0        0        0      949 2024-05-27 13:44:43.652204 clin-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 clin-1.8.0/PKG-INFO
```

### Comparing `clin-1.7.0/LICENSE` & `clin-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/README.md` & `clin-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/clients/http_client.py` & `clin-1.8.0/clin/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/clients/nakadi.py` & `clin-1.8.0/clin/clients/nakadi.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/clients/nakadi_sql.py` & `clin-1.8.0/clin/clients/nakadi_sql.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/clinfile.py` & `clin-1.8.0/clin/clinfile.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/config.py` & `clin-1.8.0/clin/config.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/models/auth.py` & `clin-1.8.0/clin/models/auth.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/models/event_type.py` & `clin-1.8.0/clin/models/event_type.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/models/shared.py` & `clin-1.8.0/clin/models/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 
 @dataclass
 class Cleanup:
     @unique
     class Policy(str, Enum):
         DELETE = "delete"
         COMPACT = "compact"
+        COMPACT_AND_DELETE = "compact_and_delete"
 
         def __str__(self) -> str:
             return str(self.value)
 
     policy: Policy
     retention_time_days: int
```

### Comparing `clin-1.7.0/clin/models/sql_query.py` & `clin-1.8.0/clin/models/sql_query.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/models/subscription.py` & `clin-1.8.0/clin/models/subscription.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/processor.py` & `clin-1.8.0/clin/processor.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/run.py` & `clin-1.8.0/clin/run.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/utils.py` & `clin-1.8.0/clin/utils.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/clin/yamlops.py` & `clin-1.8.0/clin/yamlops.py`

 * *Files identical despite different names*

### Comparing `clin-1.7.0/pyproject.toml` & `clin-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clin"
-version = "1.7.0"
+version = "1.8.0"
 description = "Cli for Nakadi resources management in Infrastructure as Code style"
 homepage = "https://github.com/zalando-incubator/clin"
 license = "MIT"
 readme = "README.md"
 
 authors = [
     "Dmitry Erokhin <dmitry.erokhin@zalando.de>",
@@ -29,15 +29,15 @@
 deepdiff = "^6.7"
 pygments = "^2.17"
 colorama = "^0.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 toml = "^0.10"
-black = "^22.6"
+black = "^23.3"
 
 [tool.poetry.scripts]
 clin = "clin.run:cli"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `clin-1.7.0/PKG-INFO` & `clin-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clin
-Version: 1.7.0
+Version: 1.8.0
 Summary: Cli for Nakadi resources management in Infrastructure as Code style
 Home-page: https://github.com/zalando-incubator/clin
 License: MIT
 Keywords: Nakadi
 Author: Dmitry Erokhin
 Author-email: dmitry.erokhin@zalando.de
 Requires-Python: >=3.7,<4.0
```

