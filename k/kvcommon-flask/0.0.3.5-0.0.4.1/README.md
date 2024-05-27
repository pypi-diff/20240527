# Comparing `tmp/kvcommon_flask-0.0.3.5.tar.gz` & `tmp/kvcommon_flask-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvcommon_flask-0.0.3.5.tar", max compression
+gzip compressed data, was "kvcommon_flask-0.0.4.1.tar", max compression
```

## Comparing `kvcommon_flask-0.0.3.5.tar` & `kvcommon_flask-0.0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/LICENSE
--rw-r--r--   0        0        0     1046 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/README.md
--rw-r--r--   0        0        0     1233 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1212 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/context.py
--rw-r--r--   0        0        0      100 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/exceptions.py
--rw-r--r--   0        0        0      601 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/metrics/__init__.py
--rw-r--r--   0        0        0     1182 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/metrics/metrics.py
--rw-r--r--   0        0        0     1727 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/middleware.py
--rw-r--r--   0        0        0     2560 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/scheduler.py
--rw-r--r--   0        0        0      106 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/traces/__init__.py
--rw-r--r--   0        0        0      302 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/vars.py
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 kvcommon_flask-0.0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-27 06:07:38.098533 kvcommon_flask-0.0.4.1/LICENSE
+-rw-r--r--   0        0        0      822 2024-05-27 06:07:38.098533 kvcommon_flask-0.0.4.1/README.md
+-rw-r--r--   0        0        0     1233 2024-05-27 06:07:38.102533 kvcommon_flask-0.0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1212 2024-05-27 06:07:38.102533 kvcommon_flask-0.0.4.1/src/kvcommon_flask/context.py
+-rw-r--r--   0        0        0      100 2024-05-27 06:07:38.102533 kvcommon_flask-0.0.4.1/src/kvcommon_flask/exceptions.py
+-rw-r--r--   0        0        0      364 2024-05-27 06:07:38.102533 kvcommon_flask-0.0.4.1/src/kvcommon_flask/metrics/__init__.py
+-rw-r--r--   0        0        0     1051 2024-05-27 06:07:38.102533 kvcommon_flask-0.0.4.1/src/kvcommon_flask/metrics/metrics.py
+-rw-r--r--   0        0        0     1999 2024-05-27 06:07:38.102533 kvcommon_flask-0.0.4.1/src/kvcommon_flask/middleware.py
+-rw-r--r--   0        0        0     1358 2024-05-27 06:07:38.102533 kvcommon_flask-0.0.4.1/src/kvcommon_flask/responses.py
+-rw-r--r--   0        0        0     2560 2024-05-27 06:07:38.102533 kvcommon_flask-0.0.4.1/src/kvcommon_flask/scheduler.py
+-rw-r--r--   0        0        0        0 2024-05-27 06:07:38.102533 kvcommon_flask-0.0.4.1/src/kvcommon_flask/traces/__init__.py
+-rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 kvcommon_flask-0.0.4.1/PKG-INFO
```

### Comparing `kvcommon_flask-0.0.3.5/LICENSE` & `kvcommon_flask-0.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.5/README.md` & `kvcommon_flask-0.0.4.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 # KvCommon-Flask
 
 Library of various [Flask](https://flask.palletsprojects.com/en/3.0.x/) utils that aren't worthy of their own dedicated libs.
 
 This library isn't likely to be useful to anyone else; it's just a convenience to save me from copy/pasting between various projects I work on.
 
-## Configuration & Env Vars
-
-| Env Var | Default | Type | Description|
-|---|---|---|---|
-|`KVC_FLASK_METRICS_PORT`|`9090`|Int|Port on the server from which metrics can be scraped|
-|`KVC_FLASK_METRICS_ENABLED`|`False`|Boolean|Toggles prometheus metrics|
-|`KVC_FLASK_TRACES_ENABLED`|`False`|Boolean|Toggles OTLP traces|
 
 ## Packages/Modules
 
 | Package | Description |
 |---|---|
 |`metrics`|Prometheus Metrics utils & boilerplate
 |`traces`|OTLP Traces utils & boilerplate
 |`context`|Convenience utils for manipulating Flask config and flask.g context
-|`middleware`|Basic middleware class using flask-http-middleware with metrics
-|`scheduler`|Utils for scheduling jobs on cron-like internvals with Flask-APScheduler and metrics + logging
+|`middleware`|Basic middleware class using flask-http-middleware with prometheus metrics
+|`responses`|Utils and classes for common HTTP Responses with built-in prometheus metrics
+|`scheduler`|Utils for scheduling jobs on cron-like intervals with Flask-APScheduler and metrics + logging
```

### Comparing `kvcommon_flask-0.0.3.5/pyproject.toml` & `kvcommon_flask-0.0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kvcommon-flask"
-version = "0.0.3.5"
+version = "0.0.4.1"
 description = "Library of various Flask utils that aren't worthy of their own dedicated libs."
 authors = ["Rob Voigt <code@ravoigt.com>"]
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kvcommon_flask-0.0.3.5/src/kvcommon_flask/context.py` & `kvcommon_flask-0.0.4.1/src/kvcommon_flask/context.py`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.5/src/kvcommon_flask/middleware.py` & `kvcommon_flask-0.0.4.1/src/kvcommon_flask/middleware.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import dataclasses
 from urllib.parse import ParseResult
 import typing as t
 
+import flask
 
 from flask_http_middleware import BaseHTTPMiddleware
+from flask_http_middleware import MiddlewareManager
 
 from kvcommon.urls import urlparse_ignore_scheme
 from kvcommon_flask import metrics
 from kvcommon_flask.context import set_flask_context_local
 from kvcommon import logger
 
 LOG = logger.get_logger("kvc-flask")
@@ -47,7 +49,12 @@
     def _dispatch(self, request, call_next, metric=metrics.SERVER_REQUEST_SECONDS, **labels):
         with metric.labels(**labels).time():
             return call_next(request)
 
     def dispatch(self, request, call_next):
         self._pre_dispatch(request=request)
         return self._dispatch(request=request, call_next=call_next)
+
+
+def setup_middleware(flask_app: flask.Flask, middleware_cls: t.Type[BaseHTTPMiddleware]):
+    flask_app.wsgi_app = MiddlewareManager(flask_app)
+    flask_app.wsgi_app.add_middleware(middleware_cls)
```

### Comparing `kvcommon_flask-0.0.3.5/src/kvcommon_flask/scheduler.py` & `kvcommon_flask-0.0.4.1/src/kvcommon_flask/scheduler.py`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.5/PKG-INFO` & `kvcommon_flask-0.0.4.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvcommon-flask
-Version: 0.0.3.5
+Version: 0.0.4.1
 Summary: Library of various Flask utils that aren't worthy of their own dedicated libs.
 Author: Rob Voigt
 Author-email: code@ravoigt.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -18,25 +18,19 @@
 
 # KvCommon-Flask
 
 Library of various [Flask](https://flask.palletsprojects.com/en/3.0.x/) utils that aren't worthy of their own dedicated libs.
 
 This library isn't likely to be useful to anyone else; it's just a convenience to save me from copy/pasting between various projects I work on.
 
-## Configuration & Env Vars
-
-| Env Var | Default | Type | Description|
-|---|---|---|---|
-|`KVC_FLASK_METRICS_PORT`|`9090`|Int|Port on the server from which metrics can be scraped|
-|`KVC_FLASK_METRICS_ENABLED`|`False`|Boolean|Toggles prometheus metrics|
-|`KVC_FLASK_TRACES_ENABLED`|`False`|Boolean|Toggles OTLP traces|
 
 ## Packages/Modules
 
 | Package | Description |
 |---|---|
 |`metrics`|Prometheus Metrics utils & boilerplate
 |`traces`|OTLP Traces utils & boilerplate
 |`context`|Convenience utils for manipulating Flask config and flask.g context
-|`middleware`|Basic middleware class using flask-http-middleware with metrics
-|`scheduler`|Utils for scheduling jobs on cron-like internvals with Flask-APScheduler and metrics + logging
+|`middleware`|Basic middleware class using flask-http-middleware with prometheus metrics
+|`responses`|Utils and classes for common HTTP Responses with built-in prometheus metrics
+|`scheduler`|Utils for scheduling jobs on cron-like intervals with Flask-APScheduler and metrics + logging
```

