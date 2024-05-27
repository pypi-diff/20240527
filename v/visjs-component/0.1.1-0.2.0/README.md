# Comparing `tmp/visjs-component-0.1.1.tar.gz` & `tmp/visjs_component-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visjs-component-0.1.1.tar", last modified: Thu Aug 17 18:12:50 2023, max compression
+gzip compressed data, was "visjs_component-0.2.0.tar", last modified: Mon May 27 16:07:23 2024, max compression
```

## Comparing `visjs-component-0.1.1.tar` & `visjs_component-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 18:12:50.466913 visjs-component-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-17 18:12:39.000000 visjs-component-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-17 18:12:39.000000 visjs-component-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-08-17 18:12:50.466913 visjs-component-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-17 18:12:39.000000 visjs-component-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-17 18:12:50.466913 visjs-component-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-17 18:12:39.000000 visjs-component-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 18:12:50.466913 visjs-component-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 18:12:50.466913 visjs-component-0.1.1/src/visjs_component/
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-08-17 18:12:39.000000 visjs-component-0.1.1/src/visjs_component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 18:12:50.466913 visjs-component-0.1.1/src/visjs_component/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-17 18:12:39.000000 visjs-component-0.1.1/src/visjs_component/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-08-17 18:12:39.000000 visjs-component-0.1.1/src/visjs_component/frontend/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-17 18:12:39.000000 visjs-component-0.1.1/src/visjs_component/frontend/streamlit-component-lib.js
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-17 18:12:39.000000 visjs-component-0.1.1/src/visjs_component/frontend/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 18:12:50.466913 visjs-component-0.1.1/src/visjs_component.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-08-17 18:12:50.000000 visjs-component-0.1.1/src/visjs_component.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-17 18:12:50.000000 visjs-component-0.1.1/src/visjs_component.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-17 18:12:50.000000 visjs-component-0.1.1/src/visjs_component.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-17 18:12:50.000000 visjs-component-0.1.1/src/visjs_component.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-17 18:12:50.000000 visjs-component-0.1.1/src/visjs_component.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:23.510698 visjs_component-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 16:07:19.000000 visjs_component-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 16:07:19.000000 visjs_component-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-27 16:07:23.510698 visjs_component-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-27 16:07:19.000000 visjs_component-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:07:23.510698 visjs_component-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-27 16:07:19.000000 visjs_component-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:23.506698 visjs_component-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:23.510698 visjs_component-0.2.0/src/visjs_component/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-27 16:07:19.000000 visjs_component-0.2.0/src/visjs_component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:23.510698 visjs_component-0.2.0/src/visjs_component/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-27 16:07:19.000000 visjs_component-0.2.0/src/visjs_component/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-27 16:07:19.000000 visjs_component-0.2.0/src/visjs_component/frontend/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-27 16:07:19.000000 visjs_component-0.2.0/src/visjs_component/frontend/streamlit-component-lib.js
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-27 16:07:19.000000 visjs_component-0.2.0/src/visjs_component/frontend/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:23.510698 visjs_component-0.2.0/src/visjs_component.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-27 16:07:23.000000 visjs_component-0.2.0/src/visjs_component.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-27 16:07:23.000000 visjs_component-0.2.0/src/visjs_component.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:07:23.000000 visjs_component-0.2.0/src/visjs_component.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 16:07:23.000000 visjs_component-0.2.0/src/visjs_component.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 16:07:23.000000 visjs_component-0.2.0/src/visjs_component.egg-info/top_level.txt
```

### Comparing `visjs-component-0.1.1/LICENSE` & `visjs_component-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `visjs-component-0.1.1/setup.py` & `visjs_component-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="visjs-component",
-    version="0.1.1",
+    version="0.2.0",
     author="yupikaiei",
     author_email="xtremerhd@gmail.com",
     description="Streamlit component that wraps visjs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `visjs-component-0.1.1/src/visjs_component/frontend/index.html` & `visjs_component-0.2.0/src/visjs_component/frontend/index.html`

 * *Files identical despite different names*

### Comparing `visjs-component-0.1.1/src/visjs_component/frontend/main.js` & `visjs_component-0.2.0/src/visjs_component/frontend/main.js`

 * *Files identical despite different names*

### Comparing `visjs-component-0.1.1/src/visjs_component/frontend/streamlit-component-lib.js` & `visjs_component-0.2.0/src/visjs_component/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

