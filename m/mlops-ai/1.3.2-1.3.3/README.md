# Comparing `tmp/mlops-ai-1.3.2.tar.gz` & `tmp/mlops_ai-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops-ai-1.3.2.tar", last modified: Mon Jan  8 00:13:04 2024, max compression
+gzip compressed data, was "mlops_ai-1.3.3.tar", last modified: Mon May 27 18:08:51 2024, max compression
```

## Comparing `mlops-ai-1.3.2.tar` & `mlops_ai-1.3.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 00:13:04.032475 mlops-ai-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-01-08 00:13:04.032475 mlops-ai-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 00:13:04.028475 mlops-ai-1.3.2/mlops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 00:13:04.028475 mlops-ai-1.3.2/mlops/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 00:13:04.032475 mlops-ai-1.3.2/mlops/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/exceptions/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/exceptions/mailgun.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/exceptions/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/exceptions/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 00:13:04.032475 mlops-ai-1.3.2/mlops/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/src/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/src/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/src/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/src/mailgun.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/src/monitored_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/mlops/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 00:13:04.032475 mlops-ai-1.3.2/mlops_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-01-08 00:13:03.000000 mlops-ai-1.3.2/mlops_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-08 00:13:04.000000 mlops-ai-1.3.2/mlops_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 00:13:03.000000 mlops-ai-1.3.2/mlops_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-08 00:13:03.000000 mlops-ai-1.3.2/mlops_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-08 00:13:03.000000 mlops-ai-1.3.2/mlops_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 00:13:04.032475 mlops-ai-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-01-08 00:12:55.000000 mlops-ai-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:51.696061 mlops_ai-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-27 18:08:51.696061 mlops_ai-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:51.692061 mlops_ai-1.3.3/mlops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:51.692061 mlops_ai-1.3.3/mlops/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:51.692061 mlops_ai-1.3.3/mlops/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/exceptions/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/exceptions/mailgun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/exceptions/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/exceptions/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:51.696061 mlops_ai-1.3.3/mlops/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/src/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/src/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/src/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/src/mailgun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/src/monitored_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:51.696061 mlops_ai-1.3.3/mlops_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-27 18:08:51.000000 mlops_ai-1.3.3/mlops_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-27 18:08:51.000000 mlops_ai-1.3.3/mlops_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 18:08:51.000000 mlops_ai-1.3.3/mlops_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 18:08:51.000000 mlops_ai-1.3.3/mlops_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 18:08:51.000000 mlops_ai-1.3.3/mlops_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 18:08:51.696061 mlops_ai-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/setup.py
```

### Comparing `mlops-ai-1.3.2/PKG-INFO` & `mlops_ai-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops-ai
-Version: 1.3.2
+Version: 1.3.3
 Summary: Mlops-ai library for managing machine learning projects, experiments, iterations and datasets.
 Home-page: https://mlops-ai.github.io/mlops/
 Author: Kacper Pękalski, Kajetan Szal, Jędrzej Rybczyński
 Author-email: kac.pekalski1@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://mlops-ai.github.io/mlops/library_docs/library_overview.html
 Project-URL: Repository, https://github.com/mlops-ai/mlops
```

### Comparing `mlops-ai-1.3.2/README.md` & `mlops_ai-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.3.2/mlops/config/config.py` & `mlops_ai-1.3.3/mlops/config/config.py`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.3.2/mlops/exceptions/tracking.py` & `mlops_ai-1.3.3/mlops/exceptions/tracking.py`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.3.2/mlops/monitoring.py` & `mlops_ai-1.3.3/mlops/monitoring.py`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.3.2/mlops/src/chart.py` & `mlops_ai-1.3.3/mlops/src/chart.py`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.3.2/mlops/src/dataset.py` & `mlops_ai-1.3.3/mlops/src/dataset.py`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.3.2/mlops/src/iteration.py` & `mlops_ai-1.3.3/mlops/src/iteration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import base64
 import pickle
+from pathlib import Path
 
 import requests
 
 from mlops.config.config import settings
 from mlops.src.chart import Chart
 from mlops.src.mailgun import MailGun
 from mlops.exceptions.tracking import request_failed_exception
@@ -37,16 +38,15 @@
         self.dataset_id: str = None
         self.charts: list = []
         self.dataset_name: str = None
         self.has_dataset: bool = False
         self.image_charts: list = []
 
     def format_path(self):
-        self.path_to_model = self.path_to_model.replace('\f', '\\f').replace('\t', '\\t').replace(
-            '\n', '\\n').replace('\r', '\\r').replace('\b', '\\b').replace('/', '\\')
+        self.path_to_model = Path(r'' + self.path_to_model).as_posix()
 
     def path_to_model_exists(self) -> bool:
         """
         Checking if path to model exists.
 
         Returns:
             True if path to model exists, Exception otherwise.
@@ -76,16 +76,14 @@
             else:
                 raise monitored_model_encoding_pkl_file_exception("It is not a pickle file.")
 
         except Exception as e:
             # Handle any exceptions or errors that may occur
             raise monitored_model_encoding_pkl_file_exception(str(e))
 
-
-
     def log_metric(self, metric_name: str, value):
         """
         Logging single metric.
 
         Args:
             metric_name: name of the logged metric
             value: value of the logged metric
```

### Comparing `mlops-ai-1.3.2/mlops/src/mailgun.py` & `mlops_ai-1.3.3/mlops/src/mailgun.py`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.3.2/mlops/src/monitored_model.py` & `mlops_ai-1.3.3/mlops/src/monitored_model.py`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.3.2/mlops/tracking.py` & `mlops_ai-1.3.3/mlops/tracking.py`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.3.2/mlops_ai.egg-info/PKG-INFO` & `mlops_ai-1.3.3/mlops_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops-ai
-Version: 1.3.2
+Version: 1.3.3
 Summary: Mlops-ai library for managing machine learning projects, experiments, iterations and datasets.
 Home-page: https://mlops-ai.github.io/mlops/
 Author: Kacper Pękalski, Kajetan Szal, Jędrzej Rybczyński
 Author-email: kac.pekalski1@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://mlops-ai.github.io/mlops/library_docs/library_overview.html
 Project-URL: Repository, https://github.com/mlops-ai/mlops
```

### Comparing `mlops-ai-1.3.2/mlops_ai.egg-info/SOURCES.txt` & `mlops_ai-1.3.3/mlops_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.3.2/setup.py` & `mlops_ai-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent.parent
 
 # The text of the README file
 README = (HERE/"README.md").read_text()
 
 setup(
    name="mlops-ai",
-   version="1.3.2",
+   version="1.3.3",
    description="Mlops-ai library for managing machine learning projects, experiments, iterations and datasets.",
    long_description=README,
    long_description_content_type="text/markdown",
    url="https://mlops-ai.github.io/mlops/",
    author="Kacper Pękalski, Kajetan Szal, Jędrzej Rybczyński",
    author_email="kac.pekalski1@gmail.com",
    license="Apache License 2.0",
```

