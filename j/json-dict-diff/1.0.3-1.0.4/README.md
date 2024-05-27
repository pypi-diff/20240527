# Comparing `tmp/json_dict_diff-1.0.3.tar.gz` & `tmp/json_dict_diff-1.0.4.tar.gz`

## Comparing `json_dict_diff-1.0.3.tar` & `json_dict_diff-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/build.sh
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/json_dict_diff.py
--rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/upload.sh
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/.github/workflows/release.yaml
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/.github/workflows/test.yaml
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/tests/test.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/LICENCE
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/README.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 json_dict_diff-1.0.4/build.sh
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 json_dict_diff-1.0.4/json_dict_diff.py
+-rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 json_dict_diff-1.0.4/upload.sh
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 json_dict_diff-1.0.4/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 json_dict_diff-1.0.4/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 json_dict_diff-1.0.4/tests/test.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 json_dict_diff-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 json_dict_diff-1.0.4/LICENCE
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 json_dict_diff-1.0.4/README.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 json_dict_diff-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 json_dict_diff-1.0.4/PKG-INFO
```

### Comparing `json_dict_diff-1.0.3/json_dict_diff.py` & `json_dict_diff-1.0.4/json_dict_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     elif isinstance(a, (tuple, list, set)):
         a = list(a)
         b = list(b)
 
         if not a or not b:
             return 0.5
 
-        # Find best match witch score matrix,
+        # Find best match with score matrix,
         # remove best match and find best score again of the reduced lists
         score_matrix = []
 
         for i1, v1 in enumerate(a):
             for i2, v2 in enumerate(b):
                 score_matrix.append(((i1, i2), _similarity_score(v1, v2)))
 
@@ -120,15 +120,15 @@
             if b_found is None:
                 res.append((v1, None))
             else:
                 if (d := diff(v1, b_updated[b_found])) is not None:
                     res.append(d)
                 del b_updated[b_found]
 
-        # Add remaining elements in bas newly created
+        # Add remaining elements in b as newly created
         for v2 in b_updated:
             if v2 is not None:
                 res.append((None, v2))
 
         if not res:
             return None
 
@@ -150,60 +150,60 @@
 
         if not res:
             return None
 
         return res
 
     else:
-        raise ValidationException(f"Invalid type => [{t}]")
+        raise ValidationException(f"Invalid type => [{type(a)}]")
 
 
 def validate(a: JDict):
     """
-    This function can be used to validate the type of a JDict object at runtime,
-    If the JDict contains a invalid type, a `ValidationException` is raised.
+    This function can be used to validate the type of a JDict object at runtime.
+    If the JDict contains an invalid type, a `ValidationException` is raised.
     """
     if a is None:
         return
 
     if isinstance(a, (int, str, float, bool)):
         return
     elif isinstance(a, (tuple, list, set)):
         for v in a:
             validate(v)
     elif isinstance(a, dict):
         for k, v in a.items():
             if not isinstance(k, str):
-                raise ValidationException(f"Invalid type => [{type(a)}]")
+                raise ValidationException(f"Invalid key type => [{type(a)}], only type str accepted")
             validate(v)
     else:
         raise ValidationException(f"Invalid type => [{type(a)}]")
 
 
 def diff(a: JDict, b: JDict) -> JDict:
     """
     This function can be used to diff two dictionaries.
-    The diff is represented as a dictionary where insertions/deletions/substititons are represented as tuples.
-    E.g the following two dictionaries:
+    The diff is represented as a dictionary where insertions/deletions/substitutions are represented as tuples.
+    For example the following two dictionaries:
 
     ```py
     diff(
       { "a": [ { "b": 1, "c": True }, 1.0, "x" ], "d": 1 },
       { "a": [ { "b": 2, "c": True }, 1.0, "y", True ] }
     )
     ```
 
     will result in the following diff:
 
     ```py
     { "a": [ { "b": (1, 2) }, ("x", "y"), (None, True) ], "d": (1, None) }
     ```
 
-    Here the tuples `(1, 2), ("x", "y"), (None, True), (1, None)` represent the substitions that happened.
-    `None` implies that a object was either removed or added.
+    Here the tuples `(1, 2), ("x", "y"), (None, True), (1, None)` represent the substitutions that happened.
+    `None` implies that an object was either removed or added.
 
     If there is no diff (e.g.: `diff({ "a": 1 }, { "a": 1 })`) the result will be `None`. In this sense,
     this function can also be used to compare two json-compatible dictionaries.
     """
 
     validate(a)
     validate(b)
```

### Comparing `json_dict_diff-1.0.3/.github/workflows/release.yaml` & `json_dict_diff-1.0.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `json_dict_diff-1.0.3/.github/workflows/test.yaml` & `json_dict_diff-1.0.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `json_dict_diff-1.0.3/tests/test.py` & `json_dict_diff-1.0.4/tests/test.py`

 * *Files identical despite different names*

### Comparing `json_dict_diff-1.0.3/LICENCE` & `json_dict_diff-1.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `json_dict_diff-1.0.3/README.md` & `json_dict_diff-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `json_dict_diff-1.0.3/pyproject.toml` & `json_dict_diff-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "json_dict_diff"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Gerrit Proessl", email="gerrit.proessl@gmail.com" },
 ]
 description = "A simple library to create a minimal diff of two json compatible dictionaries"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `json_dict_diff-1.0.3/PKG-INFO` & `json_dict_diff-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: json_dict_diff
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple library to create a minimal diff of two json compatible dictionaries
 Project-URL: Homepage, https://github.com/g3rrit/json_dict_diff
 Project-URL: Issues, https://github.com/g3rrit/json_dict_diff/issues
 Author-email: Gerrit Proessl <gerrit.proessl@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

