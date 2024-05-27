# Comparing `tmp/hermitage_alchemy-0.2.1.tar.gz` & `tmp/hermitage_alchemy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage_alchemy-0.2.1.tar", max compression
+gzip compressed data, was "hermitage_alchemy-0.2.2.tar", max compression
```

## Comparing `hermitage_alchemy-0.2.1.tar` & `hermitage_alchemy-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.2.1/README.md
--rw-r--r--   0        0        0      504 2024-05-25 14:24:50.954908 hermitage_alchemy-0.2.1/hermitage_alchemy/__init__.py
--rw-r--r--   0        0        0    10319 2024-05-25 14:24:50.955769 hermitage_alchemy-0.2.1/hermitage_alchemy/assembling.py
--rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.2.1/hermitage_alchemy/bootstraping.py
--rw-r--r--   0        0        0     6852 2024-05-25 14:24:50.956155 hermitage_alchemy-0.2.1/hermitage_alchemy/configuration.py
--rw-r--r--   0        0        0       24 2024-05-25 14:24:50.956586 hermitage_alchemy-0.2.1/hermitage_alchemy/definition/__init__.py
--rw-r--r--   0        0        0      718 2024-05-26 13:12:45.022518 hermitage_alchemy-0.2.1/hermitage_alchemy/definition/contracts.py
--rw-r--r--   0        0        0       60 2024-05-25 14:24:50.957143 hermitage_alchemy-0.2.1/hermitage_alchemy/execution/__init__.py
--rw-r--r--   0        0        0     6991 2024-05-25 14:24:50.957364 hermitage_alchemy-0.2.1/hermitage_alchemy/execution/read.py
--rw-r--r--   0        0        0     1165 2024-05-25 14:24:50.957584 hermitage_alchemy-0.2.1/hermitage_alchemy/execution/write.py
--rw-r--r--   0        0        0      438 2024-05-26 13:12:45.027432 hermitage_alchemy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 hermitage_alchemy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.2.2/README.md
+-rw-r--r--   0        0        0      504 2024-05-25 14:24:50.954908 hermitage_alchemy-0.2.2/hermitage_alchemy/__init__.py
+-rw-r--r--   0        0        0    10439 2024-05-27 14:15:43.102033 hermitage_alchemy-0.2.2/hermitage_alchemy/assembling.py
+-rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.2.2/hermitage_alchemy/bootstraping.py
+-rw-r--r--   0        0        0     6852 2024-05-25 14:24:50.956155 hermitage_alchemy-0.2.2/hermitage_alchemy/configuration.py
+-rw-r--r--   0        0        0       24 2024-05-25 14:24:50.956586 hermitage_alchemy-0.2.2/hermitage_alchemy/definition/__init__.py
+-rw-r--r--   0        0        0      718 2024-05-26 13:12:45.022518 hermitage_alchemy-0.2.2/hermitage_alchemy/definition/contracts.py
+-rw-r--r--   0        0        0       60 2024-05-25 14:24:50.957143 hermitage_alchemy-0.2.2/hermitage_alchemy/execution/__init__.py
+-rw-r--r--   0        0        0     6991 2024-05-25 14:24:50.957364 hermitage_alchemy-0.2.2/hermitage_alchemy/execution/read.py
+-rw-r--r--   0        0        0     1165 2024-05-25 14:24:50.957584 hermitage_alchemy-0.2.2/hermitage_alchemy/execution/write.py
+-rw-r--r--   0        0        0      438 2024-05-27 14:15:43.092735 hermitage_alchemy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 hermitage_alchemy-0.2.2/PKG-INFO
```

### Comparing `hermitage_alchemy-0.2.1/hermitage_alchemy/assembling.py` & `hermitage_alchemy-0.2.2/hermitage_alchemy/assembling.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,18 @@
             q = sqlalchemy.select(*self._select)
         elif self._values:
             if self._filters:
                 q = sqlalchemy.update(self._schema.get_table(Space(bucket.name))).values(self._values[0])
             else:
                 q = sqlalchemy.insert(self._schema.get_table(Space(bucket.name))).values(self._values)
         else:
-            q = sqlalchemy.delete(self._schema.get_table(Space(bucket.name)))
+            if self._filters:
+                q = sqlalchemy.delete(self._schema.get_table(Space(bucket.name)))
+            else:
+                raise ValueError("Cannot determine operation type")
 
         for join in self._joins:
             q = q.join_from(*join, isouter=True)
         for filter_clause in self._filters:
             q = q.where(filter_clause)
         for order_clause in self._orders:
             q = q.order_by(order_clause)
```

### Comparing `hermitage_alchemy-0.2.1/hermitage_alchemy/bootstraping.py` & `hermitage_alchemy-0.2.2/hermitage_alchemy/bootstraping.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.1/hermitage_alchemy/configuration.py` & `hermitage_alchemy-0.2.2/hermitage_alchemy/configuration.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.1/hermitage_alchemy/definition/contracts.py` & `hermitage_alchemy-0.2.2/hermitage_alchemy/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.1/hermitage_alchemy/execution/read.py` & `hermitage_alchemy-0.2.2/hermitage_alchemy/execution/read.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.1/hermitage_alchemy/execution/write.py` & `hermitage_alchemy-0.2.2/hermitage_alchemy/execution/write.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.1/PKG-INFO` & `hermitage_alchemy-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermitage-alchemy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Implementation of hermitage contracts for sqlalchemy engine
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

