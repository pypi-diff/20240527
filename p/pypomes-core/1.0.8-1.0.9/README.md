# Comparing `tmp/pypomes_core-1.0.8.tar.gz` & `tmp/pypomes_core-1.0.9.tar.gz`

## Comparing `pypomes_core-1.0.8.tar` & `pypomes_core-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/PKG-INFO
```

### Comparing `pypomes_core-1.0.8/src/pypomes_core/.ruff.toml` & `pypomes_core-1.0.9/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/src/pypomes_core/__init__.py` & `pypomes_core-1.0.9/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.0.9/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.0.9/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/src/pypomes_core/email_pomes.py` & `pypomes_core-1.0.9/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.0.9/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/src/pypomes_core/env_pomes.py` & `pypomes_core-1.0.9/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.0.9/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/src/pypomes_core/file_pomes.py` & `pypomes_core-1.0.9/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/src/pypomes_core/json_pomes.py` & `pypomes_core-1.0.9/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/src/pypomes_core/list_pomes.py` & `pypomes_core-1.0.9/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/src/pypomes_core/str_pomes.py` & `pypomes_core-1.0.9/src/pypomes_core/str_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 
 def str_as_list(source: str | Any,
                 separator: str = ",") -> list[any]:
     """
     Return *source* as a *list*, by splitting its contents separated by *separator*.
 
+    The returned substrings are fully whitespace-trimmed.
     If *source* is not a *str*, then it is itself returned.
 
-    :param source: the source value to be worked on
+    :param source: the string value to be worked on
     :param separator: the separator (defaults to ",")
-    :return: a list built from the contents of the source parameter, or that parameter itself, if is not string
+    :return: a list built from the contents of the source parameter, or that parameter itself, if is not a string
     """
-    result: str | list[Any]
+    result: list[Any]
     if isinstance(source, str):
-        result = source.split(sep=separator)
+        result = [s.strip() for s in source.split(sep=separator)]
     else:
         result = source
 
     return result
 
 
 def str_sanitize(target_str: str) -> str:
@@ -147,8 +148,7 @@
     :param old: the substring to replace
     :param new: the string replacement
     :param count: the maximum number of replacements (defaults to 1)
     :return: the modified string
     """
     return source[::-1].replace(old[::-1], new[::-1], count)[::-1]
 
-
```

### Comparing `pypomes_core-1.0.8/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.0.9/src/pypomes_core/validation_msgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
         "pt": "Token de autenticação inválido",
     },
     110: {
         "en": "{}",
         "pt": "{}",
     },
     111: {
-        "en": "Unknown attribute",
-        "pt": "Atributo desconhecido",
+        "en": "Attribute is unknown or invalid in this context",
+        "pt": "Atributo desconhecido ou inválido para o contexto",
     },
     112: {
         "en": "Required attribute",
         "pt": "Atributo obrigatório",
     },
     113: {
         "en": "Attribute not applicable for {}",
```

### Comparing `pypomes_core-1.0.8/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.0.9/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.0.9/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/LICENSE` & `pypomes_core-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.8/pyproject.toml` & `pypomes_core-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-1.0.8/PKG-INFO` & `pypomes_core-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 1.0.8
+Version: 1.0.9
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

