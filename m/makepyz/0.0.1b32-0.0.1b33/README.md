# Comparing `tmp/makepyz-0.0.1b32.tar.gz` & `tmp/makepyz-0.0.1b33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makepyz-0.0.1b32.tar", last modified: Mon May 27 02:06:40 2024, max compression
+gzip compressed data, was "makepyz-0.0.1b33.tar", last modified: Mon May 27 02:07:11 2024, max compression
```

## Comparing `makepyz-0.0.1b32.tar` & `makepyz-0.0.1b33.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:06:40.470766 makepyz-0.0.1b32/
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-27 02:06:40.470766 makepyz-0.0.1b32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-27 02:06:38.000000 makepyz-0.0.1b32/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 02:06:40.470766 makepyz-0.0.1b32/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:06:40.466766 makepyz-0.0.1b32/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:06:40.466766 makepyz-0.0.1b32/src/makepyz/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 02:06:38.000000 makepyz-0.0.1b32/src/makepyz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/fileops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/scm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:06:40.470766 makepyz-0.0.1b32/src/makepyz/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/scripts/makepyzui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/tasks_gh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/src/makepyz/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:06:40.470766 makepyz-0.0.1b32/src/makepyz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-27 02:06:40.000000 makepyz-0.0.1b32/src/makepyz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-27 02:06:40.000000 makepyz-0.0.1b32/src/makepyz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 02:06:40.000000 makepyz-0.0.1b32/src/makepyz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-27 02:06:40.000000 makepyz-0.0.1b32/src/makepyz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 02:06:40.000000 makepyz-0.0.1b32/src/makepyz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 02:06:40.000000 makepyz-0.0.1b32/src/makepyz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:06:40.470766 makepyz-0.0.1b32/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/tests/test_fileops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/tests/test_makepyx.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/tests/test_packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-27 02:06:19.000000 makepyz-0.0.1b32/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:07:11.985321 makepyz-0.0.1b33/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-27 02:07:11.985321 makepyz-0.0.1b33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-27 02:07:09.000000 makepyz-0.0.1b33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 02:07:11.985321 makepyz-0.0.1b33/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:07:11.977321 makepyz-0.0.1b33/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:07:11.981321 makepyz-0.0.1b33/src/makepyz/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 02:07:09.000000 makepyz-0.0.1b33/src/makepyz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/scm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:07:11.981321 makepyz-0.0.1b33/src/makepyz/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/scripts/makepyzui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/tasks_gh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/src/makepyz/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:07:11.985321 makepyz-0.0.1b33/src/makepyz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-27 02:07:11.000000 makepyz-0.0.1b33/src/makepyz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-27 02:07:11.000000 makepyz-0.0.1b33/src/makepyz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 02:07:11.000000 makepyz-0.0.1b33/src/makepyz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-27 02:07:11.000000 makepyz-0.0.1b33/src/makepyz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 02:07:11.000000 makepyz-0.0.1b33/src/makepyz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 02:07:11.000000 makepyz-0.0.1b33/src/makepyz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:07:11.985321 makepyz-0.0.1b33/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/tests/test_fileops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/tests/test_makepyx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-27 02:06:50.000000 makepyz-0.0.1b33/tests/test_tree.py
```

### Comparing `makepyz-0.0.1b32/PKG-INFO` & `makepyz-0.0.1b33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makepyz
-Version: 0.0.1b32
+Version: 0.0.1b33
 Summary: a new kind of make tool
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 Project-URL: Issues, https://github.com/cav71/makepyz/issues
 Project-URL: Source, https://github.com/cav71/makepyz
 Keywords: git,scm,version
 Classifier: Development Status :: 4 - Beta
```

### Comparing `makepyz-0.0.1b32/README.md` & `makepyz-0.0.1b33/README.md`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/pyproject.toml` & `makepyz-0.0.1b33/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "makepyz"
-version = "0.0.1b32"
+version = "0.0.1b33"
 description = "a new kind of make tool"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">= 3.8"
 keywords = [
   "git",
   "scm",
```

### Comparing `makepyz-0.0.1b32/src/makepyz/cli.py` & `makepyz-0.0.1b33/src/makepyz/cli.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/src/makepyz/exceptions.py` & `makepyz-0.0.1b33/src/makepyz/exceptions.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/src/makepyz/fileops.py` & `makepyz-0.0.1b33/src/makepyz/fileops.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/src/makepyz/github.py` & `makepyz-0.0.1b33/src/makepyz/github.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/src/makepyz/misc.py` & `makepyz-0.0.1b33/src/makepyz/misc.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/src/makepyz/packaging.py` & `makepyz-0.0.1b33/src/makepyz/packaging.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/src/makepyz/scm.py` & `makepyz-0.0.1b33/src/makepyz/scm.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/src/makepyz/scripts/makepyzui.py` & `makepyz-0.0.1b33/src/makepyz/scripts/makepyzui.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/src/makepyz/tasks.py` & `makepyz-0.0.1b33/src/makepyz/tasks.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/src/makepyz/tasks_gh.py` & `makepyz-0.0.1b33/src/makepyz/tasks_gh.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/src/makepyz/text.py` & `makepyz-0.0.1b33/src/makepyz/text.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/src/makepyz/tree.py` & `makepyz-0.0.1b33/src/makepyz/tree.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/src/makepyz.egg-info/PKG-INFO` & `makepyz-0.0.1b33/src/makepyz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makepyz
-Version: 0.0.1b32
+Version: 0.0.1b33
 Summary: a new kind of make tool
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 Project-URL: Issues, https://github.com/cav71/makepyz/issues
 Project-URL: Source, https://github.com/cav71/makepyz
 Keywords: git,scm,version
 Classifier: Development Status :: 4 - Beta
```

### Comparing `makepyz-0.0.1b32/src/makepyz.egg-info/SOURCES.txt` & `makepyz-0.0.1b33/src/makepyz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/tests/test_cli.py` & `makepyz-0.0.1b33/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/tests/test_fileops.py` & `makepyz-0.0.1b33/tests/test_fileops.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/tests/test_github.py` & `makepyz-0.0.1b33/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/tests/test_packaging.py` & `makepyz-0.0.1b33/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/tests/test_scm.py` & `makepyz-0.0.1b33/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/tests/test_text.py` & `makepyz-0.0.1b33/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b32/tests/test_tree.py` & `makepyz-0.0.1b33/tests/test_tree.py`

 * *Files identical despite different names*

