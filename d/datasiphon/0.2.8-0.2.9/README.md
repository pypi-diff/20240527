# Comparing `tmp/datasiphon-0.2.8.tar.gz` & `tmp/datasiphon-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasiphon-0.2.8.tar", last modified: Tue May 21 10:35:57 2024, max compression
+gzip compressed data, was "datasiphon-0.2.9.tar", last modified: Tue May 21 11:04:05 2024, max compression
```

## Comparing `datasiphon-0.2.8.tar` & `datasiphon-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 10:35:57.502215 datasiphon-0.2.8/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 10:35:57.502215 datasiphon-0.2.8/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.8/README.md
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.8/pyproject.toml
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-21 10:35:57.502215 datasiphon-0.2.8/setup.cfg
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 10:35:57.500214 datasiphon-0.2.8/src/
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 10:35:57.501215 datasiphon-0.2.8/src/datasiphon.egg-info/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 10:35:57.000000 datasiphon-0.2.8/src/datasiphon.egg-info/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-21 10:35:57.000000 datasiphon-0.2.8/src/datasiphon.egg-info/SOURCES.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-21 10:35:57.000000 datasiphon-0.2.8/src/datasiphon.egg-info/dependency_links.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-21 10:35:57.000000 datasiphon-0.2.8/src/datasiphon.egg-info/requires.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-21 10:35:57.000000 datasiphon-0.2.8/src/datasiphon.egg-info/top_level.txt
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 10:35:57.501215 datasiphon-0.2.8/src/siphon/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-21 10:35:14.000000 datasiphon-0.2.8/src/siphon/__init__.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      397 2024-05-21 07:52:31.000000 datasiphon-0.2.8/src/siphon/base.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:15:29.000000 datasiphon-0.2.8/src/siphon/nosql.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    38269 2024-05-21 10:35:18.000000 datasiphon-0.2.8/src/siphon/sql.py
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 10:35:57.501215 datasiphon-0.2.8/tests/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    28784 2024-05-21 10:35:16.000000 datasiphon-0.2.8/tests/test_sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 11:04:05.096030 datasiphon-0.2.9/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 11:04:05.095030 datasiphon-0.2.9/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.9/README.md
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.9/pyproject.toml
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-21 11:04:05.096030 datasiphon-0.2.9/setup.cfg
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 11:04:05.094030 datasiphon-0.2.9/src/
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 11:04:05.095030 datasiphon-0.2.9/src/datasiphon.egg-info/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 11:04:05.000000 datasiphon-0.2.9/src/datasiphon.egg-info/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-21 11:04:05.000000 datasiphon-0.2.9/src/datasiphon.egg-info/SOURCES.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-21 11:04:05.000000 datasiphon-0.2.9/src/datasiphon.egg-info/dependency_links.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-21 11:04:05.000000 datasiphon-0.2.9/src/datasiphon.egg-info/requires.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-21 11:04:05.000000 datasiphon-0.2.9/src/datasiphon.egg-info/top_level.txt
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 11:04:05.095030 datasiphon-0.2.9/src/siphon/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-21 11:03:52.000000 datasiphon-0.2.9/src/siphon/__init__.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      397 2024-05-21 07:52:31.000000 datasiphon-0.2.9/src/siphon/base.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:15:29.000000 datasiphon-0.2.9/src/siphon/nosql.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    38989 2024-05-21 11:02:49.000000 datasiphon-0.2.9/src/siphon/sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 11:04:05.095030 datasiphon-0.2.9/tests/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    29299 2024-05-21 11:01:41.000000 datasiphon-0.2.9/tests/test_sql.py
```

### Comparing `datasiphon-0.2.8/PKG-INFO` & `datasiphon-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.8
+Version: 0.2.9
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.8/README.md` & `datasiphon-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.8/pyproject.toml` & `datasiphon-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.8/src/datasiphon.egg-info/PKG-INFO` & `datasiphon-0.2.9/src/datasiphon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.8
+Version: 0.2.9
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.8/src/siphon/nosql.py` & `datasiphon-0.2.9/src/siphon/nosql.py`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.8/src/siphon/sql.py` & `datasiphon-0.2.9/src/siphon/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -539,14 +539,30 @@
     def to_op(self, original_op: str) -> Operation:
         self.used = True
         if self.operation is None:
             self.operation = original_op
         return FilterBuilder.op_mapping[self.operation](self.column, self.value)
 
 
+@dataclass(init=False)
+class Removal:
+    operation: str | None
+    column: str
+
+    def __init__(self, column: str, operation: str = None):
+        self.column = column
+        self.operation = operation
+
+    def has_operation(self) -> bool:
+        return self.operation is not None
+
+    def is_correct_op(self, op: str) -> bool:
+        return self.operation == op
+
+
 class PaginationBuilder:
     base_query: sa.Select
     sql_operators_mapping: dict[sql_operators.OperatorType, t.Type[Operation] | str] = {
         sql_operators.eq: Eq,
         sql_operators.ne: Ne,
         sql_operators.gt: Gt,
         sql_operators.ge: Ge,
@@ -563,27 +579,34 @@
     }
 
     def __init__(self, base_query: sa.Select):
         self.base_query = base_query
 
     @staticmethod
     def process_operation(
-        whereclause: sql_elements.BinaryExpression, substition: list[Substitution], bindparams: dict, removals: dict
+        whereclause: sql_elements.BinaryExpression,
+        substition: list[Substitution],
+        bindparams: dict,
+        removals: list[Removal],
     ) -> Operation | None:
         column = PaginationBuilder.get_column_from_binary_expression(whereclause)
         for item in substition:
             if item.used:
                 continue
             if item.column == column:
                 return item.to_op(PaginationBuilder.sql_operators_mapping[whereclause.operator].name)
-        if (
-            column in removals
-            and removals[column] == PaginationBuilder.sql_operators_mapping[whereclause.operator].name
-        ):
-            return None
+        for item in removals:
+            if item.column == column:
+                # if removal has set operation, remove this operation only if it matches
+                # otherwise, remove all operations for this column
+                if item.has_operation() and not item.is_correct_op(
+                    PaginationBuilder.sql_operators_mapping[whereclause.operator].name
+                ):
+                    continue
+                return None
 
         expr_value = PaginationBuilder.get_value_from_binary_expression(whereclause)
         if not isinstance(expr_value, sql_elements.BindParameter):
             raise TypeError(f"Invalid type: {type(expr_value)} for value")
         processed_expr_value = bindparams.get(column, expr_value.value)
         return PaginationBuilder.sql_operators_mapping[whereclause.operator](column, processed_expr_value)
 
@@ -679,15 +702,15 @@
             else:
                 post_processed_data[unique_col].update(
                     {junction: {operation.name: operation.value} for operation in operations}
                 )
         return post_processed_data
 
     def reconstruct_filter(
-        self, substitution: list[Substitution] = None, bindparams: dict = None, removals: dict = None
+        self, substitution: list[Substitution] = None, bindparams: dict = None, removals: list[Removal] = None
     ) -> dict:
         """
         Reconstruct the filter into a nested dictionary from query - parsable by this package
 
         :param substitution: The substitutions to apply if the substitutions are not used, they are added to the result
         :param bindparams: The bindparams to apply - from prepared statement NOTE warning: if bindparams are used and not provided
         `None` value will be used in reconstructed filter
@@ -708,19 +731,22 @@
                             f"Column not used in filter and operation for substitution not provided: {item}"
                         )
                     data[item.column] = {item.operation: item.value}
         return data
 
     @staticmethod
     def recursive_reconstruct_filter(
-        whereclause: t.Any, substitution: list[Substitution] = None, bindparams: dict = None, removals: dict = None
+        whereclause: t.Any,
+        substitution: list[Substitution] = None,
+        bindparams: dict = None,
+        removals: list[Removal] = None,
     ) -> dict:
         processed_substitution = substitution or []
         processed_bindparams = bindparams or {}
-        processed_removals = removals or {}
+        processed_removals = removals or []
         if whereclause is None:
             return None
         if isinstance(whereclause, sql_elements.BinaryExpression):
             operation = PaginationBuilder.process_operation(
                 whereclause, processed_substitution, processed_bindparams, processed_removals
             )
             return operation
@@ -780,23 +806,23 @@
         if whereclause is None:
             return None
         if isinstance(whereclause, sql_elements.BinaryExpression):
             if column_name in [
                 self.get_column_from_binary_expression(whereclause),
                 self.get_column_from_binary_expression(whereclause),
             ]:
-                return self.process_operation(whereclause, {}, {}, {})
+                return self.process_operation(whereclause, [], {}, [])
         elif isinstance(whereclause, sql_elements.BooleanClauseList):
             for clause in whereclause.clauses:
                 if isinstance(clause, sql_elements.BinaryExpression):
                     if column_name in [
                         self.get_column_from_binary_expression(clause),
                         self.get_column_from_binary_expression(clause),
                     ]:
-                        return self.process_operation(clause, {}, {}, {})
+                        return self.process_operation(clause, [], {}, [])
         return None
 
 
 class SQL(QueryBuilder):
     """
     SQL query builder
     """
```

### Comparing `datasiphon-0.2.8/tests/test_sql.py` & `datasiphon-0.2.9/tests/test_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -663,25 +663,37 @@
                     data.table_with_time_stamp.c.name == "Peter",
                 )
             ),
         )
 
         # test reconstruct with removal
         result = ds.sql.PaginationBuilder(second_sample_query).reconstruct_filter(
-            removals={"name": "eq"}, bindparams={"created_at": "2021-01-01T12:00:00"}
+            removals=[ds.sql.Removal("name")], bindparams={"created_at": "2021-01-01T12:00:00"}
         )
         self.assertEqual(
             str(ds.sql.SQL.build(data.table_with_time_stamp.select(), result)),
             str(
                 data.table_with_time_stamp.select().where(
                     data.table_with_time_stamp.c.created_at == "2021-01-01T12:00:00",
                 )
             ),
         )
 
+        not_affected_query = data.table_with_time_stamp.select().where(
+            data.table_with_time_stamp.c.name == "John",
+        )
+        # test reconstruct with removal but doesnt affect anything
+        result = ds.sql.PaginationBuilder(not_affected_query).reconstruct_filter(
+            removals=[ds.sql.Removal("name", "gt")],
+        )
+        self.assertEqual(
+            str(ds.sql.SQL.build(data.table_with_time_stamp.select(), result)),
+            str(not_affected_query),
+        )
+
         # test retrieve order_by
         sample_query = data.table_with_time_stamp.select().order_by(data.table_with_time_stamp.c.created_at.desc())
         result = ds.sql.PaginationBuilder(sample_query).retrieve_order_by()
         self.assertEqual(len(result), 1)
         self.assertEqual(result[0], (0, "created_at"))
 
         # test order by with different approach
```

