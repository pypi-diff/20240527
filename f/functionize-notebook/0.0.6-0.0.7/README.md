# Comparing `tmp/functionize_notebook-0.0.6.tar.gz` & `tmp/functionize_notebook-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functionize_notebook-0.0.6.tar", last modified: Sat May 25 07:17:35 2024, max compression
+gzip compressed data, was "functionize_notebook-0.0.7.tar", last modified: Mon May 27 04:40:46 2024, max compression
```

## Comparing `functionize_notebook-0.0.6.tar` & `functionize_notebook-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:17:35.960535 functionize_notebook-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-25 07:17:32.000000 functionize_notebook-0.0.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-25 07:17:32.000000 functionize_notebook-0.0.6/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-25 07:17:32.000000 functionize_notebook-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 07:17:32.000000 functionize_notebook-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-25 07:17:35.960535 functionize_notebook-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-25 07:17:32.000000 functionize_notebook-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:17:35.960535 functionize_notebook-0.0.6/functionize_notebook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-25 07:17:35.000000 functionize_notebook-0.0.6/functionize_notebook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-25 07:17:35.000000 functionize_notebook-0.0.6/functionize_notebook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 07:17:35.000000 functionize_notebook-0.0.6/functionize_notebook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-25 07:17:35.000000 functionize_notebook-0.0.6/functionize_notebook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-25 07:17:35.000000 functionize_notebook-0.0.6/functionize_notebook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:17:35.960535 functionize_notebook-0.0.6/notebook_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-25 07:17:32.000000 functionize_notebook-0.0.6/notebook_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 07:17:35.960535 functionize_notebook-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-25 07:17:32.000000 functionize_notebook-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:40:46.095242 functionize_notebook-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-27 04:40:46.095242 functionize_notebook-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:40:46.095242 functionize_notebook-0.0.7/functionize_notebook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-27 04:40:46.000000 functionize_notebook-0.0.7/functionize_notebook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-27 04:40:46.000000 functionize_notebook-0.0.7/functionize_notebook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:40:46.000000 functionize_notebook-0.0.7/functionize_notebook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 04:40:46.000000 functionize_notebook-0.0.7/functionize_notebook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 04:40:46.000000 functionize_notebook-0.0.7/functionize_notebook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:40:46.095242 functionize_notebook-0.0.7/notebook_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/notebook_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 04:40:46.095242 functionize_notebook-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/setup.py
```

### Comparing `functionize_notebook-0.0.6/LICENSE.txt` & `functionize_notebook-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `functionize_notebook-0.0.6/PKG-INFO` & `functionize_notebook-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functionize-notebook
-Version: 0.0.6
+Version: 0.0.7
 Summary: run notebook like a function
 Home-page: https://github.com/BuiHoangTu/functionize-notebook/tree/release
 Author: Bui Hoang Tu
 Author-email: bhtu.work@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `functionize_notebook-0.0.6/README.md` & `functionize_notebook-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `functionize_notebook-0.0.6/functionize_notebook.egg-info/PKG-INFO` & `functionize_notebook-0.0.7/functionize_notebook.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functionize-notebook
-Version: 0.0.6
+Version: 0.0.7
 Summary: run notebook like a function
 Home-page: https://github.com/BuiHoangTu/functionize-notebook/tree/release
 Author: Bui Hoang Tu
 Author-email: bhtu.work@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `functionize_notebook-0.0.6/notebook_wrapper/__init__.py` & `functionize_notebook-0.0.7/notebook_wrapper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,29 @@
 class NotebookWrapper:
     def __init__(
         self,
         notebookFile: str | Path,
         inputVariable: str | List[str] | None,
         outputVariable: str | List[str] | None,
         inputTag: str = "input",
+        allowError: bool = False,
     ):
         self.notebook = Path(notebookFile)
 
         if inputVariable is None:
             inputVariable = []
         elif isinstance(inputVariable, str):
             inputVariable = [inputVariable]
         self.inputVariable = inputVariable
 
         self.outputVariable = outputVariable
 
         self.inputTag = inputTag
+        
+        self.allowError = allowError
 
         pass
 
     def __call__(self, *args, **kwargs):
         return self.run(*args, *kwargs)
 
     def run(self, *args, **kwargs) -> Any | List[Any]:
@@ -84,15 +87,15 @@
                 datetime.now().__str__() + ".pkl",
             )
             outputPath.parent.mkdir(parents=True, exist_ok=True)
 
             outputIndex = self._insertOutputCell(nb, outputPath)
             pass
 
-        ep = ExecutePreprocessor(timeout=None)
+        ep = ExecutePreprocessor(timeout=None, allow_errors=self.allowError)
         resultNb, _ = ep.preprocess(nb, {"metadata": {"path": self.notebook.parent}})
 
         if _outputNotebook is not None:
             if inputIndex >= 0:
                 resultNb.cells.pop(inputIndex)
 
                 # Add markdown cell noting injected variables
```

### Comparing `functionize_notebook-0.0.6/setup.py` & `functionize_notebook-0.0.7/setup.py`

 * *Files identical despite different names*

