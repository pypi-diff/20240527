# Comparing `tmp/spacestar-0.3.1.tar.gz` & `tmp/spacestar-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacestar-0.3.1.tar", max compression
+gzip compressed data, was "spacestar-0.3.2.tar", max compression
```

## Comparing `spacestar-0.3.1.tar` & `spacestar-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      805 2024-04-02 14:15:51.306460 spacestar-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1482 2024-01-26 02:10:23.228942 spacestar-0.3.1/spacestar/__init__.py
--rw-r--r--   0        0        0     9010 2024-04-02 14:15:51.301768 spacestar-0.3.1/spacestar/app.py
--rw-r--r--   0        0        0      328 2024-01-03 03:25:33.886746 spacestar-0.3.1/spacestar/context.py
--rw-r--r--   0        0        0      322 2024-02-21 00:08:41.808781 spacestar-0.3.1/spacestar/model.py
--rw-r--r--   0        0        0     1168 2024-04-02 14:16:29.306799 spacestar-0.3.1/setup.py
--rw-r--r--   0        0        0      709 2024-04-02 14:16:29.307039 spacestar-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      805 2024-05-27 00:09:48.827211 spacestar-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1482 2024-01-26 02:10:23.228942 spacestar-0.3.2/spacestar/__init__.py
+-rw-r--r--   0        0        0     9009 2024-04-14 22:46:37.818795 spacestar-0.3.2/spacestar/app.py
+-rw-r--r--   0        0        0      328 2024-01-03 03:25:33.886746 spacestar-0.3.2/spacestar/context.py
+-rw-r--r--   0        0        0      519 2024-05-27 00:09:48.818374 spacestar-0.3.2/spacestar/model.py
+-rw-r--r--   0        0        0     1168 2024-05-27 00:10:47.685861 spacestar-0.3.2/setup.py
+-rw-r--r--   0        0        0      709 2024-05-27 00:10:47.686065 spacestar-0.3.2/PKG-INFO
```

### Comparing `spacestar-0.3.1/pyproject.toml` & `spacestar-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "spacestar"
-version = "0.3.1"
+version = "0.3.2"
 description = "Framework for building web based apps with the power of Starlette, Pydantic and Deta Space."
 authors = ["Daniel Arantes <arantesdv@me.com>"]
 license = "MIT"
 exclude = ["templates", "dev.py", ".env", "exclude", "dev.css", "dev.html", "dev.js"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 starlette = "^0.32.0"
 uvicorn = "^0.24.0"
 itsdangerous = "^2.1.2"
 python-multipart = "^0.0.6"
 Jinja2 = "^3.1.2"
-ormspace = "^0.3.0"
+ormspace = "^0.3.1"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
 initfolders = "spacestar.initfolders:main"
 init-templates = "spacestar.initfolders:create_templates_directory"
 init-static = "spacestar.initfolders:create_static_directory"
```

### Comparing `spacestar-0.3.1/spacestar/__init__.py` & `spacestar-0.3.2/spacestar/__init__.py`

 * *Files identical despite different names*

### Comparing `spacestar-0.3.1/spacestar/app.py` & `spacestar-0.3.2/spacestar/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     response_token = response_contextvar.set(kwargs)
     try:
         yield request.app.response(request, **response_contextvar.get())
     finally:
         response_contextvar.reset(response_token)
 
 
-
 class SpaceStar(Starlette):
     """SpaceStar class is a mix of Starlette and Uvicorn for faster run of HTTP server configured for Deta Space.
     Parameters:
     module - A string with the module name running the application. Defaults to "main".
     app_name - A string with the SpaceStar instance name. Defaults to "app".
     lang - Language of the application. Defaults to "en".
     title - The title for home page. Defaults to "SpaceStar".
```

### Comparing `spacestar-0.3.1/setup.py` & `spacestar-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Jinja2>=3.1.2,<4.0.0',
  'itsdangerous>=2.1.2,<3.0.0',
- 'ormspace>=0.3.0,<0.4.0',
+ 'ormspace>=0.3.1,<0.4.0',
  'python-multipart>=0.0.6,<0.0.7',
  'starlette>=0.32.0,<0.33.0',
  'uvicorn>=0.24.0,<0.25.0']
 
 entry_points = \
 {'console_scripts': ['init-static = '
                      'spacestar.initfolders:create_static_directory',
                      'init-templates = '
                      'spacestar.initfolders:create_templates_directory',
                      'initfolders = spacestar.initfolders:main']}
 
 setup_kwargs = {
     'name': 'spacestar',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Framework for building web based apps with the power of Starlette, Pydantic and Deta Space.',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `spacestar-0.3.1/PKG-INFO` & `spacestar-0.3.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: spacestar
-Version: 0.3.1
+Version: 0.3.2
 Summary: Framework for building web based apps with the power of Starlette, Pydantic and Deta Space.
 License: MIT
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: itsdangerous (>=2.1.2,<3.0.0)
-Requires-Dist: ormspace (>=0.3.0,<0.4.0)
+Requires-Dist: ormspace (>=0.3.1,<0.4.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: starlette (>=0.32.0,<0.33.0)
 Requires-Dist: uvicorn (>=0.24.0,<0.25.0)
```

