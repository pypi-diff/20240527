# Comparing `tmp/connexion-3.0.6.tar.gz` & `tmp/connexion-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connexion-3.0.6.tar", max compression
+gzip compressed data, was "connexion-3.1.0.tar", max compression
```

## Comparing `connexion-3.0.6.tar` & `connexion-3.1.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0    11357 2024-02-14 08:35:02.991030 connexion-3.0.6/LICENSE
--rw-r--r--   0        0        0    10411 2024-02-14 08:35:02.991030 connexion-3.0.6/README.md
--rwxr-xr-x   0        0        0     1351 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/__init__.py
--rw-r--r--   0        0        0      144 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/__main__.py
--rw-r--r--   0        0        0      250 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/apps/__init__.py
--rw-r--r--   0        0        0    13300 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/apps/abstract.py
--rw-r--r--   0        0        0     8318 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/apps/asynchronous.py
--rw-r--r--   0        0        0    11292 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/apps/flask.py
--rw-r--r--   0        0        0     4662 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/cli.py
--rw-r--r--   0        0        0      991 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/context.py
--rw-r--r--   0        0        0     1081 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/datastructures.py
--rw-r--r--   0        0        0      210 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/decorators/__init__.py
--rw-r--r--   0        0        0     6868 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/decorators/main.py
--rw-r--r--   0        0        0    15414 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/decorators/parameter.py
--rw-r--r--   0        0        0     7980 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/decorators/response.py
--rw-r--r--   0        0        0     7877 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/frameworks/__init__.py
--rw-r--r--   0        0        0     1069 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/frameworks/abstract.py
--rw-r--r--   0        0        0     4096 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/frameworks/flask.py
--rw-r--r--   0        0        0     2810 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/frameworks/starlette.py
--rw-r--r--   0        0        0     1259 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/handlers.py
--rw-r--r--   0        0        0     2264 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/http_facts.py
--rw-r--r--   0        0        0     4661 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/json_schema.py
--rw-r--r--   0        0        0     2856 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/jsonifier.py
--rw-r--r--   0        0        0     8572 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/lifecycle.py
--rw-r--r--   0        0        0      111 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/middleware/__init__.py
--rw-r--r--   0        0        0     9749 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/middleware/abstract.py
--rw-r--r--   0        0        0     1407 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/middleware/context.py
--rw-r--r--   0        0        0     3663 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/middleware/exceptions.py
--rw-r--r--   0        0        0      940 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/middleware/lifespan.py
--rw-r--r--   0        0        0    22157 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/middleware/main.py
--rw-r--r--   0        0        0     6653 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/middleware/request_validation.py
--rw-r--r--   0        0        0     5660 2024-02-14 08:35:02.991030 connexion-3.0.6/connexion/middleware/response_validation.py
--rw-r--r--   0        0        0     5413 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/middleware/routing.py
--rw-r--r--   0        0        0     5860 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/middleware/security.py
--rw-r--r--   0        0        0     1250 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/middleware/server_error.py
--rw-r--r--   0        0        0     8183 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/middleware/swagger_ui.py
--rw-r--r--   0        0        0     1828 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/mock.py
--rw-r--r--   0        0        0      531 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/operations/__init__.py
--rw-r--r--   0        0        0     6962 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/operations/abstract.py
--rw-r--r--   0        0        0     8983 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/operations/openapi.py
--rw-r--r--   0        0        0    11327 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/operations/swagger2.py
--rw-r--r--   0        0        0     3760 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/options.py
--rw-r--r--   0        0        0     2255 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/problem.py
--rw-r--r--   0        0        0    12315 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/resolver.py
--rw-r--r--   0        0        0    40020 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/resources/schemas/v2.0/schema.json
--rw-r--r--   0        0        0    35456 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/resources/schemas/v3.0/schema.json
--rw-r--r--   0        0        0    21674 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/security.py
--rw-r--r--   0        0        0     9799 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/spec.py
--rw-r--r--   0        0        0     2153 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/testing.py
--rw-r--r--   0        0        0      888 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/types.py
--rw-r--r--   0        0        0    11661 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/uri_parsing.py
--rw-r--r--   0        0        0    15481 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/utils.py
--rw-r--r--   0        0        0      892 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/validators/__init__.py
--rw-r--r--   0        0        0     7130 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/validators/abstract.py
--rw-r--r--   0        0        0     4583 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/validators/form_data.py
--rw-r--r--   0        0        0     4884 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/validators/json.py
--rw-r--r--   0        0        0     5181 2024-02-14 08:35:02.995030 connexion-3.0.6/connexion/validators/parameter.py
--rw-r--r--   0        0        0     3052 2024-02-14 08:35:03.195033 connexion-3.0.6/pyproject.toml
--rw-r--r--   0        0        0    12521 1970-01-01 00:00:00.000000 connexion-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-27 11:44:58.328977 connexion-3.1.0/LICENSE
+-rw-r--r--   0        0        0      102 2024-05-27 11:44:58.328977 connexion-3.1.0/NOTICE
+-rw-r--r--   0        0        0    10411 2024-05-27 11:44:58.328977 connexion-3.1.0/README.md
+-rwxr-xr-x   0        0        0     1351 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/__init__.py
+-rw-r--r--   0        0        0      144 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/__main__.py
+-rw-r--r--   0        0        0      250 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/apps/__init__.py
+-rw-r--r--   0        0        0    13306 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/apps/abstract.py
+-rw-r--r--   0        0        0     8318 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/apps/asynchronous.py
+-rw-r--r--   0        0        0    11292 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/apps/flask.py
+-rw-r--r--   0        0        0     4813 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/cli.py
+-rw-r--r--   0        0        0      991 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/context.py
+-rw-r--r--   0        0        0     1081 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/datastructures.py
+-rw-r--r--   0        0        0      210 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/decorators/__init__.py
+-rw-r--r--   0        0        0     6868 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/decorators/main.py
+-rw-r--r--   0        0        0    15414 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/decorators/parameter.py
+-rw-r--r--   0        0        0     7980 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/decorators/response.py
+-rw-r--r--   0        0        0     7877 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/frameworks/__init__.py
+-rw-r--r--   0        0        0     1069 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/frameworks/abstract.py
+-rw-r--r--   0        0        0     4096 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/frameworks/flask.py
+-rw-r--r--   0        0        0     2810 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/frameworks/starlette.py
+-rw-r--r--   0        0        0     1259 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/handlers.py
+-rw-r--r--   0        0        0     2264 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/http_facts.py
+-rw-r--r--   0        0        0     4661 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/json_schema.py
+-rw-r--r--   0        0        0     2856 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/jsonifier.py
+-rw-r--r--   0        0        0     8572 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/lifecycle.py
+-rw-r--r--   0        0        0      111 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/middleware/__init__.py
+-rw-r--r--   0        0        0     9749 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/middleware/abstract.py
+-rw-r--r--   0        0        0     1407 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/middleware/context.py
+-rw-r--r--   0        0        0     3890 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/middleware/exceptions.py
+-rw-r--r--   0        0        0      940 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/middleware/lifespan.py
+-rw-r--r--   0        0        0    22329 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/middleware/main.py
+-rw-r--r--   0        0        0     6653 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/middleware/request_validation.py
+-rw-r--r--   0        0        0     5660 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/middleware/response_validation.py
+-rw-r--r--   0        0        0     5413 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/middleware/routing.py
+-rw-r--r--   0        0        0     5860 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/middleware/security.py
+-rw-r--r--   0        0        0     1250 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/middleware/server_error.py
+-rw-r--r--   0        0        0     8183 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/middleware/swagger_ui.py
+-rw-r--r--   0        0        0     2033 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/mock.py
+-rw-r--r--   0        0        0      531 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/operations/__init__.py
+-rw-r--r--   0        0        0     6962 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/operations/abstract.py
+-rw-r--r--   0        0        0     8498 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/operations/openapi.py
+-rw-r--r--   0        0        0    10842 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/operations/swagger2.py
+-rw-r--r--   0        0        0     3760 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/options.py
+-rw-r--r--   0        0        0     2255 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/problem.py
+-rw-r--r--   0        0        0    12315 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/resolver.py
+-rw-r--r--   0        0        0    40020 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/resources/schemas/v2.0/schema.json
+-rw-r--r--   0        0        0    35456 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/resources/schemas/v3.0/schema.json
+-rw-r--r--   0        0        0    21811 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/security.py
+-rw-r--r--   0        0        0    10212 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/spec.py
+-rw-r--r--   0        0        0     2153 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/testing.py
+-rw-r--r--   0        0        0      888 2024-05-27 11:44:58.328977 connexion-3.1.0/connexion/types.py
+-rw-r--r--   0        0        0    11661 2024-05-27 11:44:58.332977 connexion-3.1.0/connexion/uri_parsing.py
+-rw-r--r--   0        0        0    16357 2024-05-27 11:44:58.332977 connexion-3.1.0/connexion/utils.py
+-rw-r--r--   0        0        0      892 2024-05-27 11:44:58.332977 connexion-3.1.0/connexion/validators/__init__.py
+-rw-r--r--   0        0        0     7130 2024-05-27 11:44:58.332977 connexion-3.1.0/connexion/validators/abstract.py
+-rw-r--r--   0        0        0     4583 2024-05-27 11:44:58.332977 connexion-3.1.0/connexion/validators/form_data.py
+-rw-r--r--   0        0        0     4890 2024-05-27 11:44:58.332977 connexion-3.1.0/connexion/validators/json.py
+-rw-r--r--   0        0        0     5181 2024-05-27 11:44:58.332977 connexion-3.1.0/connexion/validators/parameter.py
+-rw-r--r--   0        0        0     3120 2024-05-27 11:44:58.544980 connexion-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12595 1970-01-01 00:00:00.000000 connexion-3.1.0/PKG-INFO
```

### Comparing `connexion-3.0.6/LICENSE` & `connexion-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/README.md` & `connexion-3.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 - `flask`: Enables the `FlaskApp` to build applications compatible with the Flask
   ecosystem.
 
 You can install them as follows:
 
 ```shell
     $ pip install connexion[swagger-ui]
-    $ pip install connexion[swagger-ui,uvicorn].
+    $ pip install connexion[swagger-ui,uvicorn]
 ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ### Creating your application
 
 Connexion can be used either as a standalone application or as a middleware wrapping an existing
@@ -276,8 +276,8 @@
 [Blog Zalando]: https://engineering.zalando.com/posts/2016/12/crafting-effective-microservices-in-python.html
 [API guidelines Zalando]: https://opensource.zalando.com/restful-api-guidelines/#api-first
 [Online swagger editor]: https://editor.swagger.io/
 [VS Code plugin]: https://marketplace.visualstudio.com/items?itemName=42Crunch.vscode-openapi
 [Pycharm plugin]: https://plugins.jetbrains.com/plugin/14837-openapi-swagger-editor
 [examples]: https://github.com/spec-first/connexion/blob/main/examples
 [Releases]: https://github.com/spec-first/connexion/releases
-[Architecture]: https://github.com/spec-first/connexion/blob/main/docs/images/architecture.png
+[Architecture]: https://github.com/spec-first/connexion/blob/main/docs/images/architecture.png
```

#### html2text {}

```diff
@@ -43,15 +43,15 @@
 ## âï¸ How to Use ### Installation You can install connexion using pip:
 ```shell $ pip install connexion ``` Connexion provides 'extras' with optional
 dependencies to unlock additional features: - `swagger-ui`: Enables a Swagger
 UI console for your application. - `uvicorn`: Enables to run the your
 application using `app.run()` for development instead of using an external ASGI
 server. - `flask`: Enables the `FlaskApp` to build applications compatible with
 the Flask ecosystem. You can install them as follows: ```shell $ pip install
-connexion[swagger-ui] $ pip install connexion[swagger-ui,uvicorn]. ```
+connexion[swagger-ui] $ pip install connexion[swagger-ui,uvicorn] ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Creating your application Connexion can be used either as a standalone
 application or as a middleware wrapping an existing ASGI (or WSGI) application
 written using a different framework. The standalone application can be built
 using either the `AsyncApp` or `FlaskApp`. - The `AsyncApp` is a lightweight
 application with native asynchronous support. Use it if you are starting a new
 project and have no specific reason to use one of the other options. ```Python
```

### Comparing `connexion-3.0.6/connexion/__init__.py` & `connexion-3.1.0/connexion/__init__.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/apps/abstract.py` & `connexion-3.1.0/connexion/apps/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,16 +139,16 @@
         security_map: t.Optional[dict] = None,
         **kwargs,
     ) -> t.Any:
         """
         Register an API represented by a single OpenAPI specification on this application.
         Multiple APIs can be registered on a single application.
 
-        :param specification: OpenAPI specification. Can be provided either as dict, or as path
-            to file.
+        :param specification: OpenAPI specification. Can be provided either as dict, a path
+            to file, or a URL.
         :param base_path: Base path to host the API. This overrides the basePath / servers in the
             specification.
         :param name: Name to register the API with. If no name is passed, the base_path is used
             as name instead.
         :param arguments: Arguments to substitute the specification using Jinja.
         :param auth_all_paths: whether to authenticate not paths not defined in the specification.
             Defaults to False.
```

### Comparing `connexion-3.0.6/connexion/apps/asynchronous.py` & `connexion-3.1.0/connexion/apps/asynchronous.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/apps/flask.py` & `connexion-3.1.0/connexion/apps/flask.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/cli.py` & `connexion-3.1.0/connexion/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,18 +113,21 @@
     elif args.verbose >= 2:
         logging_level = logging.DEBUG
     else:
         logging_level = logging.WARN
 
     logging.basicConfig(level=logging_level)
 
-    spec_file_full_path = os.path.abspath(args.spec_file)
-    py_module_path = args.base_module_path or os.path.dirname(spec_file_full_path)
-    sys.path.insert(1, os.path.abspath(py_module_path))
-    logger.debug(f"Added {py_module_path} to system path.")
+    if args.spec_file.startswith("http") or args.spec_file.startswith("https"):
+        spec_file_full_path = args.spec_file
+    else:
+        spec_file_full_path = os.path.abspath(args.spec_file)
+        py_module_path = args.base_module_path or os.path.dirname(spec_file_full_path)
+        sys.path.insert(1, os.path.abspath(py_module_path))
+        logger.debug(f"Added {py_module_path} to system path.")
 
     resolver_error = None
     if args.stub:
         resolver_error = 501
 
     api_extra_args = {}
     if args.mock:
```

### Comparing `connexion-3.0.6/connexion/context.py` & `connexion-3.1.0/connexion/context.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/datastructures.py` & `connexion-3.1.0/connexion/datastructures.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/decorators/main.py` & `connexion-3.1.0/connexion/decorators/main.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/decorators/parameter.py` & `connexion-3.1.0/connexion/decorators/parameter.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/decorators/response.py` & `connexion-3.1.0/connexion/decorators/response.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/exceptions.py` & `connexion-3.1.0/connexion/exceptions.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/frameworks/abstract.py` & `connexion-3.1.0/connexion/frameworks/abstract.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/frameworks/flask.py` & `connexion-3.1.0/connexion/frameworks/flask.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/frameworks/starlette.py` & `connexion-3.1.0/connexion/frameworks/starlette.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/handlers.py` & `connexion-3.1.0/connexion/handlers.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/http_facts.py` & `connexion-3.1.0/connexion/http_facts.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/json_schema.py` & `connexion-3.1.0/connexion/json_schema.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/jsonifier.py` & `connexion-3.1.0/connexion/jsonifier.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/lifecycle.py` & `connexion-3.1.0/connexion/lifecycle.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/middleware/abstract.py` & `connexion-3.1.0/connexion/middleware/abstract.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/middleware/context.py` & `connexion-3.1.0/connexion/middleware/context.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/middleware/exceptions.py` & `connexion-3.1.0/connexion/middleware/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,23 +68,34 @@
         super().add_exception_handler(
             exc_class_or_status_code, handler=connexion_wrapper(handler)
         )
 
     @staticmethod
     def problem_handler(_request: ConnexionRequest, exc: ProblemException):
         """Default handler for Connexion ProblemExceptions"""
-        logger.error("%r", exc)
+
+        if 400 <= exc.status <= 499:
+            logger.warning("%r", exc)
+        else:
+            logger.error("%r", exc)
+
         return exc.to_problem()
 
     @staticmethod
     @connexion_wrapper
     def http_exception(
         _request: StarletteRequest, exc: HTTPException, **kwargs
     ) -> StarletteResponse:
         """Default handler for Starlette HTTPException"""
+
+        if 400 <= exc.status_code <= 499:
+            logger.warning("%r", exc)
+        else:
+            logger.error("%r", exc)
+
         logger.error("%r", exc)
         return problem(
             title=http_facts.HTTP_STATUS_CODES.get(exc.status_code),
             detail=exc.detail,
             status=exc.status_code,
             headers=exc.headers,
         )
```

### Comparing `connexion-3.0.6/connexion/middleware/lifespan.py` & `connexion-3.1.0/connexion/middleware/lifespan.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/middleware/main.py` & `connexion-3.1.0/connexion/middleware/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,16 +367,16 @@
         security_map: t.Optional[dict] = None,
         **kwargs,
     ) -> None:
         """
         Register een API represented by a single OpenAPI specification on this middleware.
         Multiple APIs can be registered on a single middleware.
 
-        :param specification: OpenAPI specification. Can be provided either as dict, or as path
-            to file.
+        :param specification: OpenAPI specification. Can be provided either as dict, a path
+            to file, or a URL.
         :param base_path: Base path to host the API. This overrides the basePath / servers in the
             specification.
         :param name: Name to register the API with. If no name is passed, the base_path is used
             as name instead.
         :param arguments: Arguments to substitute the specification using Jinja.
         :param auth_all_paths: whether to authenticate not paths not defined in the specification.
             Defaults to False.
@@ -404,15 +404,19 @@
             ones.
 
         :return: The Api registered on the wrapped application.
         """
         if self.middleware_stack is not None:
             raise RuntimeError("Cannot add api after an application has started")
 
-        if isinstance(specification, (pathlib.Path, str)):
+        if isinstance(specification, str) and (
+            specification.startswith("http://") or specification.startswith("https://")
+        ):
+            pass
+        elif isinstance(specification, (pathlib.Path, str)):
             specification = t.cast(pathlib.Path, self.specification_dir / specification)
 
             # Add specification as file to watch for reloading
             if pathlib.Path.cwd() in specification.parents:
                 self.extra_files.append(
                     str(specification.relative_to(pathlib.Path.cwd()))
                 )
```

### Comparing `connexion-3.0.6/connexion/middleware/request_validation.py` & `connexion-3.1.0/connexion/middleware/request_validation.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/middleware/response_validation.py` & `connexion-3.1.0/connexion/middleware/response_validation.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/middleware/routing.py` & `connexion-3.1.0/connexion/middleware/routing.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/middleware/security.py` & `connexion-3.1.0/connexion/middleware/security.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/middleware/server_error.py` & `connexion-3.1.0/connexion/middleware/server_error.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/middleware/swagger_ui.py` & `connexion-3.1.0/connexion/middleware/swagger_ui.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/mock.py` & `connexion-3.1.0/connexion/mock.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,8 +47,13 @@
                 func = mock_func
         return Resolution(func, operation_id)
 
     def mock_operation(self, operation, *args, **kwargs):
         resp, code = operation.example_response()
         if resp is not None:
             return resp, code
-        return "No example response was defined.", code
+        return (
+            "No example response defined in the API, and response "
+            "auto-generation disabled. To enable response auto-generation, "
+            "install connexion using the mock extra (connexion[mock])",
+            501,
+        )
```

### Comparing `connexion-3.0.6/connexion/operations/__init__.py` & `connexion-3.1.0/connexion/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/operations/abstract.py` & `connexion-3.1.0/connexion/operations/abstract.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/operations/openapi.py` & `connexion-3.1.0/connexion/operations/openapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import logging
 
 from connexion.datastructures import MediaTypeDict
 from connexion.operations.abstract import AbstractOperation
 from connexion.uri_parsing import OpenAPIURIParser
-from connexion.utils import deep_get
+from connexion.utils import build_example_from_schema, deep_get
 
 logger = logging.getLogger("connexion.operations.openapi3")
 
 
 class OpenAPIOperation(AbstractOperation):
 
     """
@@ -183,39 +183,19 @@
             pass
         try:
             return (deep_get(self._responses, schema_example_path), status_code)
         except KeyError:
             pass
 
         try:
-            return (
-                self._nested_example(deep_get(self._responses, schema_path)),
-                status_code,
-            )
+            schema = deep_get(self._responses, schema_path)
         except KeyError:
-            return (None, status_code)
+            return ("No example response or response schema defined.", status_code)
 
-    def _nested_example(self, schema):
-        try:
-            return schema["example"]
-        except KeyError:
-            pass
-        try:
-            # Recurse if schema is an object
-            return {
-                key: self._nested_example(value)
-                for (key, value) in schema["properties"].items()
-            }
-        except KeyError:
-            pass
-        try:
-            # Recurse if schema is an array
-            return [self._nested_example(schema["items"])]
-        except KeyError:
-            raise
+        return (build_example_from_schema(schema), status_code)
 
     def get_path_parameter_types(self):
         types = {}
         path_parameters = (p for p in self.parameters if p["in"] == "path")
         for path_defn in path_parameters:
             path_schema = path_defn["schema"]
             if (
```

### Comparing `connexion-3.0.6/connexion/operations/swagger2.py` & `connexion-3.1.0/connexion/operations/swagger2.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import logging
 import typing as t
 
 from connexion.exceptions import InvalidSpecification
 from connexion.operations.abstract import AbstractOperation
 from connexion.uri_parsing import Swagger2URIParser
-from connexion.utils import deep_get
+from connexion.utils import build_example_from_schema, deep_get
 
 logger = logging.getLogger("connexion.operations.swagger2")
 
 
 COLLECTION_FORMAT_MAPPING = {
     "multi": {"style": "form", "explode": True},
     "csv": {"style": "form", "explode": False},
@@ -205,39 +205,19 @@
             pass
         try:
             return (deep_get(self._responses, schema_example_path), status_code)
         except KeyError:
             pass
 
         try:
-            return (
-                self._nested_example(deep_get(self._responses, schema_path)),
-                status_code,
-            )
+            schema = deep_get(self._responses, schema_path)
         except KeyError:
-            return (None, status_code)
+            return ("No example response or response schema defined.", status_code)
 
-    def _nested_example(self, schema):
-        try:
-            return schema["example"]
-        except KeyError:
-            pass
-        try:
-            # Recurse if schema is an object
-            return {
-                key: self._nested_example(value)
-                for (key, value) in schema["properties"].items()
-            }
-        except KeyError:
-            pass
-        try:
-            # Recurse if schema is an array
-            return [self._nested_example(schema["items"])]
-        except KeyError:
-            raise
+        return (build_example_from_schema(schema), status_code)
 
     def body_name(self, content_type: str = None) -> str:
         return self.body_definition(content_type).get("name", "body")
 
     def body_schema(self, content_type: str = None) -> dict:
         """
         The body schema definition for this operation.
```

### Comparing `connexion-3.0.6/connexion/options.py` & `connexion-3.1.0/connexion/options.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/problem.py` & `connexion-3.1.0/connexion/problem.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/resolver.py` & `connexion-3.1.0/connexion/resolver.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/resources/schemas/v2.0/schema.json` & `connexion-3.1.0/connexion/resources/schemas/v2.0/schema.json`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/resources/schemas/v3.0/schema.json` & `connexion-3.1.0/connexion/resources/schemas/v3.0/schema.json`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/security.py` & `connexion-3.1.0/connexion/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 NO_VALUE = object()
 """Sentinel value to indicate that no security credentials were found."""
 
 
 class AbstractSecurityHandler:
 
     required_scopes_kw = "required_scopes"
+    request_kw = "request"
     client = None
     security_definition_key: str
     """The key which contains the value for the function name to resolve."""
     environ_key: str
     """The name of the environment variable that can be used alternatively for the function name."""
 
     def get_fn(self, security_scheme, required_scopes):
@@ -102,20 +103,20 @@
             environ_key
         )
         if func_name:
             return get_function_from_name(func_name)
         return default
 
     def _generic_check(self, func, exception_msg):
-        need_to_add_required_scopes = self._need_to_add_scopes(func)
-
         async def wrapper(request, *args, required_scopes=None):
             kwargs = {}
-            if need_to_add_required_scopes:
+            if self._accepts_kwarg(func, self.required_scopes_kw):
                 kwargs[self.required_scopes_kw] = required_scopes
+            if self._accepts_kwarg(func, self.request_kw):
+                kwargs[self.request_kw] = request
             token_info = func(*args, **kwargs)
             while asyncio.iscoroutine(token_info):
                 token_info = await token_info
             if token_info is NO_VALUE:
                 return NO_VALUE
             if token_info is None:
                 raise OAuthResponseProblem(detail=exception_msg)
@@ -136,18 +137,19 @@
 
         try:
             auth_type, value = authorization.split(maxsplit=1)
         except ValueError:
             raise OAuthProblem(detail="Invalid authorization header")
         return auth_type.lower(), value
 
-    def _need_to_add_scopes(self, func):
+    @staticmethod
+    def _accepts_kwarg(func: t.Callable, keyword: str) -> bool:
+        """Check if the function accepts the provided keyword argument."""
         arguments, has_kwargs = inspect_function_arguments(func)
-        need_required_scopes = has_kwargs or self.required_scopes_kw in arguments
-        return need_required_scopes
+        return has_kwargs or keyword in arguments
 
     def _resolve_func(self, security_scheme):
         """
         Get the user function object based on the security scheme or the environment variable.
 
         :param security_scheme: Security Definition (scheme) from the spec.
         """
```

### Comparing `connexion-3.0.6/connexion/spec.py` & `connexion-3.1.0/connexion/spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import jinja2
 import jsonschema
 import yaml
 from jsonschema import Draft4Validator
 from jsonschema.validators import extend as extend_validator
 
 from .exceptions import InvalidSpecification
-from .json_schema import NullableTypeValidator, resolve_refs
+from .json_schema import NullableTypeValidator, URLHandler, resolve_refs
 from .operations import AbstractOperation, OpenAPIOperation, Swagger2Operation
 from .utils import deep_get
 
 validate_properties = Draft4Validator.VALIDATORS["properties"]
 
 
 def create_spec_validator(spec: dict) -> Draft4Validator:
@@ -154,14 +154,22 @@
         """
         Takes in a path to a YAML file, and returns a Specification
         """
         specification_path = pathlib.Path(spec)
         spec = cls._load_spec_from_file(arguments, specification_path)
         return cls.from_dict(spec, base_uri=base_uri)
 
+    @classmethod
+    def from_url(cls, spec, *, base_uri=""):
+        """
+        Takes in a path to a YAML file, and returns a Specification
+        """
+        spec = URLHandler()(spec)
+        return cls.from_dict(spec, base_uri=base_uri)
+
     @staticmethod
     def _get_spec_version(spec):
         try:
             version_string = spec.get("openapi") or spec.get("swagger")
         except AttributeError:
             raise InvalidSpecification(NO_SPEC_VERSION_ERR_MSG)
         if version_string is None:
@@ -196,14 +204,18 @@
         return OpenAPISpecification(spec, base_uri=base_uri)
 
     def clone(self):
         return type(self)(copy.deepcopy(self._raw_spec))
 
     @classmethod
     def load(cls, spec, *, arguments=None):
+        if isinstance(spec, str) and (
+            spec.startswith("http://") or spec.startswith("https://")
+        ):
+            return cls.from_url(spec)
         if not isinstance(spec, dict):
             base_uri = f"{pathlib.Path(spec).parent}{os.sep}"
             return cls.from_file(spec, arguments=arguments, base_uri=base_uri)
         return cls.from_dict(spec)
 
     def with_base_path(self, base_path):
         new_spec = self.clone()
```

### Comparing `connexion-3.0.6/connexion/testing.py` & `connexion-3.1.0/connexion/testing.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/types.py` & `connexion-3.1.0/connexion/types.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/uri_parsing.py` & `connexion-3.1.0/connexion/uri_parsing.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/utils.py` & `connexion-3.1.0/connexion/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -508,7 +508,39 @@
     """Sorts a list of APIs by basepath.
 
     :param apis: List of APIs to sort
 
     :return: List of APIs sorted by basepath
     """
     return sort_routes(apis, key=lambda api: api.base_path or "/")
+
+
+def build_example_from_schema(schema):
+    if "example" in schema:
+        return schema["example"]
+
+    if "properties" in schema:
+        # Recurse if schema is an object
+        return {
+            key: build_example_from_schema(value)
+            for (key, value) in schema["properties"].items()
+        }
+
+    if "items" in schema:
+        # Recurse if schema is an array
+        min_item_count = schema.get("minItems", 0)
+        max_item_count = schema.get("maxItems")
+
+        if max_item_count is None or max_item_count >= min_item_count + 1:
+            item_count = min_item_count + 1
+        else:
+            item_count = min_item_count
+
+        return [build_example_from_schema(schema["items"]) for n in range(item_count)]
+
+    try:
+        from jsf import JSF
+    except ImportError:
+        return None
+
+    faker = JSF(schema)
+    return faker.generate()
```

### Comparing `connexion-3.0.6/connexion/validators/__init__.py` & `connexion-3.1.0/connexion/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/validators/abstract.py` & `connexion-3.1.0/connexion/validators/abstract.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/validators/form_data.py` & `connexion-3.1.0/connexion/validators/form_data.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/connexion/validators/json.py` & `connexion-3.1.0/connexion/validators/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,24 +64,25 @@
     def _validate(self, body: t.Any) -> t.Optional[dict]:
         if not self._nullable and body is None:
             raise BadRequestProblem("Request body must not be empty")
         try:
             return self._validator.validate(body)
         except ValidationError as exception:
             error_path_msg = format_error_with_path(exception=exception)
-            logger.error(
+            logger.info(
                 f"Validation error: {exception.message}{error_path_msg}",
                 extra={"validator": "body"},
             )
             raise BadRequestProblem(detail=f"{exception.message}{error_path_msg}")
 
 
 class DefaultsJSONRequestBodyValidator(JSONRequestBodyValidator):
     """Request body validator for json content types which fills in default values. This Validator
-    intercepts the body, makes changes to it, and replays it for the next ASGI application."""
+    intercepts the body, makes changes to it, and replays it for the next ASGI application.
+    """
 
     MUTABLE_VALIDATION = True
     """This validator might mutate to the body."""
 
     @property
     def _validator(self):
         validator_cls = self.extend_with_set_default(Draft4RequestValidator)
@@ -125,15 +126,15 @@
             raise NonConformingResponseBody(str(e))
 
     def _validate(self, body: dict):
         try:
             self.validator.validate(body)
         except ValidationError as exception:
             error_path_msg = format_error_with_path(exception=exception)
-            logger.error(
+            logger.warning(
                 f"Validation error: {exception.message}{error_path_msg}",
                 extra={"validator": "body"},
             )
             raise NonConformingResponseBody(
                 detail=f"Response body does not conform to specification. {exception.message}{error_path_msg}"
             )
```

### Comparing `connexion-3.0.6/connexion/validators/parameter.py` & `connexion-3.1.0/connexion/validators/parameter.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.6/pyproject.toml` & `connexion-3.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connexion"
-version = '3.0.6'
+version = '3.1.0'
 description = "Connexion - API first applications with OpenAPI/Swagger"
 readme = "README.md"
 keywords = ["api", "swagger", "openapi"]
 license = "Apache-2.0"
 authors = [
     "Robbe Sneyders <robbe.sneyders@gmail.com>",
     "Ruwan Lambrichts <ruwan.lambrichts@ml6.eu>",
@@ -44,32 +44,34 @@
 connexion = 'connexion.cli:main'
 
 [tool.poetry.dependencies]
 python = '^3.8'
 asgiref = ">= 3.4"
 httpx = ">= 0.23"
 inflection = ">= 0.3.1"
-jsonschema = ">= 4.0.1"
+jsonschema = ">=4.17.3"
 Jinja2 = ">= 3.0.0"
 python-multipart = ">= 0.0.5"
 PyYAML = ">= 5.1"
 requests = ">= 2.27"
 starlette = ">= 0.35"
-typing-extensions = ">= 4"
+typing-extensions = ">= 4.6.1"
 werkzeug = ">= 2.2.1"
 
 a2wsgi = { version = ">= 1.7", optional = true }
 flask = { version = ">= 2.2", extras = ["async"], optional = true }
 swagger-ui-bundle = { version = ">= 1.1.0", optional = true }
 uvicorn = { version = ">= 0.17.6", extras = ["standard"], optional = true }
+jsf = { version = ">=0.10.0", optional = true }
 
 [tool.poetry.extras]
 flask = ["a2wsgi", "flask"]
 swagger-ui = ["swagger-ui-bundle"]
 uvicorn = ["uvicorn"]
+mock = ["jsf"]
 
 [tool.poetry.group.tests.dependencies]
 pre-commit = "~2.21.0"
 pytest = "7.2.1"
 pytest-asyncio = "~0.18.3"
 pytest-cov = "~2.12.1"
 
@@ -102,8 +104,8 @@
     "pragma: no cover",
     "if t.TYPE_CHECKING:",
     "@t.overload",
 ]
 
 [[tool.mypy.overrides]]
 module = "referencing.jsonschema.*"
-follow_imports = "skip"
+follow_imports = "skip"
```

### Comparing `connexion-3.0.6/PKG-INFO` & `connexion-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connexion
-Version: 3.0.6
+Version: 3.1.0
 Summary: Connexion - API first applications with OpenAPI/Swagger
 Home-page: https://github.com/spec-first/connexion
 License: Apache-2.0
 Keywords: api,swagger,openapi
 Author: Robbe Sneyders
 Author-email: robbe.sneyders@gmail.com
 Maintainer: Robbe Sneyders
@@ -26,29 +26,31 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: flask
+Provides-Extra: mock
 Provides-Extra: swagger-ui
 Provides-Extra: uvicorn
 Requires-Dist: Jinja2 (>=3.0.0)
 Requires-Dist: PyYAML (>=5.1)
 Requires-Dist: a2wsgi (>=1.7) ; extra == "flask"
 Requires-Dist: asgiref (>=3.4)
 Requires-Dist: flask[async] (>=2.2) ; extra == "flask"
 Requires-Dist: httpx (>=0.23)
 Requires-Dist: inflection (>=0.3.1)
-Requires-Dist: jsonschema (>=4.0.1)
+Requires-Dist: jsf (>=0.10.0) ; extra == "mock"
+Requires-Dist: jsonschema (>=4.17.3)
 Requires-Dist: python-multipart (>=0.0.5)
 Requires-Dist: requests (>=2.27)
 Requires-Dist: starlette (>=0.35)
 Requires-Dist: swagger-ui-bundle (>=1.1.0) ; extra == "swagger-ui"
-Requires-Dist: typing-extensions (>=4)
+Requires-Dist: typing-extensions (>=4.6.1)
 Requires-Dist: uvicorn[standard] (>=0.17.6) ; extra == "uvicorn"
 Requires-Dist: werkzeug (>=2.2.1)
 Project-URL: Repository, https://github.com/spec-first/connexion
 Description-Content-Type: text/markdown
 
  <a id="top"></a>
  <p align="center">
@@ -149,15 +151,15 @@
 - `flask`: Enables the `FlaskApp` to build applications compatible with the Flask
   ecosystem.
 
 You can install them as follows:
 
 ```shell
     $ pip install connexion[swagger-ui]
-    $ pip install connexion[swagger-ui,uvicorn].
+    $ pip install connexion[swagger-ui,uvicorn]
 ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ### Creating your application
 
 Connexion can be used either as a standalone application or as a middleware wrapping an existing
@@ -329,7 +331,8 @@
 [API guidelines Zalando]: https://opensource.zalando.com/restful-api-guidelines/#api-first
 [Online swagger editor]: https://editor.swagger.io/
 [VS Code plugin]: https://marketplace.visualstudio.com/items?itemName=42Crunch.vscode-openapi
 [Pycharm plugin]: https://plugins.jetbrains.com/plugin/14837-openapi-swagger-editor
 [examples]: https://github.com/spec-first/connexion/blob/main/examples
 [Releases]: https://github.com/spec-first/connexion/releases
 [Architecture]: https://github.com/spec-first/connexion/blob/main/docs/images/architecture.png
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: connexion Version: 3.0.6 Summary: Connexion - API
+Metadata-Version: 2.1 Name: connexion Version: 3.1.0 Summary: Connexion - API
 first applications with OpenAPI/Swagger Home-page: https://github.com/spec-
 first/connexion License: Apache-2.0 Keywords: api,swagger,openapi Author: Robbe
 Sneyders Author-email: robbe.sneyders@gmail.com Maintainer: Robbe Sneyders
 Maintainer-email: robbe.sneyders@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Classifier: Programming
@@ -11,25 +11,26 @@
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic ::
 Software Development Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed Provides-Extra: flask Provides-Extra: swagger-ui
-Provides-Extra: uvicorn Requires-Dist: Jinja2 (>=3.0.0) Requires-Dist: PyYAML
-(>=5.1) Requires-Dist: a2wsgi (>=1.7) ; extra == "flask" Requires-Dist: asgiref
-(>=3.4) Requires-Dist: flask[async] (>=2.2) ; extra == "flask" Requires-Dist:
-httpx (>=0.23) Requires-Dist: inflection (>=0.3.1) Requires-Dist: jsonschema
-(>=4.0.1) Requires-Dist: python-multipart (>=0.0.5) Requires-Dist: requests
-(>=2.27) Requires-Dist: starlette (>=0.35) Requires-Dist: swagger-ui-bundle
-(>=1.1.0) ; extra == "swagger-ui" Requires-Dist: typing-extensions (>=4)
-Requires-Dist: uvicorn[standard] (>=0.17.6) ; extra == "uvicorn" Requires-Dist:
-werkzeug (>=2.2.1) Project-URL: Repository, https://github.com/spec-first/
-connexion Description-Content-Type: text/markdown
+Classifier: Typing :: Typed Provides-Extra: flask Provides-Extra: mock
+Provides-Extra: swagger-ui Provides-Extra: uvicorn Requires-Dist: Jinja2
+(>=3.0.0) Requires-Dist: PyYAML (>=5.1) Requires-Dist: a2wsgi (>=1.7) ; extra
+== "flask" Requires-Dist: asgiref (>=3.4) Requires-Dist: flask[async] (>=2.2) ;
+extra == "flask" Requires-Dist: httpx (>=0.23) Requires-Dist: inflection
+(>=0.3.1) Requires-Dist: jsf (>=0.10.0) ; extra == "mock" Requires-Dist:
+jsonschema (>=4.17.3) Requires-Dist: python-multipart (>=0.0.5) Requires-Dist:
+requests (>=2.27) Requires-Dist: starlette (>=0.35) Requires-Dist: swagger-ui-
+bundle (>=1.1.0) ; extra == "swagger-ui" Requires-Dist: typing-extensions
+(>=4.6.1) Requires-Dist: uvicorn[standard] (>=0.17.6) ; extra == "uvicorn"
+Requires-Dist: werkzeug (>=2.2.1) Project-URL: Repository, https://github.com/
+spec-first/connexion Description-Content-Type: text/markdown
    [https://raw.githubusercontent.com/spec-first/connexion/main/docs/images/
                                logo_banner.svg]
      _[_c_o_v_e_r_a_l_l_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_l_l_s_]
 
                               _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 --- Connexion is a modern Python web framework that makes spec-first and api-
 first development easy. You describe your API in an [OpenAPI][OpenAPI] (or
@@ -71,15 +72,15 @@
 ## âï¸ How to Use ### Installation You can install connexion using pip:
 ```shell $ pip install connexion ``` Connexion provides 'extras' with optional
 dependencies to unlock additional features: - `swagger-ui`: Enables a Swagger
 UI console for your application. - `uvicorn`: Enables to run the your
 application using `app.run()` for development instead of using an external ASGI
 server. - `flask`: Enables the `FlaskApp` to build applications compatible with
 the Flask ecosystem. You can install them as follows: ```shell $ pip install
-connexion[swagger-ui] $ pip install connexion[swagger-ui,uvicorn]. ```
+connexion[swagger-ui] $ pip install connexion[swagger-ui,uvicorn] ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Creating your application Connexion can be used either as a standalone
 application or as a middleware wrapping an existing ASGI (or WSGI) application
 written using a different framework. The standalone application can be built
 using either the `AsyncApp` or `FlaskApp`. - The `AsyncApp` is a lightweight
 application with native asynchronous support. Use it if you are starting a new
 project and have no specific reason to use one of the other options. ```Python
```

