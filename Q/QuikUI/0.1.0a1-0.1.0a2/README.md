# Comparing `tmp/QuikUI-0.1.0a1.tar.gz` & `tmp/QuikUI-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuikUI-0.1.0a1.tar", last modified: Fri May 17 19:36:28 2024, max compression
+gzip compressed data, was "QuikUI-0.1.0a2.tar", last modified: Mon May 27 16:14:00 2024, max compression
```

## Comparing `QuikUI-0.1.0a1.tar` & `QuikUI-0.1.0a2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:36:28.245252 QuikUI-0.1.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:36:28.241252 QuikUI-0.1.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:36:28.241252 QuikUI-0.1.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-17 19:36:28.245252 QuikUI-0.1.0a1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:36:28.241252 QuikUI-0.1.0a1/QuikUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-17 19:36:28.000000 QuikUI-0.1.0a1/QuikUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-17 19:36:28.000000 QuikUI-0.1.0a1/QuikUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:36:28.000000 QuikUI-0.1.0a1/QuikUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-17 19:36:28.000000 QuikUI-0.1.0a1/QuikUI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 19:36:28.000000 QuikUI-0.1.0a1/QuikUI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:36:28.245252 QuikUI-0.1.0a1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:36:28.245252 QuikUI-0.1.0a1/quikui/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:36:28.245252 QuikUI-0.1.0a1/quikui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/Anchor.html
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/AppBase.html
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/Button.html
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/CheckboxInput.html
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/Div.html
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/Form.html
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/FormInput.html
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/Heading.html
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/Image.html
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/List.html
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/Page.html
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/Paragraph.html
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/RadioInput.html
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/SelectionInput.html
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/templates/Span.html
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/quikui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:36:28.245252 QuikUI-0.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:36:15.000000 QuikUI-0.1.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.830855 QuikUI-0.1.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.822855 QuikUI-0.1.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.822855 QuikUI-0.1.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-27 16:14:00.826855 QuikUI-0.1.0a2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.826855 QuikUI-0.1.0a2/QuikUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-27 16:14:00.000000 QuikUI-0.1.0a2/QuikUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-27 16:14:00.000000 QuikUI-0.1.0a2/QuikUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:14:00.000000 QuikUI-0.1.0a2/QuikUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-27 16:14:00.000000 QuikUI-0.1.0a2/QuikUI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 16:14:00.000000 QuikUI-0.1.0a2/QuikUI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.826855 QuikUI-0.1.0a2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.826855 QuikUI-0.1.0a2/quikui/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.826855 QuikUI-0.1.0a2/quikui/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Anchor.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/AppBase.html
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/CheckboxInput.html
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Div.html
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/FormInput.html
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Image.html
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/List.html
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/RadioInput.html
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/SelectionInput.html
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Span.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:14:00.830855 QuikUI-0.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/setup.py
```

### Comparing `QuikUI-0.1.0a1/.github/workflows/publish.yaml` & `QuikUI-0.1.0a2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `QuikUI-0.1.0a1/LICENSE` & `QuikUI-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `QuikUI-0.1.0a1/PKG-INFO` & `QuikUI-0.1.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuikUI
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Build UIs quickly with Jinga2, FastAPI, Pydantic, htmx, and a little bit of magic
 Author-email: "ApeWorX LTD." <admin@apeworx.io>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `QuikUI-0.1.0a1/QuikUI.egg-info/PKG-INFO` & `QuikUI-0.1.0a2/QuikUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuikUI
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Build UIs quickly with Jinga2, FastAPI, Pydantic, htmx, and a little bit of magic
 Author-email: "ApeWorX LTD." <admin@apeworx.io>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `QuikUI-0.1.0a1/QuikUI.egg-info/SOURCES.txt` & `QuikUI-0.1.0a2/QuikUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QuikUI-0.1.0a1/examples/basic.py` & `QuikUI-0.1.0a2/examples/basic.py`

 * *Files identical despite different names*

### Comparing `QuikUI-0.1.0a1/pyproject.toml` & `QuikUI-0.1.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-  "fastapi[all]>=0.110,<1",
+  "fastapi[all]>=0.100,<1",
   "Jinja2>=3.0,<4",
-  "pydantic>=2.6,<3",
+  "pydantic>=2.1,<3",
 ]
 
 [project.optional-dependencies]
 lint = [
   "black",
 ]
 test = [
```

### Comparing `QuikUI-0.1.0a1/quikui/components.py` & `QuikUI-0.1.0a2/quikui/components.py`

 * *Files identical despite different names*

### Comparing `QuikUI-0.1.0a1/quikui/decorators.py` & `QuikUI-0.1.0a2/quikui/decorators.py`

 * *Files identical despite different names*

### Comparing `QuikUI-0.1.0a1/quikui/dependencies.py` & `QuikUI-0.1.0a2/quikui/dependencies.py`

 * *Files identical despite different names*

### Comparing `QuikUI-0.1.0a1/quikui/templates/AppBase.html` & `QuikUI-0.1.0a2/quikui/templates/AppBase.html`

 * *Files identical despite different names*

### Comparing `QuikUI-0.1.0a1/quikui/utils.py` & `QuikUI-0.1.0a2/quikui/utils.py`

 * *Files identical despite different names*

