# Comparing `tmp/makepyz-0.0.1b23.tar.gz` & `tmp/makepyz-0.0.1b25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makepyz-0.0.1b23.tar", last modified: Sat May 25 13:27:04 2024, max compression
+gzip compressed data, was "makepyz-0.0.1b25.tar", last modified: Mon May 27 00:39:25 2024, max compression
```

## Comparing `makepyz-0.0.1b23.tar` & `makepyz-0.0.1b25.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:27:04.101009 makepyz-0.0.1b23/
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-25 13:27:04.101009 makepyz-0.0.1b23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-25 13:27:01.000000 makepyz-0.0.1b23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 13:27:04.101009 makepyz-0.0.1b23/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:27:04.097009 makepyz-0.0.1b23/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:27:04.101009 makepyz-0.0.1b23/src/makepyz/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-25 13:27:01.000000 makepyz-0.0.1b23/src/makepyz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/fileops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/scm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:27:04.101009 makepyz-0.0.1b23/src/makepyz/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/scripts/makepyzui.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/src/makepyz/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:27:04.101009 makepyz-0.0.1b23/src/makepyz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-25 13:27:04.000000 makepyz-0.0.1b23/src/makepyz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-25 13:27:04.000000 makepyz-0.0.1b23/src/makepyz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 13:27:04.000000 makepyz-0.0.1b23/src/makepyz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-25 13:27:04.000000 makepyz-0.0.1b23/src/makepyz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-25 13:27:04.000000 makepyz-0.0.1b23/src/makepyz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 13:27:04.000000 makepyz-0.0.1b23/src/makepyz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:27:04.101009 makepyz-0.0.1b23/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/tests/test_fileops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/tests/test_makepyx.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/tests/test_packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-25 13:26:40.000000 makepyz-0.0.1b23/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:25.029845 makepyz-0.0.1b25/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-27 00:39:25.029845 makepyz-0.0.1b25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-27 00:39:22.000000 makepyz-0.0.1b25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 00:39:25.029845 makepyz-0.0.1b25/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:25.021845 makepyz-0.0.1b25/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:25.025845 makepyz-0.0.1b25/src/makepyz/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 00:39:22.000000 makepyz-0.0.1b25/src/makepyz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/scm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:25.025845 makepyz-0.0.1b25/src/makepyz/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/scripts/makepyzui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/tasks_gh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:25.029845 makepyz-0.0.1b25/src/makepyz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-27 00:39:25.000000 makepyz-0.0.1b25/src/makepyz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-27 00:39:25.000000 makepyz-0.0.1b25/src/makepyz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 00:39:25.000000 makepyz-0.0.1b25/src/makepyz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-27 00:39:25.000000 makepyz-0.0.1b25/src/makepyz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 00:39:25.000000 makepyz-0.0.1b25/src/makepyz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 00:39:25.000000 makepyz-0.0.1b25/src/makepyz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:25.029845 makepyz-0.0.1b25/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_fileops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_makepyx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_tree.py
```

### Comparing `makepyz-0.0.1b23/PKG-INFO` & `makepyz-0.0.1b25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makepyz
-Version: 0.0.1b23
+Version: 0.0.1b25
 Summary: a new kind of make tool
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 Project-URL: Issues, https://github.com/cav71/makepyz/issues
 Project-URL: Source, https://github.com/cav71/makepyz
 Keywords: git,scm,version
 Classifier: Development Status :: 4 - Beta
```

### Comparing `makepyz-0.0.1b23/README.md` & `makepyz-0.0.1b25/README.md`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/pyproject.toml` & `makepyz-0.0.1b25/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "makepyz"
-version = "0.0.1b23"
+version = "0.0.1b25"
 description = "a new kind of make tool"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">= 3.8"
 keywords = [
   "git",
   "scm",
@@ -68,14 +68,15 @@
 ignore_missing_imports = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 warn_no_return = false
 warn_unused_ignores = true
 check_untyped_defs = true
+exclude = []
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.paths]
 source = [
   "src/",
```

### Comparing `makepyz-0.0.1b23/src/makepyz/exceptions.py` & `makepyz-0.0.1b25/src/makepyz/exceptions.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/src/makepyz/fileops.py` & `makepyz-0.0.1b25/src/makepyz/fileops.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/src/makepyz/github.py` & `makepyz-0.0.1b25/src/makepyz/github.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/src/makepyz/misc.py` & `makepyz-0.0.1b25/src/makepyz/misc.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/src/makepyz/packaging.py` & `makepyz-0.0.1b25/src/makepyz/packaging.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/src/makepyz/scm.py` & `makepyz-0.0.1b25/src/makepyz/scm.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/src/makepyz/text.py` & `makepyz-0.0.1b25/src/makepyz/text.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/src/makepyz/tree.py` & `makepyz-0.0.1b25/src/makepyz/tree.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/src/makepyz.egg-info/PKG-INFO` & `makepyz-0.0.1b25/src/makepyz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makepyz
-Version: 0.0.1b23
+Version: 0.0.1b25
 Summary: a new kind of make tool
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 Project-URL: Issues, https://github.com/cav71/makepyz/issues
 Project-URL: Source, https://github.com/cav71/makepyz
 Keywords: git,scm,version
 Classifier: Development Status :: 4 - Beta
```

### Comparing `makepyz-0.0.1b23/src/makepyz.egg-info/SOURCES.txt` & `makepyz-0.0.1b25/src/makepyz.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/makepyz/fileops.py
 src/makepyz/github.py
 src/makepyz/misc.py
 src/makepyz/packaging.py
 src/makepyz/py.typed
 src/makepyz/scm.py
 src/makepyz/tasks.py
+src/makepyz/tasks_gh.py
 src/makepyz/text.py
 src/makepyz/tree.py
 src/makepyz.egg-info/PKG-INFO
 src/makepyz.egg-info/SOURCES.txt
 src/makepyz.egg-info/dependency_links.txt
 src/makepyz.egg-info/entry_points.txt
 src/makepyz.egg-info/requires.txt
```

### Comparing `makepyz-0.0.1b23/tests/test_cli.py` & `makepyz-0.0.1b25/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/tests/test_fileops.py` & `makepyz-0.0.1b25/tests/test_fileops.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/tests/test_github.py` & `makepyz-0.0.1b25/tests/test_github.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     data = json.loads(path.read_text())
 
     assert github.get_gdata(json.dumps(data)) == {
         "ref_name": "main",
         "ref_type": "branch",
         "run_number": "5",
         "sha": "18cc30248e1023c50f26b0d5c38c11e71e5af99a",
-        "workflow_ref": "LuxorLabs/luxos-tooling/.github/workflows/"
+        "workflow_ref": "cav71/makepyz/.github/workflows/"
         "push-main.yml@refs/heads/main",
     }
 
     assert github.get_gdata(f"@{path}") == {
         "ref_name": "main",
         "ref_type": "branch",
         "run_number": "5",
         "sha": "18cc30248e1023c50f26b0d5c38c11e71e5af99a",
-        "workflow_ref": "LuxorLabs/luxos-tooling/.github/workflows/"
+        "workflow_ref": "cav71/makepyz/.github/workflows/"
         "push-main.yml@refs/heads/main",
     }
```

### Comparing `makepyz-0.0.1b23/tests/test_packaging.py` & `makepyz-0.0.1b25/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/tests/test_scm.py` & `makepyz-0.0.1b25/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/tests/test_text.py` & `makepyz-0.0.1b25/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b23/tests/test_tree.py` & `makepyz-0.0.1b25/tests/test_tree.py`

 * *Files identical despite different names*

