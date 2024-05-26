# Comparing `tmp/streamlit_p5-0.0.1.tar.gz` & `tmp/streamlit_p5-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_p5-0.0.1.tar", last modified: Sat May 25 08:39:51 2024, max compression
+gzip compressed data, was "streamlit_p5-0.0.2.tar", last modified: Sun May 26 22:17:50 2024, max compression
```

## Comparing `streamlit_p5-0.0.1.tar` & `streamlit_p5-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-25 08:39:51.521729 streamlit_p5-0.0.1/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       35 2024-05-25 08:26:39.000000 streamlit_p5-0.0.1/MANIFEST.in
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1130 2024-05-25 08:39:51.521729 streamlit_p5-0.0.1/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      512 2024-05-25 08:26:39.000000 streamlit_p5-0.0.1/README.md
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-05-25 08:39:51.521729 streamlit_p5-0.0.1/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1048 2024-05-25 08:39:32.000000 streamlit_p5-0.0.1/setup.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-25 08:39:51.517729 streamlit_p5-0.0.1/streamlit_p5/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1297 2024-05-25 08:26:39.000000 streamlit_p5-0.0.1/streamlit_p5/__init__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-25 08:39:51.517729 streamlit_p5-0.0.1/streamlit_p5/p5/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2045 2024-05-25 07:01:19.000000 streamlit_p5-0.0.1/streamlit_p5/p5/index.html
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)  1034532 2024-05-24 21:32:33.000000 streamlit_p5-0.0.1/streamlit_p5/p5/p5.min.js
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-25 08:39:51.517729 streamlit_p5-0.0.1/streamlit_p5.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1130 2024-05-25 08:39:51.000000 streamlit_p5-0.0.1/streamlit_p5.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      287 2024-05-25 08:39:51.000000 streamlit_p5-0.0.1/streamlit_p5.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-25 08:39:51.000000 streamlit_p5-0.0.1/streamlit_p5.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      140 2024-05-25 08:39:51.000000 streamlit_p5-0.0.1/streamlit_p5.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       13 2024-05-25 08:39:51.000000 streamlit_p5-0.0.1/streamlit_p5.egg-info/top_level.txt
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-26 22:17:50.512182 streamlit_p5-0.0.2/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       35 2024-05-25 08:26:39.000000 streamlit_p5-0.0.2/MANIFEST.in
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1527 2024-05-26 22:17:50.512182 streamlit_p5-0.0.2/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      909 2024-05-25 18:54:26.000000 streamlit_p5-0.0.2/README.md
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-05-26 22:17:50.512182 streamlit_p5-0.0.2/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      897 2024-05-26 22:17:39.000000 streamlit_p5-0.0.2/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-26 22:17:50.508182 streamlit_p5-0.0.2/streamlit_p5/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1297 2024-05-25 08:26:39.000000 streamlit_p5-0.0.2/streamlit_p5/__init__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-26 22:17:50.508182 streamlit_p5-0.0.2/streamlit_p5/p5/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2045 2024-05-25 07:01:19.000000 streamlit_p5-0.0.2/streamlit_p5/p5/index.html
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)  1034532 2024-05-24 21:32:33.000000 streamlit_p5-0.0.2/streamlit_p5/p5/p5.min.js
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-26 22:17:50.508182 streamlit_p5-0.0.2/streamlit_p5.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1527 2024-05-26 22:17:50.000000 streamlit_p5-0.0.2/streamlit_p5.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      287 2024-05-26 22:17:50.000000 streamlit_p5-0.0.2/streamlit_p5.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-26 22:17:50.000000 streamlit_p5-0.0.2/streamlit_p5.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      140 2024-05-26 22:17:50.000000 streamlit_p5-0.0.2/streamlit_p5.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       13 2024-05-26 22:17:50.000000 streamlit_p5-0.0.2/streamlit_p5.egg-info/top_level.txt
```

### Comparing `streamlit_p5-0.0.1/PKG-INFO` & `streamlit_p5-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_p5
-Version: 0.0.1
+Version: 0.0.2
 Summary: Embed the power of Processing.org in your Streamlit app
 Home-page: 
 Author: Neal Riley
 Author-email: neal.riley@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
@@ -19,19 +19,33 @@
 # streamlit_sp5
 
 Embed your processing sketches in Streamlit!
 
 ## Installation instructions
 
 ```sh
-pip install streamlit_p5
+pip install streamlit streamlit_p5
+```
+
+## Quickstart
+
+```python
+streamlit run example.py
 ```
 
 ## Usage instructions
 
+The `sketch` object takes a few arguments: 
+
+- sketch : a string representing your P5js sketch
+- width : width of the element in Streamlit
+- height : height of the element in Streamlit (make sure to match these with your sketch!)
+
+### Example:
+
 ```python
 import streamlit as st
 from streamlit_p5 import sketch
 
 p5_sketch = sketch("""
 function setup() {
    createCanvas(700, 500);
@@ -40,7 +54,13 @@
 // The background function is a statement that tells the computer
 // which color (or gray value) to make the background of the display window 
 function draw() {
    background(204, 153, 0);
 }
 """, width=700, height=500)
 ```
+
+Wanna build this from source? just run: 
+
+```sh
+python setup.py sdist bdist_wheel
+```
```

### Comparing `streamlit_p5-0.0.1/setup.py` & `streamlit_p5-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,26 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit_p5",
-    version="0.0.1",
+    version="0.0.2",
     author="Neal Riley",
     author_email="neal.riley@gmail.com",
     description="Embed the power of Processing.org in your Streamlit app",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[],
     python_requires=">=3.7",
     install_requires=[
-        # By definition, a Custom Component depends on Streamlit.
-        # If your component has other Python dependencies, list
-        # them here.
         "streamlit >= 0.63",
     ],
     extras_require={
         "devel": [
             "wheel",
             "pytest==7.4.0",
             "playwright==1.39.0",
```

### Comparing `streamlit_p5-0.0.1/streamlit_p5/__init__.py` & `streamlit_p5-0.0.2/streamlit_p5/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_p5-0.0.1/streamlit_p5/p5/index.html` & `streamlit_p5-0.0.2/streamlit_p5/p5/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_p5-0.0.1/streamlit_p5/p5/p5.min.js` & `streamlit_p5-0.0.2/streamlit_p5/p5/p5.min.js`

 * *Files identical despite different names*

### Comparing `streamlit_p5-0.0.1/streamlit_p5.egg-info/PKG-INFO` & `streamlit_p5-0.0.2/streamlit_p5.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_p5
-Version: 0.0.1
+Version: 0.0.2
 Summary: Embed the power of Processing.org in your Streamlit app
 Home-page: 
 Author: Neal Riley
 Author-email: neal.riley@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
@@ -19,19 +19,33 @@
 # streamlit_sp5
 
 Embed your processing sketches in Streamlit!
 
 ## Installation instructions
 
 ```sh
-pip install streamlit_p5
+pip install streamlit streamlit_p5
+```
+
+## Quickstart
+
+```python
+streamlit run example.py
 ```
 
 ## Usage instructions
 
+The `sketch` object takes a few arguments: 
+
+- sketch : a string representing your P5js sketch
+- width : width of the element in Streamlit
+- height : height of the element in Streamlit (make sure to match these with your sketch!)
+
+### Example:
+
 ```python
 import streamlit as st
 from streamlit_p5 import sketch
 
 p5_sketch = sketch("""
 function setup() {
    createCanvas(700, 500);
@@ -40,7 +54,13 @@
 // The background function is a statement that tells the computer
 // which color (or gray value) to make the background of the display window 
 function draw() {
    background(204, 153, 0);
 }
 """, width=700, height=500)
 ```
+
+Wanna build this from source? just run: 
+
+```sh
+python setup.py sdist bdist_wheel
+```
```

