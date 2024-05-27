# Comparing `tmp/goodboy_sqlalchemy-0.2.2.tar.gz` & `tmp/goodboy_sqlalchemy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodboy_sqlalchemy-0.2.2.tar", max compression
+gzip compressed data, was "goodboy_sqlalchemy-0.2.3.tar", max compression
```

## Comparing `goodboy_sqlalchemy-0.2.2.tar` & `goodboy_sqlalchemy-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1058 2022-03-07 16:56:23.742158 goodboy_sqlalchemy-0.2.2/LICENSE
--rw-r--r--   0        0        0      113 2022-03-07 16:54:23.496000 goodboy_sqlalchemy-0.2.2/README.md
--rw-r--r--   0        0        0      786 2023-03-03 16:10:34.347621 goodboy_sqlalchemy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      707 2023-03-03 16:10:39.199671 goodboy_sqlalchemy-0.2.2/src/goodboy_sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2955 2023-03-03 16:07:35.561788 goodboy_sqlalchemy-0.2.2/src/goodboy_sqlalchemy/column.py
--rw-r--r--   0        0        0     2643 2022-03-18 17:07:52.265231 goodboy_sqlalchemy-0.2.2/src/goodboy_sqlalchemy/column_schemas.py
--rw-r--r--   0        0        0     5024 2022-04-08 16:09:38.032206 goodboy_sqlalchemy-0.2.2/src/goodboy_sqlalchemy/mapped.py
--rw-r--r--   0        0        0     5661 2023-02-17 05:21:44.826187 goodboy_sqlalchemy-0.2.2/src/goodboy_sqlalchemy/mapped_key.py
--rw-r--r--   0        0        0      110 2022-03-12 17:03:17.754562 goodboy_sqlalchemy-0.2.2/src/goodboy_sqlalchemy/messages.py
--rw-r--r--   0        0        0        0 2022-04-08 16:32:29.141917 goodboy_sqlalchemy-0.2.2/src/goodboy_sqlalchemy/py.typed
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 goodboy_sqlalchemy-0.2.2/setup.py
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 goodboy_sqlalchemy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-04-14 11:07:25.254259 goodboy_sqlalchemy-0.2.3/LICENSE
+-rw-r--r--   0        0        0      113 2024-04-14 11:07:25.254346 goodboy_sqlalchemy-0.2.3/README.md
+-rw-r--r--   0        0        0      786 2024-05-27 14:55:13.255877 goodboy_sqlalchemy-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      707 2024-05-27 14:55:02.827776 goodboy_sqlalchemy-0.2.3/src/goodboy_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2955 2024-04-14 11:07:25.255022 goodboy_sqlalchemy-0.2.3/src/goodboy_sqlalchemy/column.py
+-rw-r--r--   0        0        0     2643 2024-04-14 11:07:25.255138 goodboy_sqlalchemy-0.2.3/src/goodboy_sqlalchemy/column_schemas.py
+-rw-r--r--   0        0        0     5024 2024-04-14 11:07:25.255340 goodboy_sqlalchemy-0.2.3/src/goodboy_sqlalchemy/mapped.py
+-rw-r--r--   0        0        0     5660 2024-05-27 14:45:26.997357 goodboy_sqlalchemy-0.2.3/src/goodboy_sqlalchemy/mapped_key.py
+-rw-r--r--   0        0        0      110 2024-04-14 11:07:25.255631 goodboy_sqlalchemy-0.2.3/src/goodboy_sqlalchemy/messages.py
+-rw-r--r--   0        0        0        0 2024-04-14 11:07:25.255674 goodboy_sqlalchemy-0.2.3/src/goodboy_sqlalchemy/py.typed
+-rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 goodboy_sqlalchemy-0.2.3/PKG-INFO
```

### Comparing `goodboy_sqlalchemy-0.2.2/LICENSE` & `goodboy_sqlalchemy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `goodboy_sqlalchemy-0.2.2/pyproject.toml` & `goodboy_sqlalchemy-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goodboy-sqlalchemy"
-version = "0.2.2"
+version = "0.2.3"
 description = "Data validation tool for SQLALchemy"
 license = "MIT"
 authors = ["Maxim Andryunin <maxim.andryunin@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `goodboy_sqlalchemy-0.2.2/src/goodboy_sqlalchemy/__init__.py` & `goodboy_sqlalchemy-0.2.3/src/goodboy_sqlalchemy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Mapped,
     MappedError,
     MappedKeyBuilder,
     mapped_key_builder,
 )
 from goodboy_sqlalchemy.messages import DEFAULT_MESSAGES
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 __all__ = [
     "column_schema_builder",
     "Column",
     "ColumnBuilder",
     "ColumnBuilderError",
     "ColumnSchemaBuilder",
```

### Comparing `goodboy_sqlalchemy-0.2.2/src/goodboy_sqlalchemy/column.py` & `goodboy_sqlalchemy-0.2.3/src/goodboy_sqlalchemy/column.py`

 * *Files identical despite different names*

### Comparing `goodboy_sqlalchemy-0.2.2/src/goodboy_sqlalchemy/column_schemas.py` & `goodboy_sqlalchemy-0.2.3/src/goodboy_sqlalchemy/column_schemas.py`

 * *Files identical despite different names*

### Comparing `goodboy_sqlalchemy-0.2.2/src/goodboy_sqlalchemy/mapped.py` & `goodboy_sqlalchemy-0.2.3/src/goodboy_sqlalchemy/mapped.py`

 * *Files identical despite different names*

### Comparing `goodboy_sqlalchemy-0.2.2/src/goodboy_sqlalchemy/mapped_key.py` & `goodboy_sqlalchemy-0.2.3/src/goodboy_sqlalchemy/mapped_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     ):
         value = self._column.validate(value, typecast, context)
 
         if self._column.unique:
             query = sa_orm.Query(self._sa_mapped_class).filter(self._sa_column == value)
 
             if instance:
-                instance_pk = getattr(instance, self._sa_pk_column.name)
+                instance_pk = getattr(instance, self._sa_pk_column.key)
                 query = query.filter(self._sa_pk_column != instance_pk)
 
             exists = session.query(query.exists()).scalar()
 
             if exists:
                 raise gb.SchemaError([self._error("already_exists")])
```

### Comparing `goodboy_sqlalchemy-0.2.2/PKG-INFO` & `goodboy_sqlalchemy-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: goodboy-sqlalchemy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Data validation tool for SQLALchemy
 License: MIT
 Author: Maxim Andryunin
 Author-email: maxim.andryunin@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: goodboy (>=0.2,<0.3)
 Requires-Dist: sqlalchemy
 Requires-Dist: typing-extensions (>=4.0) ; python_version >= "3.6" and python_version < "3.8"
 Description-Content-Type: text/markdown
 
 # Goodboy-SQLAlchemy: Data Validation for SQLAlchemy
```

