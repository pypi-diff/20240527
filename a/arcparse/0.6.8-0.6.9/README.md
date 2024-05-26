# Comparing `tmp/arcparse-0.6.8.tar.gz` & `tmp/arcparse-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcparse-0.6.8.tar", max compression
+gzip compressed data, was "arcparse-0.6.9.tar", max compression
```

## Comparing `arcparse-0.6.8.tar` & `arcparse-0.6.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2024-02-25 06:04:17.573985 arcparse-0.6.8/LICENSE
--rw-r--r--   0        0        0     8072 2024-02-25 06:04:55.273972 arcparse-0.6.8/README.md
--rw-r--r--   0        0        0      547 2024-02-25 06:04:55.273972 arcparse-0.6.8/arcparse/__init__.py
--rw-r--r--   0        0        0     4544 2024-02-25 06:18:27.403808 arcparse-0.6.8/arcparse/_argument_helpers.py
--rw-r--r--   0        0        0     7358 2024-02-25 06:09:33.723910 arcparse-0.6.8/arcparse/_partial_arguments.py
--rw-r--r--   0        0        0     1572 2024-02-25 06:04:17.573985 arcparse-0.6.8/arcparse/_typehints.py
--rw-r--r--   0        0        0     5271 2024-02-25 06:09:33.723910 arcparse-0.6.8/arcparse/arguments.py
--rw-r--r--   0        0        0     1407 2024-02-25 06:04:17.573985 arcparse-0.6.8/arcparse/converters.py
--rw-r--r--   0        0        0      195 2024-02-25 06:04:17.573985 arcparse-0.6.8/arcparse/errors.py
--rw-r--r--   0        0        0     8537 2024-02-25 06:04:55.273972 arcparse-0.6.8/arcparse/parser.py
--rw-r--r--   0        0        0        0 2024-02-25 06:04:17.573985 arcparse-0.6.8/arcparse/py.typed
--rw-r--r--   0        0        0      894 2024-02-25 06:18:27.403808 arcparse-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     8780 1970-01-01 00:00:00.000000 arcparse-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-02-25 06:04:17.573985 arcparse-0.6.9/LICENSE
+-rw-r--r--   0        0        0     8072 2024-02-25 06:04:55.273972 arcparse-0.6.9/README.md
+-rw-r--r--   0        0        0      547 2024-02-25 06:04:55.273972 arcparse-0.6.9/arcparse/__init__.py
+-rw-r--r--   0        0        0     4549 2024-02-25 06:29:11.093706 arcparse-0.6.9/arcparse/_argument_helpers.py
+-rw-r--r--   0        0        0     7358 2024-02-25 06:09:33.723910 arcparse-0.6.9/arcparse/_partial_arguments.py
+-rw-r--r--   0        0        0     1572 2024-02-25 06:04:17.573985 arcparse-0.6.9/arcparse/_typehints.py
+-rw-r--r--   0        0        0     5271 2024-02-25 06:09:33.723910 arcparse-0.6.9/arcparse/arguments.py
+-rw-r--r--   0        0        0     1407 2024-02-25 06:04:17.573985 arcparse-0.6.9/arcparse/converters.py
+-rw-r--r--   0        0        0      195 2024-02-25 06:04:17.573985 arcparse-0.6.9/arcparse/errors.py
+-rw-r--r--   0        0        0     8537 2024-02-25 06:04:55.273972 arcparse-0.6.9/arcparse/parser.py
+-rw-r--r--   0        0        0        0 2024-02-25 06:04:17.573985 arcparse-0.6.9/arcparse/py.typed
+-rw-r--r--   0        0        0      894 2024-02-25 06:30:40.913683 arcparse-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     8780 1970-01-01 00:00:00.000000 arcparse-0.6.9/PKG-INFO
```

### Comparing `arcparse-0.6.8/LICENSE` & `arcparse-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arcparse-0.6.8/README.md` & `arcparse-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `arcparse-0.6.8/arcparse/__init__.py` & `arcparse-0.6.9/arcparse/__init__.py`

 * *Files identical despite different names*

### Comparing `arcparse-0.6.8/arcparse/_argument_helpers.py` & `arcparse-0.6.9/arcparse/_argument_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     PartialTriFlag,
 )
 from .arguments import Void, void
 
 
 def _check_short_format(short: str) -> None:
     if not re.match(r"^-[^-]+$", short):
-        raise InvalidArgument(f"Invalid argument short-hand \"{}\", expected a dash followed by non-dash characters")
+        raise InvalidArgument(f"Invalid argument short-hand \"{short}\", expected a dash followed by non-dash characters")
 
 
 def positional[T](
     *,
     default: T | str | Void = void,
     choices: Collection[str] | None = None,
     converter: Callable[[str], T] | None = None,
```

### Comparing `arcparse-0.6.8/arcparse/_partial_arguments.py` & `arcparse-0.6.9/arcparse/_partial_arguments.py`

 * *Files identical despite different names*

### Comparing `arcparse-0.6.8/arcparse/_typehints.py` & `arcparse-0.6.9/arcparse/_typehints.py`

 * *Files identical despite different names*

### Comparing `arcparse-0.6.8/arcparse/arguments.py` & `arcparse-0.6.9/arcparse/arguments.py`

 * *Files identical despite different names*

### Comparing `arcparse-0.6.8/arcparse/converters.py` & `arcparse-0.6.9/arcparse/converters.py`

 * *Files identical despite different names*

### Comparing `arcparse-0.6.8/arcparse/parser.py` & `arcparse-0.6.9/arcparse/parser.py`

 * *Files identical despite different names*

### Comparing `arcparse-0.6.8/pyproject.toml` & `arcparse-0.6.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arcparse"
-version = "0.6.8"
+version = "0.6.9"
 description = "Declare program arguments declaratively and type-safely"
 license = "MIT"
 authors = ["Jakub Rozek <jakub.rozek314@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Kuba314/arcparse"
 keywords = ["argparse", "declarative", "argument", "parsing", "type-safe"]
 classifiers = [
```

### Comparing `arcparse-0.6.8/PKG-INFO` & `arcparse-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcparse
-Version: 0.6.8
+Version: 0.6.9
 Summary: Declare program arguments declaratively and type-safely
 Home-page: https://github.com/Kuba314/arcparse
 License: MIT
 Keywords: argparse,declarative,argument,parsing,type-safe
 Author: Jakub Rozek
 Author-email: jakub.rozek314@gmail.com
 Requires-Python: >=3.12,<4.0
```

