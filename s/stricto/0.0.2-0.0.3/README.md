# Comparing `tmp/stricto-0.0.2.tar.gz` & `tmp/stricto-0.0.3.tar.gz`

## Comparing `stricto-0.0.2.tar` & `stricto-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,32 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stricto-0.0.2/requirements.txt
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 stricto-0.0.2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 stricto-0.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 stricto-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0    20896 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_a44f0ac069e85531_test_bool_py.html
--rw-r--r--   0        0        0   102817 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_a44f0ac069e85531_test_dict_py.html
--rw-r--r--   0        0        0    14092 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_a44f0ac069e85531_test_error_py.html
--rw-r--r--   0        0        0    54313 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_a44f0ac069e85531_test_float_py.html
--rw-r--r--   0        0        0    28268 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_a44f0ac069e85531_test_in_py.html
--rw-r--r--   0        0        0    60379 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_a44f0ac069e85531_test_int_py.html
--rw-r--r--   0        0        0   101229 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_a44f0ac069e85531_test_list_py.html
--rw-r--r--   0        0        0    43004 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_a44f0ac069e85531_test_string_py.html
--rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_f495c9c796458a5c___init___py.html
--rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_f495c9c796458a5c_bool_py.html
--rw-r--r--   0        0        0    69739 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_f495c9c796458a5c_dict_py.html
--rw-r--r--   0        0        0    16224 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_f495c9c796458a5c_error_py.html
--rw-r--r--   0        0        0    14956 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_f495c9c796458a5c_float_py.html
--rw-r--r--   0        0        0   109229 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_f495c9c796458a5c_generic_py.html
--rw-r--r--   0        0        0    13129 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_f495c9c796458a5c_in_type_py.html
--rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_f495c9c796458a5c_int_py.html
--rw-r--r--   0        0        0    93174 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_f495c9c796458a5c_list_py.html
--rw-r--r--   0        0        0    15667 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_f495c9c796458a5c_string_py.html
--rw-r--r--   0        0        0    11031 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/d_f495c9c796458a5c_time_stamp_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/status.json
--rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 stricto-0.0.2/htmlcov/style.css
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 stricto-0.0.2/stricto/__init__.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 stricto-0.0.2/stricto/bool.py
--rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 stricto-0.0.2/stricto/dict.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 stricto-0.0.2/stricto/error.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 stricto-0.0.2/stricto/float.py
--rw-r--r--   0        0        0    11172 2020-02-02 00:00:00.000000 stricto-0.0.2/stricto/generic.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 stricto-0.0.2/stricto/in_type.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 stricto-0.0.2/stricto/int.py
--rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 stricto-0.0.2/stricto/list.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 stricto-0.0.2/stricto/string.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stricto-0.0.2/tests/__init__.py
--rwxr-xr-x   0        0        0     1458 2020-02-02 00:00:00.000000 stricto-0.0.2/tests/test_bool.py
--rwxr-xr-x   0        0        0     8439 2020-02-02 00:00:00.000000 stricto-0.0.2/tests/test_dict.py
--rwxr-xr-x   0        0        0     1059 2020-02-02 00:00:00.000000 stricto-0.0.2/tests/test_error.py
--rwxr-xr-x   0        0        0     4664 2020-02-02 00:00:00.000000 stricto-0.0.2/tests/test_float.py
--rwxr-xr-x   0        0        0     1987 2020-02-02 00:00:00.000000 stricto-0.0.2/tests/test_in.py
--rwxr-xr-x   0        0        0     5203 2020-02-02 00:00:00.000000 stricto-0.0.2/tests/test_int.py
--rwxr-xr-x   0        0        0     8158 2020-02-02 00:00:00.000000 stricto-0.0.2/tests/test_list.py
--rwxr-xr-x   0        0        0     3573 2020-02-02 00:00:00.000000 stricto-0.0.2/tests/test_string.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 stricto-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 stricto-0.0.2/LICENSE
--rw-r--r--   0        0        0     8852 2020-02-02 00:00:00.000000 stricto-0.0.2/README.md
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 stricto-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 stricto-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 stricto-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 stricto-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stricto-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 stricto-0.0.3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 stricto-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 stricto-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 stricto-0.0.3/stricto/__init__.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 stricto-0.0.3/stricto/bool.py
+-rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 stricto-0.0.3/stricto/dict.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 stricto-0.0.3/stricto/error.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 stricto-0.0.3/stricto/float.py
+-rw-r--r--   0        0        0    11172 2020-02-02 00:00:00.000000 stricto-0.0.3/stricto/generic.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 stricto-0.0.3/stricto/in_type.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 stricto-0.0.3/stricto/int.py
+-rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 stricto-0.0.3/stricto/list.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 stricto-0.0.3/stricto/string.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 stricto-0.0.3/stricto/tuple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stricto-0.0.3/tests/__init__.py
+-rwxr-xr-x   0        0        0     1458 2020-02-02 00:00:00.000000 stricto-0.0.3/tests/test_bool.py
+-rwxr-xr-x   0        0        0     8715 2020-02-02 00:00:00.000000 stricto-0.0.3/tests/test_dict.py
+-rwxr-xr-x   0        0        0     1059 2020-02-02 00:00:00.000000 stricto-0.0.3/tests/test_error.py
+-rwxr-xr-x   0        0        0     4664 2020-02-02 00:00:00.000000 stricto-0.0.3/tests/test_float.py
+-rwxr-xr-x   0        0        0     1987 2020-02-02 00:00:00.000000 stricto-0.0.3/tests/test_in.py
+-rwxr-xr-x   0        0        0     5203 2020-02-02 00:00:00.000000 stricto-0.0.3/tests/test_int.py
+-rwxr-xr-x   0        0        0     8158 2020-02-02 00:00:00.000000 stricto-0.0.3/tests/test_list.py
+-rwxr-xr-x   0        0        0     3573 2020-02-02 00:00:00.000000 stricto-0.0.3/tests/test_string.py
+-rwxr-xr-x   0        0        0     7198 2020-02-02 00:00:00.000000 stricto-0.0.3/tests/test_tuple.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 stricto-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 stricto-0.0.3/LICENSE
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 stricto-0.0.3/README.md
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 stricto-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    12239 2020-02-02 00:00:00.000000 stricto-0.0.3/PKG-INFO
```

### Comparing `stricto-0.0.2/.github/workflows/pylint.yml` & `stricto-0.0.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/.github/workflows/release.yml` & `stricto-0.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/.github/workflows/test.yml` & `stricto-0.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/stricto/bool.py` & `stricto-0.0.3/stricto/bool.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/stricto/dict.py` & `stricto-0.0.3/stricto/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,16 +200,16 @@
                         self.path_name() + f".{key}",
                     )
             return
 
         if isinstance(value, Dict):
             for key in self._keys:
                 key_object = self.__dict__[key]
-                if key_object.exists() is False:
-                    continue
+                #if key_object.exists() is False:
+                #    continue
 
                 sub_value = value.get(key).get_value()
                 key_object.check(sub_value)
             return
 
     def check_type(self, value):
         """
```

### Comparing `stricto-0.0.2/stricto/error.py` & `stricto-0.0.3/stricto/error.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     """
     Specifics Errors for stricto.
     Use a ErrorType value (for future internationalisation)
     """
 
     WRONGTYPE = auto()
     NOTALIST = auto()
+    NOTATUPLE = auto()
     NOTADICT = auto()
     NOTONEOF = auto()
     NULL = auto()
     NOTATYPE = auto()
     UNKNOWNCONTENT = auto()
     NOTCALLABLE = auto()
     CONSTRAINT = auto()
```

### Comparing `stricto-0.0.2/stricto/float.py` & `stricto-0.0.3/stricto/float.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/stricto/generic.py` & `stricto-0.0.3/stricto/generic.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/stricto/in_type.py` & `stricto-0.0.3/stricto/in_type.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/stricto/int.py` & `stricto-0.0.3/stricto/int.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/stricto/list.py` & `stricto-0.0.3/stricto/list.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/stricto/string.py` & `stricto-0.0.3/stricto/string.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/tests/test_bool.py` & `stricto-0.0.3/tests/test_bool.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/tests/test_dict.py` & `stricto-0.0.3/tests/test_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,13 +289,18 @@
         with self.assertRaises(Error) as e:
             a.set({"d": 2})
         self.assertEqual(e.exception.message, "locked")
         with self.assertRaises(Error) as e:
             a.d=2
         self.assertEqual(e.exception.message, "locked")
 
+        with self.assertRaises(Error) as e:
+            a.set({'must_exists': False, 'a': 2, 'b': 1, 'c': 2, 'e': 4, 'd':2 })
+        self.assertEqual(e.exception.message, "locked")
+        self.assertEqual(repr (a), "{'must_exists': False, 'a': 2, 'b': 1, 'c': 2, 'e': 4}")
+
         a.must_exists = True
         self.assertEqual(a.get('d'), 3)
         self.assertEqual(a.get_value()['d'], 3)
         self.assertEqual(repr (a), "{'must_exists': True, 'a': 2, 'b': 1, 'c': 2, 'd': 3, 'e': 4}")
         a.set({"d": 2})
         self.assertEqual(a.d, 2)
```

### Comparing `stricto-0.0.2/tests/test_error.py` & `stricto-0.0.3/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/tests/test_float.py` & `stricto-0.0.3/tests/test_float.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/tests/test_in.py` & `stricto-0.0.3/tests/test_in.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/tests/test_int.py` & `stricto-0.0.3/tests/test_int.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/tests/test_list.py` & `stricto-0.0.3/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/tests/test_string.py` & `stricto-0.0.3/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/LICENSE` & `stricto-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stricto-0.0.2/README.md` & `stricto-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 The main difference with [jsonschema](https://github.com/python-jsonschema/jsonschema) is that the schema is directly in types of data. You don't have to *validate* them.
 
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/bwallrich/stricto
+pip install stricto
 ```
 
 ## Quickstart
 
 ```python
 from stricto import Dict, Int, String, List
 
@@ -72,14 +72,15 @@
 | - | - |
 | bool | Bool() |
 | int | Int() |
 | float | Float() |
 | string | String() |
 | list | List() |
 | dict | Dict() |
+| tuple | Tuple() |
 | | In() |
 
 ```python
 # example
 from stricto import Dict, Int
 
 a = Int()
@@ -209,14 +210,67 @@
 # function return a regexp
 a=String( pattern=lambda self, value, root : r'.*Z$')
 a.set('Allo')        # -> raise an error
 a.set('AtoZ')        # OK
 
 ```
 
+### List()
+
+```List( options )``` is for list.
+
+```List( options )``` use [generic options](#all-types).
+
+available specific options for List() ares :
+
+| Option | Default | Description |
+| - | - | - |
+| ```min=``` | None | minimum number of elements in the list |
+| ```minimum=21``` | None | similar to ```min``` |
+| ```max=99``` | None | maximum number of elements in the list |
+| ```maximum=99``` | None | similar to ```max=99``` |
+| ```uniq=True``` | None | duplicate values are forbidden |
+
+```python
+# example
+from stricto import Dict, List
+
+client = Dict{
+    "nicknames" : List( String(), default=[], uniq=True, min=0, max=3)
+}
+
+client.nicknames = [ "Ed", "Eddy", "Edward" ]  # -> raise an error
+client.nicknames = [ "Ed" ]  # -> Ok
+client.nicknames.append( "Ed" ) # -> raise an error (must be uniq)
+```
+
+### Tuple()
+
+```Tuple( options )``` is for tuple.
+
+```Tuple( options )``` use [generic options](#all-types).
+
+Ther is no available specific options for Tuple().
+
+```python
+# example
+from stricto import Dict, Tuple
+
+client = Dict{
+    "address" : Tuple( (Int(), String()) )
+}
+
+print(client.address) # -> None
+client.address = ( 12, "accacia avenue" )  # -> Ok
+client.address[1] # -> "acacia avenue"
+client.address[0] = 13  # -> raise an error like a standard tuple
+client.address = ( 13, "accacia avenue" )  # -> Ok
+
+```
+
 ### In()
 
 ```In( [ Array of types ] )``` is not a type, but an **union** of diffferent types.
 
 ```In( options )``` use [generic options](#all-types).
 
 
@@ -370,12 +424,25 @@
 a.female_infos.number_of_litter = 2 # -> Raise an Error
 
 a.gender = "Female"
 a.female_infos.number_of_litter = 2 # -> Ok
 a.female_infos # -> { "number_of_litter" : 2 }
 ```
 
-## Tests
+## Tests & co
 
 ```bash
+# all tests
 python -m unittest
+# or for only some tests
+python -m unittest tests/test_bool.py
+# or for a specific test
+
+
+# pylint
+pylint $(git ls-files '*.py')
+
+# coverage
+coverage run -m unittest
+coverage html # report under htmlcov/index.html
+
 ```
```

### Comparing `stricto-0.0.2/pyproject.toml` & `stricto-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stricto"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Bertrand Wallrich", email="Bertrand.Wallrich@inria.fr" },
 ]
 description = "Strict Dict (json) with schema validation embedded"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
```

### Comparing `stricto-0.0.2/PKG-INFO` & `stricto-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stricto
-Version: 0.0.2
+Version: 0.0.3
 Summary: Strict Dict (json) with schema validation embedded
 Project-URL: GitHub, https://github.com/NiziL/esnpy
 Project-URL: Homepage, https://github.com/bwallrich/stricto
 Project-URL: Issues, https://github.com/bwallrich/stricto/issues
 Author-email: Bertrand Wallrich <Bertrand.Wallrich@inria.fr>
 License: MIT License
         
@@ -49,15 +49,15 @@
 
 The main difference with [jsonschema](https://github.com/python-jsonschema/jsonschema) is that the schema is directly in types of data. You don't have to *validate* them.
 
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/bwallrich/stricto
+pip install stricto
 ```
 
 ## Quickstart
 
 ```python
 from stricto import Dict, Int, String, List
 
@@ -108,14 +108,15 @@
 | - | - |
 | bool | Bool() |
 | int | Int() |
 | float | Float() |
 | string | String() |
 | list | List() |
 | dict | Dict() |
+| tuple | Tuple() |
 | | In() |
 
 ```python
 # example
 from stricto import Dict, Int
 
 a = Int()
@@ -245,14 +246,67 @@
 # function return a regexp
 a=String( pattern=lambda self, value, root : r'.*Z$')
 a.set('Allo')        # -> raise an error
 a.set('AtoZ')        # OK
 
 ```
 
+### List()
+
+```List( options )``` is for list.
+
+```List( options )``` use [generic options](#all-types).
+
+available specific options for List() ares :
+
+| Option | Default | Description |
+| - | - | - |
+| ```min=``` | None | minimum number of elements in the list |
+| ```minimum=21``` | None | similar to ```min``` |
+| ```max=99``` | None | maximum number of elements in the list |
+| ```maximum=99``` | None | similar to ```max=99``` |
+| ```uniq=True``` | None | duplicate values are forbidden |
+
+```python
+# example
+from stricto import Dict, List
+
+client = Dict{
+    "nicknames" : List( String(), default=[], uniq=True, min=0, max=3)
+}
+
+client.nicknames = [ "Ed", "Eddy", "Edward" ]  # -> raise an error
+client.nicknames = [ "Ed" ]  # -> Ok
+client.nicknames.append( "Ed" ) # -> raise an error (must be uniq)
+```
+
+### Tuple()
+
+```Tuple( options )``` is for tuple.
+
+```Tuple( options )``` use [generic options](#all-types).
+
+Ther is no available specific options for Tuple().
+
+```python
+# example
+from stricto import Dict, Tuple
+
+client = Dict{
+    "address" : Tuple( (Int(), String()) )
+}
+
+print(client.address) # -> None
+client.address = ( 12, "accacia avenue" )  # -> Ok
+client.address[1] # -> "acacia avenue"
+client.address[0] = 13  # -> raise an error like a standard tuple
+client.address = ( 13, "accacia avenue" )  # -> Ok
+
+```
+
 ### In()
 
 ```In( [ Array of types ] )``` is not a type, but an **union** of diffferent types.
 
 ```In( options )``` use [generic options](#all-types).
 
 
@@ -406,12 +460,25 @@
 a.female_infos.number_of_litter = 2 # -> Raise an Error
 
 a.gender = "Female"
 a.female_infos.number_of_litter = 2 # -> Ok
 a.female_infos # -> { "number_of_litter" : 2 }
 ```
 
-## Tests
+## Tests & co
 
 ```bash
+# all tests
 python -m unittest
+# or for only some tests
+python -m unittest tests/test_bool.py
+# or for a specific test
+
+
+# pylint
+pylint $(git ls-files '*.py')
+
+# coverage
+coverage run -m unittest
+coverage html # report under htmlcov/index.html
+
 ```
```

