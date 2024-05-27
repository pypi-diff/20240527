# Comparing `tmp/pyshared-1.5.9.tar.gz` & `tmp/pyshared-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyshared-1.5.9.tar", last modified: Fri May 17 15:17:45 2024, max compression
+gzip compressed data, was "pyshared-1.6.0.tar", last modified: Mon May 27 00:37:36 2024, max compression
```

## Comparing `pyshared-1.5.9.tar` & `pyshared-1.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-17 15:17:45.156407 pyshared-1.5.9/
--rw-r--r--   0 mym2       (501) staff       (20)     1068 2024-01-11 01:41:50.000000 pyshared-1.5.9/LICENSE
--rw-r--r--   0 mym2       (501) staff       (20)     7001 2024-05-17 15:17:45.156138 pyshared-1.5.9/PKG-INFO
--rw-r--r--   0 mym2       (501) staff       (20)     3963 2024-04-23 06:16:19.000000 pyshared-1.5.9/README.md
--rw-r--r--   0 mym2       (501) staff       (20)     1740 2024-05-16 01:16:38.000000 pyshared-1.5.9/pyproject.toml
-drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-17 15:17:45.154345 pyshared-1.5.9/pyshared/
--rw-r--r--   0 mym2       (501) staff       (20)      759 2024-05-02 17:09:02.000000 pyshared-1.5.9/pyshared/__init__.py
--rw-r--r--   0 mym2       (501) staff       (20)      124 2024-01-11 01:53:35.000000 pyshared-1.5.9/pyshared/consts.py
--rw-r--r--   0 mym2       (501) staff       (20)     1293 2024-01-12 03:28:53.000000 pyshared-1.5.9/pyshared/crypto.py
--rw-r--r--   0 mym2       (501) staff       (20)     2029 2024-04-03 16:31:09.000000 pyshared-1.5.9/pyshared/env.py
--rw-r--r--   0 mym2       (501) staff       (20)      943 2024-03-31 21:02:23.000000 pyshared-1.5.9/pyshared/exceptions.py
--rw-r--r--   0 mym2       (501) staff       (20)     2120 2024-05-05 14:26:20.000000 pyshared-1.5.9/pyshared/log.py
--rw-r--r--   0 mym2       (501) staff       (20)      936 2024-04-12 00:40:19.000000 pyshared-1.5.9/pyshared/pytest.py
--rw-r--r--   0 mym2       (501) staff       (20)     5650 2024-05-05 09:51:40.000000 pyshared-1.5.9/pyshared/python.py
--rw-r--r--   0 mym2       (501) staff       (20)      790 2024-01-11 05:57:29.000000 pyshared-1.5.9/pyshared/shell.py
--rw-r--r--   0 mym2       (501) staff       (20)     2083 2024-01-12 03:45:28.000000 pyshared-1.5.9/pyshared/terminal.py
--rw-r--r--   0 mym2       (501) staff       (20)     2792 2024-04-18 06:32:58.000000 pyshared-1.5.9/pyshared/test.py
--rw-r--r--   0 mym2       (501) staff       (20)       22 2024-05-16 01:16:38.000000 pyshared-1.5.9/pyshared/version.py
-drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-17 15:17:45.155333 pyshared-1.5.9/pyshared.egg-info/
--rw-r--r--   0 mym2       (501) staff       (20)     7001 2024-05-17 15:17:45.000000 pyshared-1.5.9/pyshared.egg-info/PKG-INFO
--rw-r--r--   0 mym2       (501) staff       (20)      419 2024-05-17 15:17:45.000000 pyshared-1.5.9/pyshared.egg-info/SOURCES.txt
--rw-r--r--   0 mym2       (501) staff       (20)        1 2024-05-17 15:17:45.000000 pyshared-1.5.9/pyshared.egg-info/dependency_links.txt
--rw-r--r--   0 mym2       (501) staff       (20)       68 2024-05-17 15:17:45.000000 pyshared-1.5.9/pyshared.egg-info/requires.txt
--rw-r--r--   0 mym2       (501) staff       (20)        9 2024-05-17 15:17:45.000000 pyshared-1.5.9/pyshared.egg-info/top_level.txt
--rw-r--r--   0 mym2       (501) staff       (20)       38 2024-05-17 15:17:45.156458 pyshared-1.5.9/setup.cfg
+drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-27 00:37:36.269119 pyshared-1.6.0/
+-rw-r--r--   0 mym2       (501) staff       (20)     1068 2024-01-11 01:41:50.000000 pyshared-1.6.0/LICENSE
+-rw-r--r--   0 mym2       (501) staff       (20)     7318 2024-05-27 00:37:36.268927 pyshared-1.6.0/PKG-INFO
+-rw-r--r--   0 mym2       (501) staff       (20)     4280 2024-05-27 00:27:08.000000 pyshared-1.6.0/README.md
+-rw-r--r--   0 mym2       (501) staff       (20)     1740 2024-05-27 00:37:30.000000 pyshared-1.6.0/pyproject.toml
+drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-27 00:37:36.267670 pyshared-1.6.0/pyshared/
+-rw-r--r--   0 mym2       (501) staff       (20)      860 2024-05-26 22:51:48.000000 pyshared-1.6.0/pyshared/__init__.py
+-rw-r--r--   0 mym2       (501) staff       (20)      124 2024-01-11 01:53:35.000000 pyshared-1.6.0/pyshared/consts.py
+-rw-r--r--   0 mym2       (501) staff       (20)     1293 2024-01-12 03:28:53.000000 pyshared-1.6.0/pyshared/crypto.py
+-rw-r--r--   0 mym2       (501) staff       (20)     2029 2024-04-03 16:31:09.000000 pyshared-1.6.0/pyshared/env.py
+-rw-r--r--   0 mym2       (501) staff       (20)      943 2024-03-31 21:02:23.000000 pyshared-1.6.0/pyshared/exceptions.py
+-rw-r--r--   0 mym2       (501) staff       (20)     2120 2024-05-05 14:26:20.000000 pyshared-1.6.0/pyshared/log.py
+-rw-r--r--   0 mym2       (501) staff       (20)      936 2024-04-12 00:40:19.000000 pyshared-1.6.0/pyshared/pytest.py
+-rw-r--r--   0 mym2       (501) staff       (20)    10270 2024-05-27 00:27:31.000000 pyshared-1.6.0/pyshared/python.py
+-rw-r--r--   0 mym2       (501) staff       (20)      790 2024-01-11 05:57:29.000000 pyshared-1.6.0/pyshared/shell.py
+-rw-r--r--   0 mym2       (501) staff       (20)     2083 2024-01-12 03:45:28.000000 pyshared-1.6.0/pyshared/terminal.py
+-rw-r--r--   0 mym2       (501) staff       (20)     2792 2024-04-18 06:32:58.000000 pyshared-1.6.0/pyshared/test.py
+-rw-r--r--   0 mym2       (501) staff       (20)       22 2024-05-27 00:37:30.000000 pyshared-1.6.0/pyshared/version.py
+drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-27 00:37:36.268453 pyshared-1.6.0/pyshared.egg-info/
+-rw-r--r--   0 mym2       (501) staff       (20)     7318 2024-05-27 00:37:36.000000 pyshared-1.6.0/pyshared.egg-info/PKG-INFO
+-rw-r--r--   0 mym2       (501) staff       (20)      419 2024-05-27 00:37:36.000000 pyshared-1.6.0/pyshared.egg-info/SOURCES.txt
+-rw-r--r--   0 mym2       (501) staff       (20)        1 2024-05-27 00:37:36.000000 pyshared-1.6.0/pyshared.egg-info/dependency_links.txt
+-rw-r--r--   0 mym2       (501) staff       (20)       68 2024-05-27 00:37:36.000000 pyshared-1.6.0/pyshared.egg-info/requires.txt
+-rw-r--r--   0 mym2       (501) staff       (20)        9 2024-05-27 00:37:36.000000 pyshared-1.6.0/pyshared.egg-info/top_level.txt
+-rw-r--r--   0 mym2       (501) staff       (20)       38 2024-05-27 00:37:36.269165 pyshared-1.6.0/setup.cfg
```

### Comparing `pyshared-1.5.9/LICENSE` & `pyshared-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyshared-1.5.9/PKG-INFO` & `pyshared-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshared
-Version: 1.5.9
+Version: 1.6.0
 Summary: A Python library containing common utility functions for use across multiple codebases, filling gaps not covered by the standard Python libraries.
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Cary Carter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -129,17 +129,21 @@
 
 ### `exceptions.py`
 
 - `NotPrintableError`: Both str and repr methods raised exceptions.
 
 ### `python.py`
 
+- `HumanTime`: A class for converting seconds to human-readable time strings.
+- `UniqueList`: A list that only allows unique elements.
+- `default_repr`: Generates a default representation for custom objects.
+- `htime`: A function for converting seconds to human-readable time strings.
 - `ranstr`: Creates random strings of specified length and character set.
 - `safe_repr`: Safely returns the object's repr/str or an error string without throwing exceptions if the object is not printable.
-- `default_repr`: Generates a default representation for custom objects.
+- `tmp_pythonpath`: Adds a temporary directory to the Python path for the duration of a context manager.
 - `truncstr`: Truncates a string, preserving a portion from the start and/or end.
 
 ### `pytest.py`
 
 - `multiscope_fixture`: Creates multiple scoped pytest fixture and ensures the fixtures are available in the module.
 
 ### `shell.py`
```

### Comparing `pyshared-1.5.9/README.md` & `pyshared-1.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -65,17 +65,21 @@
 
 ### `exceptions.py`
 
 - `NotPrintableError`: Both str and repr methods raised exceptions.
 
 ### `python.py`
 
+- `HumanTime`: A class for converting seconds to human-readable time strings.
+- `UniqueList`: A list that only allows unique elements.
+- `default_repr`: Generates a default representation for custom objects.
+- `htime`: A function for converting seconds to human-readable time strings.
 - `ranstr`: Creates random strings of specified length and character set.
 - `safe_repr`: Safely returns the object's repr/str or an error string without throwing exceptions if the object is not printable.
-- `default_repr`: Generates a default representation for custom objects.
+- `tmp_pythonpath`: Adds a temporary directory to the Python path for the duration of a context manager.
 - `truncstr`: Truncates a string, preserving a portion from the start and/or end.
 
 ### `pytest.py`
 
 - `multiscope_fixture`: Creates multiple scoped pytest fixture and ensures the fixtures are available in the module.
 
 ### `shell.py`
```

### Comparing `pyshared-1.5.9/pyproject.toml` & `pyshared-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "flake8",
     "twine",
     "build",
 ]
 
 [project]
 name = "pyshared"
-version = "1.5.9"
+version = "1.6.0"
 authors = [{name = "Cary Carter", email = "ccarterdev@gmail.com"}]
 description = "A Python library containing common utility functions for use across multiple codebases, filling gaps not covered by the standard Python libraries."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 
 classifiers = [
```

### Comparing `pyshared-1.5.9/pyshared/crypto.py` & `pyshared-1.6.0/pyshared/crypto.py`

 * *Files identical despite different names*

### Comparing `pyshared-1.5.9/pyshared/env.py` & `pyshared-1.6.0/pyshared/env.py`

 * *Files identical despite different names*

### Comparing `pyshared-1.5.9/pyshared/exceptions.py` & `pyshared-1.6.0/pyshared/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyshared-1.5.9/pyshared/log.py` & `pyshared-1.6.0/pyshared/log.py`

 * *Files identical despite different names*

### Comparing `pyshared-1.5.9/pyshared/pytest.py` & `pyshared-1.6.0/pyshared/pytest.py`

 * *Files identical despite different names*

### Comparing `pyshared-1.5.9/pyshared/shell.py` & `pyshared-1.6.0/pyshared/shell.py`

 * *Files identical despite different names*

### Comparing `pyshared-1.5.9/pyshared/terminal.py` & `pyshared-1.6.0/pyshared/terminal.py`

 * *Files identical despite different names*

### Comparing `pyshared-1.5.9/pyshared/test.py` & `pyshared-1.6.0/pyshared/test.py`

 * *Files identical despite different names*

### Comparing `pyshared-1.5.9/pyshared.egg-info/PKG-INFO` & `pyshared-1.6.0/pyshared.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshared
-Version: 1.5.9
+Version: 1.6.0
 Summary: A Python library containing common utility functions for use across multiple codebases, filling gaps not covered by the standard Python libraries.
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Cary Carter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -129,17 +129,21 @@
 
 ### `exceptions.py`
 
 - `NotPrintableError`: Both str and repr methods raised exceptions.
 
 ### `python.py`
 
+- `HumanTime`: A class for converting seconds to human-readable time strings.
+- `UniqueList`: A list that only allows unique elements.
+- `default_repr`: Generates a default representation for custom objects.
+- `htime`: A function for converting seconds to human-readable time strings.
 - `ranstr`: Creates random strings of specified length and character set.
 - `safe_repr`: Safely returns the object's repr/str or an error string without throwing exceptions if the object is not printable.
-- `default_repr`: Generates a default representation for custom objects.
+- `tmp_pythonpath`: Adds a temporary directory to the Python path for the duration of a context manager.
 - `truncstr`: Truncates a string, preserving a portion from the start and/or end.
 
 ### `pytest.py`
 
 - `multiscope_fixture`: Creates multiple scoped pytest fixture and ensures the fixtures are available in the module.
 
 ### `shell.py`
```

