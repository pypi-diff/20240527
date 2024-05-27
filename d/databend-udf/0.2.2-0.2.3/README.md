# Comparing `tmp/databend-udf-0.2.2.tar.gz` & `tmp/databend_udf-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databend-udf-0.2.2.tar", last modified: Mon Feb 19 00:29:31 2024, max compression
+gzip compressed data, was "databend_udf-0.2.3.tar", last modified: Mon May 27 04:57:27 2024, max compression
```

## Comparing `databend-udf-0.2.2.tar` & `databend_udf-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:29:31.427874 databend-udf-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-02-19 00:29:31.427874 databend-udf-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-02-19 00:29:21.000000 databend-udf-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:29:31.423874 databend-udf-0.2.2/databend_udf/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-19 00:29:21.000000 databend-udf-0.2.2/databend_udf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-02-19 00:29:21.000000 databend-udf-0.2.2/databend_udf/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:29:31.423874 databend-udf-0.2.2/databend_udf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-02-19 00:29:31.000000 databend-udf-0.2.2/databend_udf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-19 00:29:31.000000 databend-udf-0.2.2/databend_udf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 00:29:31.000000 databend-udf-0.2.2/databend_udf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-19 00:29:31.000000 databend-udf-0.2.2/databend_udf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-19 00:29:31.000000 databend-udf-0.2.2/databend_udf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-19 00:29:21.000000 databend-udf-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 00:29:31.427874 databend-udf-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:57:27.415497 databend_udf-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-27 04:57:27.415497 databend_udf-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-27 04:57:04.000000 databend_udf-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:57:27.415497 databend_udf-0.2.3/databend_udf/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 04:57:04.000000 databend_udf-0.2.3/databend_udf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19330 2024-05-27 04:57:04.000000 databend_udf-0.2.3/databend_udf/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:57:27.415497 databend_udf-0.2.3/databend_udf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-27 04:57:27.000000 databend_udf-0.2.3/databend_udf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-27 04:57:27.000000 databend_udf-0.2.3/databend_udf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:57:27.000000 databend_udf-0.2.3/databend_udf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 04:57:27.000000 databend_udf-0.2.3/databend_udf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 04:57:27.000000 databend_udf-0.2.3/databend_udf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-27 04:57:04.000000 databend_udf-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 04:57:27.415497 databend_udf-0.2.3/setup.cfg
```

### Comparing `databend-udf-0.2.2/PKG-INFO` & `databend_udf-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-udf
-Version: 0.2.2
+Version: 0.2.3
 Summary: Databend UDF Server
 License: Apache-2.0
 Project-URL: Repository, https://github.com/datafuselabs/databend-udf
 Project-URL: Homepage, https://databend.rs
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `databend-udf-0.2.2/README.md` & `databend_udf-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `databend-udf-0.2.2/databend_udf/udf.py` & `databend_udf-0.2.3/databend_udf/udf.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     _func: Callable
     _io_threads: Optional[int]
     _executor: Optional[ThreadPoolExecutor]
     _skip_null: bool
 
     def __init__(
-        self, func, input_types, result_type, name=None, io_threads=None, skip_null=None
+        self, func, input_types, result_type, name=None, io_threads=32, skip_null=None
     ):
         self._func = func
         self._input_schema = pa.schema(
             field.with_name(arg_name)
             for arg_name, field in zip(
                 inspect.getfullargspec(func)[0],
                 [_to_arrow_field(t) for t in _to_list(input_types)],
```

### Comparing `databend-udf-0.2.2/databend_udf.egg-info/PKG-INFO` & `databend_udf-0.2.3/databend_udf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-udf
-Version: 0.2.2
+Version: 0.2.3
 Summary: Databend UDF Server
 License: Apache-2.0
 Project-URL: Repository, https://github.com/datafuselabs/databend-udf
 Project-URL: Homepage, https://databend.rs
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `databend-udf-0.2.2/pyproject.toml` & `databend_udf-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 description = "Databend UDF Server"
 license = { text = "Apache-2.0" }
 name = "databend-udf"
-version = "0.2.2"
+version = "0.2.3"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["pyarrow"]
 
 [project.optional-dependencies]
 lint = ["ruff"]
```

