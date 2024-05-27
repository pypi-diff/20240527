# Comparing `tmp/pysql-repo-0.7.3.2.tar.gz` & `tmp/pysql-repo-0.7.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysql-repo-0.7.3.2.tar", last modified: Wed May 22 21:58:15 2024, max compression
+gzip compressed data, was "pysql-repo-0.7.3.3.tar", last modified: Mon May 27 09:45:41 2024, max compression
```

## Comparing `pysql-repo-0.7.3.2.tar` & `pysql-repo-0.7.3.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:58:15.713587 pysql-repo-0.7.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    41380 2024-05-22 21:58:15.713587 pysql-repo-0.7.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    40736 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:58:15.713587 pysql-repo-0.7.3.2/pysql_repo/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:58:15.713587 pysql-repo-0.7.3.2/pysql_repo/_constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/_constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/_constants/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/_database_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    23747 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:58:15.713587 pysql-repo-0.7.3.2/pysql_repo/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/asyncio/async_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/asyncio/async_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19656 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/asyncio/async_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/asyncio/async_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:58:15.713587 pysql-repo-0.7.3.2/pysql_repo/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:58:13.000000 pysql-repo-0.7.3.2/pysql_repo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:58:15.713587 pysql-repo-0.7.3.2/pysql_repo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41380 2024-05-22 21:58:15.000000 pysql-repo-0.7.3.2/pysql_repo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-22 21:58:15.000000 pysql-repo-0.7.3.2/pysql_repo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:58:15.000000 pysql-repo-0.7.3.2/pysql_repo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 21:58:15.000000 pysql-repo-0.7.3.2/pysql_repo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 21:58:15.000000 pysql-repo-0.7.3.2/pysql_repo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:58:15.713587 pysql-repo-0.7.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-22 21:58:14.000000 pysql-repo-0.7.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:41.962936 pysql-repo-0.7.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    41380 2024-05-27 09:45:41.962936 pysql-repo-0.7.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    40736 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:41.962936 pysql-repo-0.7.3.3/pysql_repo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:41.962936 pysql-repo-0.7.3.3/pysql_repo/_constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/_constants/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/_database_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23115 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:41.962936 pysql-repo-0.7.3.3/pysql_repo/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/asyncio/async_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/asyncio/async_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19656 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/asyncio/async_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/asyncio/async_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:41.962936 pysql-repo-0.7.3.3/pysql_repo/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:38.000000 pysql-repo-0.7.3.3/pysql_repo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:41.962936 pysql-repo-0.7.3.3/pysql_repo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41380 2024-05-27 09:45:41.000000 pysql-repo-0.7.3.3/pysql_repo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-27 09:45:41.000000 pysql-repo-0.7.3.3/pysql_repo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:45:41.000000 pysql-repo-0.7.3.3/pysql_repo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 09:45:41.000000 pysql-repo-0.7.3.3/pysql_repo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 09:45:41.000000 pysql-repo-0.7.3.3/pysql_repo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 09:45:41.962936 pysql-repo-0.7.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-27 09:45:40.000000 pysql-repo-0.7.3.3/setup.py
```

### Comparing `pysql-repo-0.7.3.2/PKG-INFO` & `pysql-repo-0.7.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysql-repo
-Version: 0.7.3.2
+Version: 0.7.3.3
 Summary: A project to have a base repository class to perform select/insert/update/delete with dynamic syntax
 Home-page: https://github.com/Impro02/pysql-repo
-Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.7.3.2.tar.gz
+Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.7.3.3.tar.gz
 Author: Maxime MARTIN
 Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysql-repo-0.7.3.2/README.md` & `pysql-repo-0.7.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo/__init__.py` & `pysql-repo-0.7.3.3/pysql_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo/_constants/enum.py` & `pysql-repo-0.7.3.3/pysql_repo/_constants/enum.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo/_database.py` & `pysql-repo-0.7.3.3/pysql_repo/_database.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo/_database_base.py` & `pysql-repo-0.7.3.3/pysql_repo/_database_base.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo/_decorators.py` & `pysql-repo-0.7.3.3/pysql_repo/_decorators.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo/_repository.py` & `pysql-repo-0.7.3.3/pysql_repo/_repository.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo/_service.py` & `pysql-repo-0.7.3.3/pysql_repo/_service.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo/_utils.py` & `pysql-repo-0.7.3.3/pysql_repo/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from sqlalchemy.sql.dml import ReturningDelete, ReturningInsert, ReturningUpdate
 from sqlalchemy.sql.elements import Null, BinaryExpression
 
 # Enum
 from pysql_repo._constants.enum import LoadingTechnique, Operators
 
 FilterType: TypeAlias = Dict[
-    Union[InstrumentedAttribute[Any], Tuple[InstrumentedAttribute[Any]]], Any
+    Union[InstrumentedAttribute[Any], Tuple[InstrumentedAttribute[Any], ...]], Any
 ]
 
 _T = TypeVar("_T", bound=DeclarativeBase)
 
 _T_SELECT_UPDATE = TypeVar("_T_SELECT_UPDATE", bound=Union[Select[Any], Update])
 
 _T_SELECT_UPDATE_DELETE = TypeVar(
@@ -506,58 +506,62 @@
         values (dict): A dictionary containing the filter conditions.
         with_optional (bool, optional): Whether to include optional conditions with a value of None. Defaults to False.
 
     Returns:
         List[ColumnExpressionArgument]: A list of SQLAlchemy conditions.
 
     """
+
+    def is_value_null(value: Any) -> bool:
+        return value is None or isinstance(value, Null)
+
     conditions = []
     for key, value in values.items():
         if type(value) is set:
             value = list(value)
         elif type(value) is dict:
             for k, v in value.items():
                 if with_optional and v is None:
                     continue
 
                 match k:
                     case Operators.EQUAL:
                         conditions.append(key == v)
                     case Operators.IEQUAL:
-                        if not isinstance(v, Null):
+                        if not is_value_null(v):
                             conditions.append(func.lower(key) == func.lower(v))
                         else:
                             conditions.append(key == v)
                     case Operators.DIFFERENT:
                         conditions.append(key != v)
                     case Operators.IDIFFERENT:
-                        if not isinstance(v, Null):
+                        if not is_value_null(v):
                             conditions.append(func.lower(key) != func.lower(v))
                         else:
                             conditions.append(key != v)
                     case Operators.LIKE:
-                        if not isinstance(v, Null):
+                        if not is_value_null(v):
                             if isinstance(key, InstrumentedAttribute):
                                 conditions.append(key.like(v))
                         else:
                             conditions.append(key == v)
                     case Operators.NOT_LIKE:
-                        if not isinstance(v, Null):
+                        if not is_value_null(v):
                             if isinstance(key, InstrumentedAttribute):
                                 conditions.append(~key.like(v))
                         else:
                             conditions.append(key != v)
                     case Operators.ILIKE:
-                        if not isinstance(v, Null):
+                        if not is_value_null(v):
                             if isinstance(key, InstrumentedAttribute):
                                 conditions.append(key.ilike(v))
                         else:
                             conditions.append(key == v)
                     case Operators.NOT_ILIKE:
-                        if not isinstance(v, Null):
+                        if not is_value_null(v):
                             if isinstance(key, InstrumentedAttribute):
                                 conditions.append(~key.ilike(v))
                         else:
                             conditions.append(key != v)
                     case Operators.BETWEEN:
                         if len(v) != 2:
                             continue
@@ -588,32 +592,24 @@
                             conditions.append(key.in_(v))
                     case Operators.IIN:
                         v = v if isinstance(v, Iterable) else [v]
                         if isinstance(key, tuple):
                             conditions.append(
                                 tuple_(*(func.lower(key_) for key_ in key)).in_(
                                     [
-                                        (
-                                            func.lower(v_)
-                                            if not isinstance(v_, Null)
-                                            else v_
-                                        )
+                                        func.lower(v_) if not is_value_null(v) else v_
                                         for v_ in v
                                     ]
                                 )
                             )
                         else:
                             conditions.append(
                                 func.lower(key).in_(
                                     [
-                                        (
-                                            func.lower(v_)
-                                            if not isinstance(v_, Null)
-                                            else v_
-                                        )
+                                        func.lower(v_) if not is_value_null(v) else v_
                                         for v_ in v
                                     ]
                                 )
                             )
                     case Operators.NOT_IN:
                         v = v if isinstance(v, Iterable) else [v]
                         if isinstance(key, tuple):
@@ -623,32 +619,24 @@
 
                     case Operators.NOT_IIN:
                         v = v if isinstance(v, Iterable) else [v]
                         if isinstance(key, tuple):
                             conditions.append(
                                 tuple_(*(func.lower(key_) for key_ in key)).notin_(
                                     [
-                                        (
-                                            func.lower(v_)
-                                            if not isinstance(v_, Null)
-                                            else v_
-                                        )
+                                        func.lower(v_) if not is_value_null(v) else v_
                                         for v_ in v
                                     ]
                                 )
                             )
                         else:
                             conditions.append(
                                 func.lower(key).notin_(
                                     [
-                                        (
-                                            func.lower(v_)
-                                            if not isinstance(v_, Null)
-                                            else v_
-                                        )
+                                        func.lower(v_) if not is_value_null(v) else v_
                                         for v_ in v
                                     ]
                                 )
                             )
                     case Operators.HAS:
                         v = get_filters(
                             v,
```

### Comparing `pysql-repo-0.7.3.2/pysql_repo/asyncio/async_database.py` & `pysql-repo-0.7.3.3/pysql_repo/asyncio/async_database.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo/asyncio/async_decorator.py` & `pysql-repo-0.7.3.3/pysql_repo/asyncio/async_decorator.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo/asyncio/async_repository.py` & `pysql-repo-0.7.3.3/pysql_repo/asyncio/async_repository.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo/asyncio/async_service.py` & `pysql-repo-0.7.3.3/pysql_repo/asyncio/async_service.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo/libs/file_lib.py` & `pysql-repo-0.7.3.3/pysql_repo/libs/file_lib.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/pysql_repo.egg-info/PKG-INFO` & `pysql-repo-0.7.3.3/pysql_repo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysql-repo
-Version: 0.7.3.2
+Version: 0.7.3.3
 Summary: A project to have a base repository class to perform select/insert/update/delete with dynamic syntax
 Home-page: https://github.com/Impro02/pysql-repo
-Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.7.3.2.tar.gz
+Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.7.3.3.tar.gz
 Author: Maxime MARTIN
 Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysql-repo-0.7.3.2/pysql_repo.egg-info/SOURCES.txt` & `pysql-repo-0.7.3.3/pysql_repo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.3.2/setup.py` & `pysql-repo-0.7.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "0.7.3.2"
+version = "0.7.3.3"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="pysql-repo",
     version=version,
```

