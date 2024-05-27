# Comparing `tmp/opengeodeweb_back-4.1.1.tar.gz` & `tmp/opengeodeweb_back-4.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengeodeweb_back-4.1.1.tar", last modified: Fri May  3 09:48:04 2024, max compression
+gzip compressed data, was "opengeodeweb_back-4.2.0rc1.tar", last modified: Mon May 27 10:11:09 2024, max compression
```

## Comparing `opengeodeweb_back-4.1.1.tar` & `opengeodeweb_back-4.2.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:04.263737 opengeodeweb_back-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-03 09:48:04.263737 opengeodeweb_back-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-03 09:47:56.000000 opengeodeweb_back-4.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:48:04.263737 opengeodeweb_back-4.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:04.259737 opengeodeweb_back-4.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:04.263737 opengeodeweb_back-4.1.1/src/OpenGeodeWeb_Back.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-03 09:48:04.000000 opengeodeweb_back-4.1.1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-03 09:48:04.000000 opengeodeweb_back-4.1.1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:48:04.000000 opengeodeweb_back-4.1.1/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-03 09:48:04.000000 opengeodeweb_back-4.1.1/src/OpenGeodeWeb_Back.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 09:48:04.000000 opengeodeweb_back-4.1.1/src/OpenGeodeWeb_Back.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:04.259737 opengeodeweb_back-4.1.1/src/opengeodeweb_back/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/src/opengeodeweb_back/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/src/opengeodeweb_back/geode_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20286 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/src/opengeodeweb_back/geode_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:04.263737 opengeodeweb_back-4.1.1/src/opengeodeweb_back/routes/
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/src/opengeodeweb_back/routes/blueprint_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:04.263737 opengeodeweb_back-4.1.1/src/opengeodeweb_back/routes/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/src/opengeodeweb_back/routes/schemas/allowed_files.json
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/src/opengeodeweb_back/routes/schemas/allowed_objects.json
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/src/opengeodeweb_back/routes/schemas/geode_objects_and_output_extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/src/opengeodeweb_back/routes/schemas/geographic_coordinate_systems.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/src/opengeodeweb_back/routes/schemas/inspect_file.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/src/opengeodeweb_back/routes/schemas/missing_files.json
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-03 09:47:49.000000 opengeodeweb_back-4.1.1/src/opengeodeweb_back/routes/schemas/upload_file.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:04.263737 opengeodeweb_back-4.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-05-03 09:47:50.000000 opengeodeweb_back-4.1.1/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-03 09:47:50.000000 opengeodeweb_back-4.1.1/tests/test_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-27 10:11:00.000000 opengeodeweb_back-4.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.549610 opengeodeweb_back-4.2.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-27 10:11:09.000000 opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 10:11:09.000000 opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:11:09.000000 opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-27 10:11:09.000000 opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 10:11:09.000000 opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/geode_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20286 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/geode_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/blueprint_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/allowed_files.json
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/allowed_objects.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/geode_objects_and_output_extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/geographic_coordinate_systems.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/inspect_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/missing_files.json
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/upload_file.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/tests/test_routes.py
```

### Comparing `opengeodeweb_back-4.1.1/LICENSE` & `opengeodeweb_back-4.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.1/PKG-INFO` & `opengeodeweb_back-4.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 4.1.1
+Version: 4.2.0rc1
 Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <team-web@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,15 @@
 Requires-Dist: opengeode-core==14.19.2
 Requires-Dist: opengeode-geosciences==7.6.4
 Requires-Dist: opengeode-geosciencesio==4.7.6
 Requires-Dist: opengeode-inspector==5.1.3
 Requires-Dist: opengeode-io==6.5.1
 Requires-Dist: referencing==0.35.0
 Requires-Dist: rpds-py==0.18.0
+Requires-Dist: typing-extensions==4.12.0
 Requires-Dist: werkzeug==3.0.2
 
 <h1 align="center">OpenGeodeWeb-Back<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenSource Python framework based on OpenGeode</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CI/badge.svg" alt="Build Status">
```

### Comparing `opengeodeweb_back-4.1.1/README.md` & `opengeodeweb_back-4.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.1/pyproject.toml` & `opengeodeweb_back-4.2.0rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OpenGeodeWeb-Back"
-version = "4.1.1"
+version = "4.2.0-rc.1"
 dynamic = ["dependencies"]
 authors = [
   { name="Geode-solutions", email="team-web@geode-solutions.com" },
 ]
 description = "OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `opengeodeweb_back-4.1.1/requirements.txt` & `opengeodeweb_back-4.2.0rc1/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile requirements.in
 #
 asgiref==3.8.1
     # via flask
 attrs==23.2.0
@@ -106,11 +106,13 @@
     # via
     #   jsonschema
     #   jsonschema-specifications
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
+typing-extensions==4.12.0
+    # via asgiref
 werkzeug==3.0.2
     # via
     #   -r requirements.in
     #   flask
```

### Comparing `opengeodeweb_back-4.1.1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO` & `opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 4.1.1
+Version: 4.2.0rc1
 Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <team-web@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,15 @@
 Requires-Dist: opengeode-core==14.19.2
 Requires-Dist: opengeode-geosciences==7.6.4
 Requires-Dist: opengeode-geosciencesio==4.7.6
 Requires-Dist: opengeode-inspector==5.1.3
 Requires-Dist: opengeode-io==6.5.1
 Requires-Dist: referencing==0.35.0
 Requires-Dist: rpds-py==0.18.0
+Requires-Dist: typing-extensions==4.12.0
 Requires-Dist: werkzeug==3.0.2
 
 <h1 align="center">OpenGeodeWeb-Back<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenSource Python framework based on OpenGeode</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CI/badge.svg" alt="Build Status">
```

### Comparing `opengeodeweb_back-4.1.1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt` & `opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.1/src/OpenGeodeWeb_Back.egg-info/requires.txt` & `opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 opengeode-core==14.19.2
 opengeode-geosciences==7.6.4
 opengeode-geosciencesio==4.7.6
 opengeode-inspector==5.1.3
 opengeode-io==6.5.1
 referencing==0.35.0
 rpds-py==0.18.0
+typing-extensions==4.12.0
 werkzeug==3.0.2
```

### Comparing `opengeodeweb_back-4.1.1/src/opengeodeweb_back/geode_functions.py` & `opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/geode_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,7 +350,20 @@
         as_attachment=True,
         mimetype=mimetype,
     )
     response.headers["new-file-name"] = new_file_name
     response.headers["Access-Control-Expose-Headers"] = "new-file-name"
 
     return response
+
+
+def handle_exception(e):
+    response = e.get_response()
+    response.data = flask.json.dumps(
+        {
+            "code": e.code,
+            "name": e.name,
+            "description": e.description,
+        }
+    )
+    response.content_type = "application/json"
+    return response
```

### Comparing `opengeodeweb_back-4.1.1/src/opengeodeweb_back/geode_objects.py` & `opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/geode_objects.py`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.1/src/opengeodeweb_back/routes/blueprint_routes.py` & `opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/blueprint_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     methods=allowed_files_json["methods"],
 )
 def allowed_files():
     geode_functions.validate_request(flask.request, allowed_files_json)
     extensions = geode_functions.list_input_extensions(
         flask.request.json["supported_feature"]
     )
-    return {"status": 200, "extensions": extensions}
+    return flask.make_response({"extensions": extensions}, 200)
 
 
 with open(
     os.path.join(schemas, "upload_file.json"),
     "r",
 ) as file:
     upload_file_json = json.load(file)
```

### Comparing `opengeodeweb_back-4.1.1/tests/test_functions.py` & `opengeodeweb_back-4.2.0rc1/tests/test_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -325,7 +325,18 @@
         assert type(version) is dict
 
 
 def test_extension_from_filename():
     extension = geode_functions.extension_from_filename("test.toto")
     assert type(extension) is str
     assert extension.count(".") == 0
+
+
+def test_handle_exception(client):
+    route = "/error"
+    response = client.post(route)
+    assert response.status_code == 500
+    data = response.get_json()
+    assert type(data) is dict
+    assert type(data["description"]) is str
+    assert type(data["name"]) is str
+    assert type(data["code"]) is int
```

### Comparing `opengeodeweb_back-4.1.1/tests/test_routes.py` & `opengeodeweb_back-4.2.0rc1/tests/test_routes.py`

 * *Files identical despite different names*

