# Comparing `tmp/pysquril-0.6.2.tar.gz` & `tmp/pysquril-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysquril-0.6.2.tar", max compression
+gzip compressed data, was "pysquril-0.7.0.tar", max compression
```

## Comparing `pysquril-0.6.2.tar` & `pysquril-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      179 2024-04-10 11:04:36.758264 pysquril-0.6.2/README.md
--rw-r--r--   0        0        0      539 2024-04-10 11:04:36.758264 pysquril-0.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/__init__.py
--rw-r--r--   0        0        0    34186 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/backends.py
--rw-r--r--   0        0        0      412 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/exc.py
--rw-r--r--   0        0        0    24631 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/generator.py
--rw-r--r--   0        0        0    14457 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/parser.py
--rw-r--r--   0        0        0     2482 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/test_data.py
--rw-r--r--   0        0        0    33976 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/tests.py
--rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 pysquril-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     3262 2024-05-27 10:01:31.474077 pysquril-0.7.0/README.md
+-rw-r--r--   0        0        0      539 2024-05-27 10:01:31.474077 pysquril-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/__init__.py
+-rw-r--r--   0        0        0    38193 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/backends.py
+-rw-r--r--   0        0        0      412 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/exc.py
+-rw-r--r--   0        0        0    25460 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/generator.py
+-rw-r--r--   0        0        0     2423 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/interactive.py
+-rw-r--r--   0        0        0    15251 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/parser.py
+-rw-r--r--   0        0        0     2629 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/test_data.py
+-rw-r--r--   0        0        0    35659 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/tests.py
+-rw-r--r--   0        0        0      406 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/utils.py
+-rw-r--r--   0        0        0     3999 1970-01-01 00:00:00.000000 pysquril-0.7.0/PKG-INFO
```

### Comparing `pysquril-0.6.2/pyproject.toml` & `pysquril-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysquril"
-version = "0.6.2"
+version = "0.7.0"
 description = "Python implementation of structured URI query language"
 readme = "README.md"
 repository = "https://github.com/unioslo/pysquril"
 authors = [
     "Leon du Toit <l.c.d.toit@usit.uio.no>",
     "Eirik Haatveit <haatveit@uio.no>",
 ]
```

### Comparing `pysquril-0.6.2/pysquril/backends.py` & `pysquril-0.7.0/pysquril/backends.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 
 import datetime
 import json
 import logging
 import sqlite3
+import uuid
 
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from datetime import timedelta
 from typing import Union, ContextManager, Iterable, Optional, Any, Callable
 from urllib.parse import unquote
 from uuid import uuid4
 
 import psycopg2
 import psycopg2.extensions
 import psycopg2.pool
 
 from pysquril.exc import DataIntegrityError, ParseError, OperationNotPermittedError
 from pysquril.generator import SqliteQueryGenerator, PostgresQueryGenerator
+from pysquril.utils import audit_table, audit_table_src, AUDIT_SEPARATOR, AUDIT_SUFFIX
+
+def sqlite_init(path: str) -> sqlite3.Connection:
+    engine = sqlite3.connect(path)
+    return engine
+
+
+def postgres_init(dbconfig: dict) -> psycopg2.pool.SimpleConnectionPool:
+    min_conn = 2
+    max_conn = 5
+    dsn = f"dbname={dbconfig['dbname']} user={dbconfig['user']} password={dbconfig['pw']} host={dbconfig['host']}"
+    pool = psycopg2.pool.SimpleConnectionPool(
+        min_conn, max_conn, dsn
+    )
+    return pool
+
 
 @contextmanager
 def sqlite_session(
     engine: sqlite3.Connection,
 ) -> ContextManager[sqlite3.Cursor]:
     session = engine.cursor()
     try:
@@ -58,14 +75,32 @@
 
     """
     Container for generating audit events.
     Keeps state for transaction IDs, generates
     timestamps, and event IDs, propagates
     audit messages.
 
+    There are five types of audit events:
+
+    1. update - changes to existing data (default on)
+    2. delete - deletions of existing data (default on)
+    3. restore - rolling back update and/or delete events (default on)
+    4. create - records of new data (default off)
+    5. read - who accessed with a given query  (default off)
+
+    Notes:
+
+    If create and read events are used, one could calculate
+    who looked at data for a given data subject, when on the
+    basis of audit data alone. One would have to apply the
+    query in each read event to the state of the data at the
+    time of the query, and check if the data belonging to the
+    subject (and/or the identfier of the data subject)
+    is contained in the returned result.
+
     """
 
     def __init__(
         self,
         identity: str,
         message: Optional[str] = "",
         identity_name: Optional[str] = None,
@@ -98,14 +133,20 @@
 
     def event_delete(self, *, diff: Any, previous: Any, query: str) -> dict:
         return self._event(diff, previous, "delete", query)
 
     def event_restore(self, *, diff: Any, previous: Any, query: str) -> dict:
         return self._event(diff, previous, "restore", query)
 
+    def event_create(self, *, diff: Any) -> dict:
+        return self._event(diff, None, "create", None)
+
+    def event_read(self, *, query: str) -> dict:
+        return self._event(None, None, "read", query)
+
 
 class DatabaseBackend(ABC):
 
     sep: str # schema separator character
     generator_class: Union[SqliteQueryGenerator, PostgresQueryGenerator]
     json_object_func: str
 
@@ -148,14 +189,15 @@
 
     @abstractmethod
     def table_insert(
         self,
         table_name: str,
         data: Union[dict, list],
         session: Optional[Union[sqlite3.Cursor, psycopg2.extensions.cursor]] = None,
+        audit: bool = False,
     ) -> bool:
         pass
 
     @abstractmethod
     def table_update(
         self,
         table_name: str,
@@ -163,19 +205,25 @@
         data: dict,
         tsc: Optional[AuditTransaction] = None,
         session: Optional[Union[sqlite3.Cursor, psycopg2.extensions.cursor]] = None,
     ) -> bool:
         pass
 
     @abstractmethod
-    def table_delete(self, table_name: str, uri_query: str) -> bool:
+    def table_delete(self, table_name: str, uri_query: str, audit: bool = True) -> bool:
         pass
 
     @abstractmethod
-    def table_select(self, table_name: str, uri_query: str, data: Optional[Union[dict, list]] = None) -> Iterable[tuple]:
+    def table_select(
+        self,
+        table_name: str,
+        uri_query: str,
+        data: Optional[Union[dict, list]] = None,
+        audit: bool = False,
+    ) -> Iterable[tuple]:
         pass
 
     @abstractmethod
     def table_restore(self, table_name: str, uri_query: str) -> bool:
         pass
 
     @abstractmethod
@@ -221,15 +269,15 @@
         """
         Check if the table from which audit records originate
         still exists.
 
         """
         exists = False
         try:
-            current_data = list(self.table_select(table_name.replace("_audit", ""), ""))
+            current_data = list(self.table_select(audit_table_src(table_name), ""))
             exists = True
         except (sqlite3.OperationalError, psycopg2.errors.UndefinedTable):
             pass
         return exists
 
     def table_restore(self, table_name: str, uri_query: str) -> dict:
         """
@@ -294,15 +342,15 @@
         except (sqlite3.OperationalError, psycopg2.errors.UndefinedTable):
             current_data = []
             current_pks = []
         # fetch the desired state
         if "order" in query_parts:
             uri_query = uri_query.split("&order")[0]
         uri_query = f"{uri_query}&order=timestamp.asc" # sorted from old to new
-        target_data = list(self.table_select(f"{table_name}_audit", uri_query))
+        target_data = list(self.table_select(audit_table(table_name), uri_query))
         if not target_data:
             return work_done # nothing to do
         tsc = AuditTransaction(self.requestor, message, self.requestor_name)
         session_func = self._session_func()
         try:
             # ensure the table exists, may have been deleted
             with session_func(self.engine) as session:
@@ -310,30 +358,30 @@
         except psycopg2.errors.DuplicateObject as e:
             pass # already exists
         handled = []
         with session_func(self.engine) as session:
             for entry in target_data:
                 target_entry = entry.get("previous")
                 pk_value = self._get_pk_value(primary_key, target_entry) if target_entry else None
-                if pk_value in handled or entry.get("event") == "restore":
+                if pk_value in handled or entry.get("event") in ["restore", "create", "read"]:
                     continue
                 target_entry = entry.get("previous")
                 result = list(
                     self.table_select(
                         table_name,
                         f"where={primary_key}=eq.{pk_value}",
                     )
                 )
                 if len(result) > 1:
                     raise DataIntegrityError(f"primary_key: {primary_key} is not unique")
                 elif not result:
                     # then it is currently deleted
                     self.table_insert(table_name, target_entry, session)
                     self.table_insert(
-                        f"{table_name}_audit",
+                        audit_table(table_name),
                         tsc.event_restore(diff=target_entry, previous=None, query=uri_query),
                         session,
                     )
                     work_done["restores"].append(entry)
                 else:
                     current_entry = result[0]
                     diff = self._diff_entries(current_entry, target_entry)
@@ -420,99 +468,137 @@
 
     def _query_for_select(
         self,
         table_name: str,
         uri_query: str,
         data: Optional[Union[dict, list]] = None,
         array_agg: bool = False,
+        apply_cutoff: bool = False,
     ) -> str:
         """
         Return the appropriate select statement for a given
         table_name, and uri_query, calculating any backup
         cutoff for audit data if needed.
 
         """
         backup_cutoff = None
-        if (
-            table_name.endswith("_audit")
-            and not self._audit_source_exists(table_name)
-            and self.backup_days is not None
-        ):
+        if apply_cutoff:
             backup_cutoff = (datetime.date.today() - timedelta(days=self.backup_days)).isoformat()
         sql = self.generator_class(
             f'{self._fqtn(table_name)}',
             uri_query,
             data=data,
             backup_cutoff=backup_cutoff,
             array_agg=array_agg,
         )
         return sql.select_query
 
-    def _query_for_select_many(self, uri_query: str, tables: list) -> str:
+    def _query_for_select_many(self, uri_query: str, tables: list, apply_cutoff: bool = False) -> str:
         queries = []
         for table_name in tables:
-            sql = self._query_for_select(table_name, uri_query, array_agg=True)
+            sql = self._query_for_select(table_name, uri_query, array_agg=True, apply_cutoff=apply_cutoff)
             queries.append(f"select {self.json_object_func}('{table_name}', ({sql}))")
         return " union all ".join(queries)
 
     def _yield_results(self, query: str)-> Iterable[tuple]:
         raise NotImplementedError
 
+    def _is_audit_table(self, table_name: str) -> bool:
+        """
+        Determine whether a given table is an audit table.
+
+        """
+        sufficient = False
+        neccesary = table_name.endswith(AUDIT_SEPARATOR + AUDIT_SUFFIX)
+        if not neccesary:
+            return neccesary and sufficient
+        try:
+            dummy_event = AuditTransaction("").event_read(query="")
+            result = list(
+                self._yield_results(
+                    f"select data from {table_name} limit 1"
+                )
+            )[0]
+            sufficient = (
+                uuid.UUID(result.get("transaction_id"))
+                and uuid.UUID(result.get("event_id"))
+                and result.get("event") in ["update", "delete", "read", "create"]
+                and result.get("timestamp") is not None
+                and set(result.keys()).difference(dummy_event.keys()) == set()
+            )
+
+        except Exception as e:
+            pass
+        return neccesary and sufficient
+
     def table_select(
         self,
         table_name: str,
         uri_query: str,
         data: Optional[Union[dict, list]] = None,
         exclude_endswith: list = [],
+        audit: bool = False,
     ) -> Iterable[tuple]:
         """
         Yield a resulset associated with a table_name, and a uri_query.
 
         The table_name can be either a reference to a specific table, or an
         asterisk expression intended to match a set of table names. In the
         latter case, a query is constructed to union the resulsets from
         all the relevant tables together.
 
         Optionally exclude tables that end with a specific pattern.
 
         """
+        apply_cutoff = (
+            self._is_audit_table(table_name)
+            and not self._audit_source_exists(table_name)
+            and self.backup_days is not None
+        )
         if "*" in table_name:
             tables = self.tables_list(exclude_endswith = exclude_endswith, table_like=table_name)
             if not tables:
                 return iter([])
-            query = self._query_for_select_many(uri_query, tables)
+            query = self._query_for_select_many(uri_query, tables, apply_cutoff=apply_cutoff)
         elif "," in  table_name:
             tables = table_name.split(",")
-            query = self._query_for_select_many(uri_query, tables)
+            query = self._query_for_select_many(uri_query, tables, apply_cutoff=apply_cutoff)
         else:
-            query = self._query_for_select(table_name, uri_query, data)
+            query = self._query_for_select(table_name, uri_query, data, apply_cutoff=apply_cutoff)
+        if audit:
+            tsc = AuditTransaction(identity=self.requestor, identity_name=self.requestor_name)
+            self.table_insert(audit_table(table_name), tsc.event_read(query=uri_query))
         return self._yield_results(query)
 
     def table_delete(
         self,
         table_name: str,
         uri_query: str,
         update_all_view: Optional[bool] = False,
+        audit: bool = True,
     ) -> bool:
         """
         Delete the intended data from the table if a uri_query
         is present, otherwise drop the table. All deletions
-        are recorded in the audit log.
+        are recorded in the audit log by default, but this can
+        be disabled by callers. This is useful for cases where
+        data is being deleted completely for compliance purposes.
 
         """
         audit_data = []
         sql = self.generator_class(f'{self._fqtn(table_name)}', uri_query)
-        tsc = AuditTransaction(self.requestor, sql.message, self.requestor_name)
-        for row in self.table_select(table_name, uri_query):
-            audit_data.append(tsc.event_delete(diff=None, previous=row, query=uri_query))
+        if audit:
+            tsc = AuditTransaction(self.requestor, sql.message, self.requestor_name)
+            for row in self.table_select(table_name, uri_query):
+                audit_data.append(tsc.event_delete(diff=None, previous=row, query=uri_query))
         with self._session_func()(self.engine) as session:
             session.execute(sql.delete_query)
-            if not table_name.endswith("_audit"):
-                self.table_create(f'{table_name}_audit', session)
-                self.table_insert(f'{table_name}_audit', audit_data, session)
+            if not table_name.endswith("_audit") and audit:
+                self.table_create(audit_table(table_name), session)
+                self.table_insert(audit_table(table_name), audit_data, session)
         if update_all_view:
             self._define_all_view(table_name)
         return True
 
     def table_update(
         self,
         table_name: str,
@@ -521,58 +607,72 @@
         tsc: Optional[AuditTransaction] = None,
         session: Optional[Union[sqlite3.Cursor, psycopg2.extensions.cursor]] = None,
     ) -> bool:
         """
         Update one or more keys, recording changes in the audit log.
 
         """
+        if self._is_audit_table(table_name):
+            raise OperationNotPermittedError("audit tables cannot be altered directly")
         audit_data = []
         sql = self.generator_class(f'{self._fqtn(table_name)}', uri_query, data=data)
         tsc = AuditTransaction(self.requestor, sql.message, self.requestor_name) if not tsc else tsc
         for val in self.table_select(table_name, uri_query, data=data):
             audit_data.append(tsc.event_update(diff=data, previous=val, query=uri_query))
         if session:
             session.execute(sql.update_query)
-            self.table_insert(f'{table_name}_audit', audit_data, session)
+            self.table_insert(audit_table(table_name), audit_data, session)
         else:
             with self._session_func()(self.engine) as session:
                 session.execute(sql.update_query)
-            self.table_insert(f'{table_name}_audit', audit_data)
+            self.table_insert(audit_table(table_name), audit_data)
         return True
 
     def table_alter(self, table_name: str, uri_query: str) -> dict:
         """
         Alter the name of a table, and its audit table (if it exists).
         Return information about which tables were altered.
 
         """
-        if table_name.endswith("_audit"):
+        if self._is_audit_table(table_name):
             raise OperationNotPermittedError("audit tables cannot be altered directly")
         sql = self.generator_class(
             f'{self._fqtn(table_name)}',
             uri_query,
             table_name_func=self._fqtn,
         )
         with self._session_func()(self.engine) as session:
             session.execute(sql.alter_query)
         altered = {"tables": [table_name]}
         try:
-            audit_table_name = f"{table_name}_audit"
+            audit_table_name = audit_table(table_name)
             sql = self.generator_class(
                 f'{self._fqtn(audit_table_name)}',
                 uri_query,
                 table_name_func=self._fqtn,
+                audit=True,
             )
             with self._session_func()(self.engine) as session:
                 session.execute(sql.alter_query)
             altered["tables"].append(audit_table_name)
         except (psycopg2.errors.UndefinedTable, sqlite3.OperationalError):
             pass
         return altered
 
+    def _audit_insert(self, table_name: str, data: Union[str, list]) -> bool:
+        tsc = AuditTransaction(identity=self.requestor, identity_name=self.requestor_name)
+        audit_data = []
+        if type(data) is list:
+            for row in data:
+                audit_data.append(tsc.event_create(diff=row))
+        else:
+            audit_data = [tsc.event_create(diff=data)]
+        self.table_insert(audit_table(table_name), audit_data)
+        return True
+
 
 class SqliteBackend(GenericBackend):
 
     """
     This backend works reliably, and offers decent read-write
     performance to API clients under the following conditions:
 
@@ -700,14 +800,15 @@
 
     def table_insert(
         self,
         table_name: str,
         data: Union[dict, list],
         session: Optional[sqlite3.Cursor] = None,
         update_all_view: Optional[bool] = False,
+        audit: bool = False,
     ) -> bool:
         try:
             dtype = type(data)
             insert_stmt = f'insert into {self._fqtn(table_name)} (data) values (?)'
             target = []
             if dtype is list:
                 for element in data:
@@ -715,27 +816,27 @@
             elif dtype is dict:
                 target.append((json.dumps(data),))
             if session:
                 # in this case we are re-using a session
                 # from a context manager estabilshed by the caller
                 # and if an exception is raised, the caller handles it
                 session.executemany(insert_stmt, target)
-                return True
             else:
                 try:
                     with sqlite_session(self.engine) as session:
                         session.executemany(insert_stmt, target)
-                    return True
                 except (sqlite3.ProgrammingError, sqlite3.OperationalError) as e:
                     with sqlite_session(self.engine) as session:
                         self.table_create(table_name, session)
                         session.executemany(insert_stmt, target)
                     if update_all_view:
                         self._define_all_view(table_name)
-                    return True
+            if audit:
+                self._audit_insert(table_name, data)
+            return True
         except sqlite3.IntegrityError as e:
             logging.info('Ignoring duplicate row')
             return True # idempotent PUT
         except sqlite3.ProgrammingError as e:
             logging.error('Syntax error?')
             raise e
         except sqlite3.OperationalError as e:
@@ -889,14 +990,15 @@
 
     def table_insert(
         self,
         table_name: str,
         data: Union[dict, list],
         session: Optional[psycopg2.extensions.cursor] = None,
         update_all_view: Optional[bool] = False,
+        audit: bool = False,
     ) -> bool:
         try:
             dtype = type(data)
             insert_stmt = f'insert into {self._fqtn(table_name)} (data) values (%s)'
             target = []
             if dtype is list:
                 for element in data:
@@ -904,27 +1006,27 @@
             elif dtype is dict:
                 target.append((json.dumps(data),))
             if session:
                 # in this case we are re-using a session
                 # from a context manager estabilshed by the caller
                 # and if an exception is raised, the caller handles it
                 session.executemany(insert_stmt, target)
-                return True
             else:
                 try:
                     with postgres_session(self.engine) as session:
                         session.executemany(insert_stmt, target)
-                    return True
                 except (psycopg2.ProgrammingError, psycopg2.OperationalError) as e:
                     with postgres_session(self.engine) as session:
                         self.table_create(table_name, session)
                         session.executemany(insert_stmt, target)
                     if update_all_view:
                         self._define_all_view(table_name)
-                    return True
+            if audit:
+                self._audit_insert(table_name, data)
+            return True
         except psycopg2.IntegrityError as e:
             logging.info('Ignoring duplicate row')
             return True # idempotent PUT
         except psycopg2.ProgrammingError as e:
             logging.error('Syntax error?')
             raise e
         except psycopg2.OperationalError as e:
```

### Comparing `pysquril-0.6.2/pysquril/generator.py` & `pysquril-0.7.0/pysquril/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,33 +15,36 @@
     WhereTerm,
     OrderTerm,
     RangeTerm,
     SetTerm,
     Clause,
     UriQuery,
 )
+from pysquril.utils import audit_table
 
 class SqlGenerator(object):
 
     """
     Generic class, used to implement SQL code generation.
 
     """
 
     db_init_sql = None
     json_array_sql = None
+    cascade_on_drop = False
 
     def __init__(
         self,
         table_name: str,
         uri_query: str,
         data: Union[list, dict] = None,
         backup_cutoff: Optional[str] = None,
         array_agg: Optional[bool] = False,
         table_name_func: Optional[Callable] = None,
+        audit: bool = False,
     ) -> None:
         self.table_name = table_name
         self.uri_query = uri_query
         self.data = data
         self.parsed_uri_query = UriQuery(table_name, uri_query)
         self.table_name_func = table_name_func
         self.operators = {
@@ -61,15 +64,15 @@
             msg = 'Extending the SqlGenerator requires setting the class level property: json_array_sql'
             raise Exception(msg)
         self.has_aggregate_func = False
         self.select_query = self.sql_select(backup_cutoff, array_agg)
         self.update_query = self.sql_update()
         self.delete_query = self.sql_delete()
         self.message = self.uri_message()
-        self.alter_query = self.sql_alter()
+        self.alter_query = self.sql_alter(audit)
 
     # Classes that extend the SqlGenerator must implement the following methods
     # they are called by functions that are mapped over terms in clauses
     # for each term, an appropriate piece of SQL needs to be returned.
     # What is appropriate, depends on the backend.
 
     def _gen_sql_key_selection(self, term: SelectTerm, parsed: Key) -> str:
@@ -349,35 +352,37 @@
                 _query += f"update {self.table_name} {expr} {_where}; "
             return _query
 
     def sql_delete(self) -> str:
         _where = self._gen_sql_where_clause()
         if not _where:
             query = f"drop table {self.table_name}"
+            if self.cascade_on_drop:
+                query += " cascade"
         else:
             query = f"delete from {self.table_name} {_where}"
         return query
 
     def uri_message(self) -> str:
         return self.parsed_uri_query.message
 
-    def sql_alter(self) -> str:
+    def sql_alter(self, audit: bool) -> str:
         """
         Change the name of a table, if it does not
         exist an error is raised.
 
         """
         alter = self.parsed_uri_query.alter
         if not alter:
             return ""
         else:
             term = alter.parsed[0]
             element = term.parsed[0]
-            if self.table_name.endswith('_audit"'):
-                new_name = self.table_name_func(f"{element.val}_audit", no_schema=True)
+            if audit:
+                new_name = self.table_name_func(audit_table(element.val), no_schema=True)
             else:
                 new_name = self.table_name_func(element.val, no_schema=True)
             sql = f"alter table {self.table_name} rename to {new_name}"
             return sql
 
 
 class SqliteQueryGenerator(SqlGenerator):
@@ -461,17 +466,23 @@
                 _key = select_term.bare_term
                 _idx = select_term.parsed[-1].idx
                 _col = select_term.parsed[-1].sub_selections[0]
                 target = f'{_key}[{_idx}].{_col}'
             else:
                 target = select_term.bare_term
         else:
-            if not isinstance(select_term.parsed[0], Key):
-                raise Exception(f'Invalid term {term.original}')
-            target = select_term.parsed[0].element
+            if not (
+                isinstance(select_term.parsed[0], Key) or
+                isinstance(select_term.parsed[0], ArraySpecific)
+            ):
+                raise ParseError(f'Unsupported where term: {term.original}')
+            if isinstance(select_term.parsed[0], ArraySpecific):
+                target = select_term.original
+            else:
+                target = select_term.parsed[0].element
         col = f"json_extract(data, '$.{target}')"
         if isinstance(term, WhereTerm) and term.parsed[0].op in ['eq', 'neq']:
             col = f"cast ({col} as text)"
         return col
 
     def _gen_sql_update(self, term: SetTerm) -> str:
         key = term.parsed[0].select_term.bare_term
@@ -495,14 +506,15 @@
                 return f"'{val}'"
         except ValueError:
             return f"'{val}'"
 
 
 class PostgresQueryGenerator(SqlGenerator):
 
+    cascade_on_drop = True
     json_array_sql = 'jsonb_build_array'
     db_init_sql = [
         """
         create or replace function filter_array_elements(data jsonb, keys text[])
             returns jsonb as $$
             declare key text;
             declare element jsonb;
@@ -624,18 +636,26 @@
                 _idx = select_term.parsed[-1].idx
                 _col = select_term.parsed[-1].sub_selections[0]
                 col = f"data#>'{{{target}}}'#>'{{{_idx}}}'#>'{{{_col}}}'"
             else:
                 target = self._gen_select_target(select_term.bare_term)
                 col = f"data{final_select_op}'{{{target}}}'"
         else:
-            if not isinstance(select_term.parsed[0], Key):
-                raise Exception(f'Invalid term {term.original}')
-            target = select_term.parsed[0].element
-            col = f"data{final_select_op}'{{{target}}}'"
+            if not (
+                isinstance(select_term.parsed[0], Key) or
+                isinstance(select_term.parsed[0], ArraySpecific)
+            ):
+                raise ParseError(f'Unsupported where term: {term.original}')
+            if isinstance(select_term.parsed[0], ArraySpecific):
+                target = self._gen_select_target(select_term.bare_term)
+                _idx = select_term.parsed[0].idx
+                col = f"data#>'{{{target}}}'{final_select_op}'{{{_idx}}}'"
+            else:
+                target = select_term.parsed[0].element
+                col = f"data{final_select_op}'{{{target}}}'"
         if isinstance(term, WhereTerm):
             try:
                 integer_ops = ['gt', 'gte', 'lt', 'lte']
                 int(term.parsed[0].val)
                 if (
                     term.parsed[0].op in integer_ops
                     and str(float(term.parsed[0].val)) != str(term.parsed[0].val)
@@ -650,15 +670,14 @@
     def _gen_sql_update(self, term: SetTerm) -> str:
         key = term.parsed[0].select_term.bare_term
         if not self.data or key not in self.data.keys():
             raise ParseError(f'Target key of update: {key} not found in payload')
         val = json.dumps(self.data[key]).replace("'", "''") # to handle single quotes inside
         return f" set data = jsonb_set(data, '{{{key}}}', ('{val}')::jsonb)"
 
-
     def _gen_select_with_retention(self, backup_cutoff: str) -> str:
         return f"(select * from {self.table_name} where data->>'timestamp' >= '{backup_cutoff}')a"
 
     def _gen_array_agg(self, query: str) -> str:
         return f"select json_agg(data) from ({query})a"
 
     def _maybe_float(self, val: Any) -> Union[str, float]:
```

### Comparing `pysquril-0.6.2/pysquril/parser.py` & `pysquril-0.7.0/pysquril/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,14 +383,36 @@
         element = term.parsed[0]
         if element.select_term.bare_term != "name":
             raise ParseError("alter statements limited to `name` attribute")
         if element.op != "eq":
             raise ParseError(f"rename requires `eq` operator, not {element.op}")
 
 
+class Message(object):
+
+    def __init__(self, original: str) -> None:
+        self.original = original
+        self.parsed = self.parse_message(original)
+
+    def parse_message(self, message: str) -> str:
+        out = ""
+        if unquote(message) != message:
+            out = unquote(message)
+        else:
+            for idx, token in enumerate(message):
+                previous = previous_element(message, idx)
+                if (token == "'" and previous != "\\") or token == "\\":
+                    continue
+                elif token == "'" and previous == "\\":
+                    out += "''"
+                else:
+                    out += token
+        return out
+
+
 class UriQuery(object):
 
     """
     Lex and parse a URI query into a UriQuery object:
 
         Query
             -> Clause(s)
@@ -420,22 +442,14 @@
             if self.order:
                 raise ParseError("ordering not supported for group_by")
             group_by_keys = self.group_by.split_clause()
             select_keys = self.select.split_clause()
             if not set(group_by_keys).intersection(select_keys) == set(group_by_keys):
                 raise ParseError("group by keys must be used in select")
 
-    def parse_message(self) -> str:
-        message = ""
-        parts = self.original.split("&")
-        for part in parts:
-            if part.startswith("message="):
-                message = unquote(part.split("=")[-1])
-        return message
-
     def _slice(
         self,
         *,
         target: str,
         positions: list,
     ) -> list:
         """
@@ -491,7 +505,18 @@
     def parse_clause(self, *, prefix: str, Cls: Clause) -> Clause:
         parts = self._slice(
             target=self.original, positions=self._index_clauses(self.original)
         )
         for part in parts:
             if part.startswith(prefix):
                 return Cls(part[len(prefix):])
+
+    def parse_message(self) -> str:
+        prefix = "message="
+        message = None
+        parts = self._slice(
+            target=self.original, positions=self._index_clauses(self.original)
+        )
+        for part in parts:
+            if part.startswith(prefix):
+                message = Message(part[len(prefix):]).parsed
+        return message
```

### Comparing `pysquril-0.6.2/pysquril/test_data.py` & `pysquril-0.7.0/pysquril/test_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         'lol2': '123',
         'lol3': {'yeah': 123},
         'lol4': {'yeah': '123'},
         'float': 3.1,
         'float_str': '3.2',
         'self': 'yes',
         'beneficial': 'yes',
+        'contemplate': 'arising',
     },
     {
         'y': 11,
         'z': 1,
         'c': [
             {
                 'h': 3,
@@ -46,14 +47,15 @@
         'lol1': 456,
         'lol2': '456',
         'lol3': {'yeah': 456},
         'lol4': {'yeah': '456'},
         'float': 4.1,
         'self': 'no',
         'beneficial': 'yes',
+        'contemplate': 'vanishing',
     },
     {
         'a': {
             'k1': {
                 'r1': [1, 2],
                 'r2': 2
             },
@@ -64,14 +66,15 @@
         'd': 'string3',
         'timestamp': '2020-10-14T13:15:46.187575',
         'q': {
             'r': [{'s': 77}],
         },
         'self': 'yes',
         'beneficial': 'no',
+        'contemplate': 'non arising',
     },
     {
         'a': {
             'k1': {
                 'r1': [33, 200],
                 'r2': 90
             },
@@ -83,14 +86,15 @@
         'timestamp': '2020-10-14T16:15:26.388575',
         'q': {
             'r': [{'s': 0}],
         },
         'meh2': '()[],and:,or:. where=;',
         'self': 'no',
         'beneficial': 'no',
+        'contemplate': "g'n niks nie",
     },
     {
         'x': 10,
         'timestamp': '2020-10-14T20:20:34.388511',
         'q': {
             'r': [{'s': 10}],
         },
```

### Comparing `pysquril-0.6.2/pysquril/tests.py` & `pysquril-0.7.0/pysquril/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,49 @@
 
 import datetime
 import json
 import os
 import sqlite3
 import unittest
+import uuid
 import tempfile
 
 from datetime import timedelta
 from typing import Callable, Union
 from urllib.parse import quote
 
 import psycopg2
 import psycopg2.errors
 import psycopg2.extensions
 import psycopg2.pool
 import pytest
 
 from termcolor import colored
 
-from pysquril.backends import SqliteBackend, PostgresBackend, sqlite_session, postgres_session
+from pysquril.backends import (
+    SqliteBackend,
+    PostgresBackend,
+    sqlite_init,
+    postgres_init,
+    sqlite_session,
+    postgres_session,
+)
 from pysquril.exc import ParseError, OperationNotPermittedError
 from pysquril.generator import SqliteQueryGenerator, PostgresQueryGenerator
 from pysquril.parser import (
     SelectClause,
     WhereClause,
     GroupByTerm,
     GroupByClause,
     AlterClause,
     UriQuery,
 )
 from pysquril.test_data import dataset
+from pysquril.utils import audit_table
 
-def sqlite_init(
-    path: str,
-    name: str = 'api-data.db',
-) -> sqlite3.Connection:
-    engine = sqlite3.connect(path + '/' + name)
-    return engine
-
-
-def postgres_init(dbconfig: dict) -> psycopg2.pool.SimpleConnectionPool:
-    min_conn = 2
-    max_conn = 5
-    dsn = f"dbname={dbconfig['dbname']} user={dbconfig['user']} password={dbconfig['pw']} host={dbconfig['host']}"
-    pool = psycopg2.pool.SimpleConnectionPool(
-        min_conn, max_conn, dsn
-    )
-    return pool
 
 TEST_REQUESTOR = "p11-treq"
 TEST_REQUESTOR_NAME = "Test Requestor"
 
 class TestParser(object):
 
     def test_select(self) -> None:
@@ -223,15 +216,15 @@
             pass
         try:
             db.table_delete('another_table', '')
         except Exception as e:
             pass
         try:
             db.table_delete('silly_table', '')
-            db.table_delete('silly_table_audit', '')
+            db.table_delete(audit_table('silly_table'), '')
         except Exception as e:
             pass
 
         # test '*' without any tables
         out = list(db.table_select('*', 'select=count(1)', exclude_endswith = ['_audit', '_metadata']))
         assert list(out) == []
 
@@ -388,15 +381,20 @@
         assert len(out) == 2
         # Run the query with not as a string value.
         out=run_select_query('select=d&where=d=eq.not')
         assert len(out) == 0
         # in
         out = run_select_query('select=d&where=d=in.[string1,string2]')
         assert len(out) == 2
-        assert out == [['string1'], ['string2']]
+        out = run_select_query("select=contemplate&where=contemplate=in.['non arising','vanishing']")
+        assert len(out) == 2
+        assert ['non arising'] in out
+        assert ['vanishing'] in out
+        out = run_select_query("select=contemplate&where=contemplate=in.['g\\'n niks nie','vanishing']")
+        assert len(out) == 2
         # nested key ops
         out = run_select_query('where=a.k1.r2=eq.90')
         assert len(out) == 1
         # nested key ops with slicing
         out = run_select_query('select=x&where=a.k1.r1[0]=eq.1')
         assert out[0][0] == 88
         out = run_select_query('select=x&where=a.k3[0|h]=eq.0')
@@ -442,14 +440,18 @@
         assert out[0][0] == 107
         # ampersand
         out = run_select_query("select=x&where=being=eq.'arising&vanishing'")
         assert out[0][0] == 10
         # esacping single quotes
         out = run_select_query("select=x&where=loop=eq.'g\\'n kat oor die pad'")
         assert out[0][0] == 10
+        # with a simple array
+        out = run_select_query("select=z&where=b[0]=eq.1")
+        assert out[0][0] == 5
+
 
         # ORDER
         if verbose:
             print('\n===> ORDER\n')
         # Note: postgres and sqlite treat NULLs different in ordering
         # postgres puts them first, sqlite puts them last, so be it
         # simple key
@@ -565,19 +567,19 @@
             table='yet_another_table'
         )
         out = run_alter_query("alter=name=eq.silly_table", "yet_another_table")
         assert len(out["tables"]) == 2
 
         # not permitted directly on an audit table
         with pytest.raises(OperationNotPermittedError):
-            run_alter_query("alter=name=eq.new", "silly_table_audit")
+            run_alter_query("alter=name=eq.new", audit_table("silly_table"))
 
 
     def test_sqlite(self):
-        engine = sqlite_init('/tmp', name='api-test.db')
+        engine = sqlite_init('/tmp/api-test.db')
         self.run_backend_tests(
             self.data,
             engine,
             sqlite_session,
             SqliteQueryGenerator,
             SqliteBackend,
             self.verbose
@@ -643,15 +645,15 @@
         retrieved_data = result[0]
         self.assertEqual(retrieved_data, {**data, **new_data})
         self.assertNotEqual(retrieved_data[key_to_update], original_value)
         self.assertEqual(retrieved_data[key_to_update], new_data[key_to_update])
 
         # view update audit data
         result = list(self.backend.table_select(
-            table_name=f"{test_table}_audit", uri_query="order=timestamp.asc")
+            table_name=audit_table(test_table), uri_query="order=timestamp.asc")
         )
         self.assertTrue(result)
         audit_event = result[0]
         self.assertEqual(audit_event["previous"], data)
         self.assertEqual(audit_event["diff"], new_data)
         self.assertEqual(audit_event["event"], "update")
         self.assertTrue(audit_event["transaction_id"] is not None)
@@ -677,28 +679,28 @@
             uri_query=f"restore&primary_key={pkey}&where=event_id=eq.{audit_event.get('event_id')}&message={quote(message)}"
         )
         self.assertEqual(len(result.get("updates")), 1)
         self.assertEqual(len(result.get("restores")), 0)
         result = list(self.backend.table_select(table_name=test_table, uri_query="where=id=eq.1"))
         self.assertEqual(result[0].get(key_to_update), original_value)
         result = list(self.backend.table_select(
-            table_name=f"{test_table}_audit", uri_query="order=timestamp.desc")
+            table_name=audit_table(test_table), uri_query="order=timestamp.desc")
         )
         self.assertEqual(result[0].get("message"), message)
 
         # delete a specific entry
         message = "bad data: must delete, & never repeat (tm)"
         self.backend.table_delete(
             table_name=test_table,
             uri_query=f"where=key3=not.is.null&message={quote(message)}"
         )
-        result = list(self.backend.table_select(table_name=f"{test_table}_audit", uri_query=""))
+        result = list(self.backend.table_select(table_name=audit_table(test_table), uri_query=""))
         self.assertEqual(len(result), 4)
         result = list(self.backend.table_select(
-            table_name=f"{test_table}_audit", uri_query="order=timestamp.desc")
+            table_name=audit_table(test_table), uri_query="order=timestamp.desc")
         )
         self.assertEqual(result[0].get("message"), message)
 
         # restore the deleted entry
         result = self.backend.table_restore(
             table_name=test_table,
             uri_query=f"restore&primary_key={pkey}&where=event=eq.delete"
@@ -708,15 +710,15 @@
         result = list(self.backend.table_select(table_name=test_table, uri_query="where=id=eq.2"))
         self.assertTrue(result[0] is not None)
 
         # delete the table
         self.backend.table_delete(table_name=test_table, uri_query="")
 
         # check that the deletes are in the audit
-        result = list(self.backend.table_select(table_name=f"{test_table}_audit", uri_query=""))
+        result = list(self.backend.table_select(table_name=audit_table(test_table), uri_query=""))
         self.assertEqual(len(result), 7)
 
         # restore everything
         result = self.backend.table_restore(table_name=test_table, uri_query=f"restore&primary_key={pkey}")
         self.assertTrue(result is not None)
         result = list(self.backend.table_select(table_name=test_table, uri_query="order=id.asc"))
         self.assertEqual(result[0], data)
@@ -727,18 +729,18 @@
 
         # try to retrieve deleted table
         select = self.backend.table_select(table_name=test_table, uri_query="")
         with self.assertRaises((sqlite3.OperationalError, psycopg2.errors.UndefinedTable)):
             next(select)
 
         # delete the audit table
-        self.backend.table_delete(table_name=f"{test_table}_audit", uri_query="")
+        self.backend.table_delete(table_name=audit_table(test_table), uri_query="")
         
         # try to retrieve deleted table's audit table
-        select = self.backend.table_select(table_name=f"{test_table}_audit", uri_query="")
+        select = self.backend.table_select(table_name=audit_table(test_table), uri_query="")
         with self.assertRaises((sqlite3.OperationalError, psycopg2.errors.UndefinedTable)):
             next(select)
 
         # test deleting an entire table, without any updates
         # automatic audit table creation on delete
         # use a nested primary key, to test restores with such keys
         some_data = {"pk": {"id": 0}, "lol": None, "cat": [1, 2]}
@@ -748,103 +750,142 @@
         self.backend.table_insert(table_name=some_table, data=some_more_data)
         self.backend.table_update(
             table_name=some_table,
             uri_query=f"set=lol&where=pk.id=eq.0",
             data={"lol": "wat"},
         )
         self.backend.table_delete(table_name=some_table, uri_query="")
-        audit = list(self.backend.table_select(table_name=f"{some_table}_audit", uri_query=""))
+        audit = list(self.backend.table_select(table_name=audit_table(some_table), uri_query=""))
         self.assertEqual(len(audit), 3)
         nested_result = self.backend.table_restore(
             table_name=some_table, uri_query=f"restore&primary_key=pk.id"
         )
         self.assertEqual(len(nested_result.get("restores")), 2)
         self.assertEqual(len(nested_result.get("updates")), 0)
         self.backend.table_delete(table_name=some_table, uri_query="")
-        self.backend.table_delete(table_name=f"{some_table}_audit", uri_query="")
+        self.backend.table_delete(table_name=audit_table(some_table), uri_query="")
 
 
         # test backup retention enforcement
         backup_table = "backedup"
         self.backend.backup_days = 1
         self.backend.table_insert(table_name=backup_table, data={"breathe-in": "long", "id": 0})
         self.backend.table_insert(table_name=backup_table, data={"breathe-out": "long", "id": 1})
         self.backend.table_delete(table_name=backup_table, uri_query="")
 
         # within the retention period
-        audit = list(self.backend.table_select(table_name=f"{backup_table}_audit", uri_query=""))
+        audit = list(self.backend.table_select(table_name=audit_table(backup_table), uri_query=""))
         self.assertEqual(len(audit), 2)
         result = self.backend.table_restore(
             table_name=backup_table, uri_query=f"restore&primary_key=id",
         )
         self.assertEqual(len(result.get("restores")), 2)
         original = list(self.backend.table_select(table_name=backup_table, uri_query=""))
         self.assertTrue(len(original), 2)
 
         # cleanup
         self.backend.table_delete(table_name=backup_table, uri_query="")
-        self.backend.table_delete(table_name=f"{backup_table}_audit", uri_query="")
+        self.backend.table_delete(table_name=audit_table(backup_table), uri_query="")
 
 
         # outside the retention period
         not_backup_table = "notbackedup"
         self.backend.backup_days = 1
         self.backend.table_insert(table_name=not_backup_table, data={"breathe-in": "short", "id": 0})
         self.backend.table_insert(table_name=not_backup_table, data={"breathe-out": "short", "id": 1})
         self.backend.table_delete(table_name=not_backup_table, uri_query="")
 
         # now adjust the audit timestamps to fall outside the retention period
         target = (datetime.datetime.now() - timedelta(days=2)).isoformat()
         if isinstance(self.backend, SqliteBackend):
             new = json.dumps({"timestamp": target})
-            update_query = f"update {not_backup_table}_audit set data = json_patch(data, '{new}')"
+            update_query = f"update {audit_table(not_backup_table)} set data = json_patch(data, '{new}')"
         elif isinstance(self.backend, PostgresBackend):
-            update_query = f"update {not_backup_table}_audit set data = jsonb_set(data, '{{timestamp}}', '\"{target}\"')"
+            update_query = f"update {audit_table(not_backup_table)} set data = jsonb_set(data, '{{timestamp}}', '\"{target}\"')"
         with self.session_func(self.engine) as session:
             session.execute(update_query)
 
         # should not be able to view audit or restore data
-        audit = list(self.backend.table_select(table_name=f"{not_backup_table}_audit", uri_query=""))
+        audit = list(self.backend.table_select(table_name=audit_table(not_backup_table), uri_query=""))
         self.assertEqual(len(audit), 0)
         result = self.backend.table_restore(
             table_name=not_backup_table, uri_query=f"restore&primary_key=id",
         )
         self.assertEqual(len(result.get("restores")), 0)
 
         # cleanup
-        self.backend.table_delete(table_name=f"{not_backup_table}_audit", uri_query="")
+        self.backend.table_delete(table_name=audit_table(not_backup_table), uri_query="")
+
+        # delete without audit
+        table_without_audit = "without_audit"
+        self.backend.table_insert(table_name=table_without_audit, data={"breathe": "calming", "id": 0})
+        self.backend.table_delete(table_name=table_without_audit, uri_query="", audit=False)
+        with pytest.raises((psycopg2.errors.UndefinedTable, sqlite3.OperationalError)):
+            audit = list(
+                self.backend.table_select(
+                    table_name=audit_table(table_without_audit),
+                    uri_query="",
+                )
+            )
 
+        # audit for create and read
+        verbose_table = "table_with_full_audit"
+        try:
+            self.backend.table_delete(table_name=verbose_table, uri_query="")
+            self.backend.table_delete(table_name=audit_table(verbose_table), uri_query="")
+        except Exception:
+            pass
+        self.backend.table_insert(
+            table_name=verbose_table,
+            data={"observing": "mind objects", "id": 0},
+            audit=True,
+        )
+        self.backend.table_select(
+            table_name=verbose_table, uri_query="select=observing", audit=True,
+        )
+        audit = list(
+            self.backend.table_select(
+                table_name=audit_table(verbose_table),
+                uri_query="",
+            )
+        )
+        self.assertEqual(len(audit), 2)
+        self.backend.table_delete(table_name=audit_table(verbose_table), uri_query="")
 
     def test_all_view(self) -> bool:
         tenant1 = "p11"
         tenant2 = "p12"
         tenant3 = "p13"
         table_name = "A"
-        for idx, tenant in enumerate([tenant1, tenant2, tenant3]):
+        for tenant in [tenant1, tenant2, tenant3]:
             view_backend = self.backend_class(
                 self.engine, schema=tenant, schema_pattern="p"
             )
+            try:
+                view_backend.table_delete(table_name=table_name, uri_query="")
+            except Exception as e:
+                pass
             view_backend.table_insert(
                 table_name,
-                data={"id": idx, "data": f"yes {str(idx)}"},
+                data={"id": str(uuid.uuid4()), "data": f"yes"},
                 update_all_view=True,
             )
         all_backend = self.backend_class(
             self.engine, schema="all", schema_pattern="p"
         )
         result = list(all_backend.table_select(table_name, ""))
         self.assertEqual(len(result), 3)
 
 class TestSqliteBackend(TestSqlBackend):
     __test__ = True
 
     def setUp(self) -> None:
         self.directory = tempfile.gettempdir()
         self.file = f"{__package__}_test.db"
-        self.engine = sqlite_init(self.directory, name=self.file)
+        self.engine = sqlite_init(f"{self.directory}/{self.file}")
         self.backend = SqliteBackend(
             self.engine, requestor=TEST_REQUESTOR, requestor_name=TEST_REQUESTOR_NAME
         )
         self.session_func = sqlite_session
         self.backend_class = SqliteBackend
     
     def tearDown(self) -> None:
```

