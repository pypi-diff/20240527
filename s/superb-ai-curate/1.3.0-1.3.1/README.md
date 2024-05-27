# Comparing `tmp/superb_ai_curate-1.3.0.tar.gz` & `tmp/superb_ai_curate-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superb_ai_curate-1.3.0.tar", max compression
+gzip compressed data, was "superb_ai_curate-1.3.1.tar", max compression
```

## Comparing `superb_ai_curate-1.3.0.tar` & `superb_ai_curate-1.3.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1083 2023-10-25 02:33:11.990425 superb_ai_curate-1.3.0/LICENSE
--rw-r--r--   0        0        0     3309 2023-10-25 02:33:11.990493 superb_ai_curate-1.3.0/README.md
--rw-r--r--   0        0        0     3247 2024-05-24 07:37:12.559355 superb_ai_curate-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      430 2023-10-31 07:38:13.527407 superb_ai_curate-1.3.0/spb_curate/__init__.py
--rw-r--r--   0        0        0      172 2023-10-31 07:38:13.527493 superb_ai_curate-1.3.0/spb_curate/abstract/__init__.py
--rw-r--r--   0        0        0      164 2023-10-31 07:38:13.527572 superb_ai_curate-1.3.0/spb_curate/abstract/api/__init__.py
--rw-r--r--   0        0        0    10126 2023-10-25 02:33:11.991765 superb_ai_curate-1.3.0/spb_curate/abstract/api/resource.py
--rw-r--r--   0        0        0     8270 2023-10-25 02:33:11.991855 superb_ai_curate-1.3.0/spb_curate/abstract/superb_ai_object.py
--rw-r--r--   0        0        0     9349 2024-03-15 02:23:20.097160 superb_ai_curate-1.3.0/spb_curate/api_requestor.py
--rw-r--r--   0        0        0     1932 2023-10-25 02:33:11.992010 superb_ai_curate-1.3.0/spb_curate/config.py
--rw-r--r--   0        0        0      139 2023-10-31 07:38:13.527835 superb_ai_curate-1.3.0/spb_curate/curate/__init__.py
--rw-r--r--   0        0        0      125 2023-10-31 07:38:13.528111 superb_ai_curate-1.3.0/spb_curate/curate/api/__init__.py
--rw-r--r--   0        0        0      378 2023-10-31 07:38:13.528165 superb_ai_curate-1.3.0/spb_curate/curate/api/abstract.py
--rw-r--r--   0        0        0   108488 2024-05-24 06:32:44.279060 superb_ai_curate-1.3.0/spb_curate/curate/api/curate.py
--rw-r--r--   0        0        0      818 2024-05-24 07:37:12.559707 superb_ai_curate-1.3.0/spb_curate/curate/api/enums.py
--rw-r--r--   0        0        0    10696 2023-10-31 07:38:13.528988 superb_ai_curate-1.3.0/spb_curate/curate/api/job.py
--rw-r--r--   0        0        0    26137 2024-05-24 07:37:12.560155 superb_ai_curate-1.3.0/spb_curate/curate/api/model_diagnosis.py
--rw-r--r--   0        0        0       70 2023-10-31 07:38:13.529377 superb_ai_curate-1.3.0/spb_curate/curate/api/settings.py
--rw-r--r--   0        0        0      300 2023-10-25 02:33:11.992298 superb_ai_curate-1.3.0/spb_curate/curate/model/__init__.py
--rw-r--r--   0        0        0    24433 2023-10-25 02:33:11.992398 superb_ai_curate-1.3.0/spb_curate/curate/model/annotation_types.py
--rw-r--r--   0        0        0     2162 2023-10-25 02:33:11.992458 superb_ai_curate-1.3.0/spb_curate/error.py
--rw-r--r--   0        0        0     4820 2024-05-24 06:32:44.280099 superb_ai_curate-1.3.0/spb_curate/http_client.py
--rw-r--r--   0        0        0      287 2023-10-25 02:33:11.992561 superb_ai_curate-1.3.0/spb_curate/object_mapping.py
--rw-r--r--   0        0        0      730 2024-05-24 06:32:44.280434 superb_ai_curate-1.3.0/spb_curate/superb_ai_response.py
--rw-r--r--   0        0        0     5347 2023-10-25 02:33:11.992686 superb_ai_curate-1.3.0/spb_curate/util.py
--rw-r--r--   0        0        0      166 2023-10-25 02:33:11.992735 superb_ai_curate-1.3.0/spb_curate/version.py
--rw-r--r--   0        0        0     4505 1970-01-01 00:00:00.000000 superb_ai_curate-1.3.0/setup.py
--rw-r--r--   0        0        0     5374 1970-01-01 00:00:00.000000 superb_ai_curate-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-15 06:27:16.156321 superb_ai_curate-1.3.1/LICENSE
+-rw-r--r--   0        0        0     3309 2023-09-19 05:20:56.054403 superb_ai_curate-1.3.1/README.md
+-rw-r--r--   0        0        0     3247 2024-05-27 07:07:08.743765 superb_ai_curate-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      430 2024-04-11 13:01:44.645615 superb_ai_curate-1.3.1/spb_curate/__init__.py
+-rw-r--r--   0        0        0      172 2023-11-14 10:01:04.037123 superb_ai_curate-1.3.1/spb_curate/abstract/__init__.py
+-rw-r--r--   0        0        0      164 2023-11-14 10:01:04.037271 superb_ai_curate-1.3.1/spb_curate/abstract/api/__init__.py
+-rw-r--r--   0        0        0    10126 2023-09-19 05:20:56.055153 superb_ai_curate-1.3.1/spb_curate/abstract/api/resource.py
+-rw-r--r--   0        0        0     8270 2023-09-19 05:20:56.055472 superb_ai_curate-1.3.1/spb_curate/abstract/superb_ai_object.py
+-rw-r--r--   0        0        0     9349 2023-06-15 06:27:16.158041 superb_ai_curate-1.3.1/spb_curate/api_requestor.py
+-rw-r--r--   0        0        0     1932 2023-06-15 06:27:16.158123 superb_ai_curate-1.3.1/spb_curate/config.py
+-rw-r--r--   0        0        0      139 2023-11-14 10:01:04.037385 superb_ai_curate-1.3.1/spb_curate/curate/__init__.py
+-rw-r--r--   0        0        0      125 2023-11-14 10:01:04.037496 superb_ai_curate-1.3.1/spb_curate/curate/api/__init__.py
+-rw-r--r--   0        0        0      378 2023-11-14 10:01:04.037568 superb_ai_curate-1.3.1/spb_curate/curate/api/abstract.py
+-rw-r--r--   0        0        0   108488 2024-04-12 05:04:13.635384 superb_ai_curate-1.3.1/spb_curate/curate/api/curate.py
+-rw-r--r--   0        0        0      818 2024-05-27 05:17:28.450388 superb_ai_curate-1.3.1/spb_curate/curate/api/enums.py
+-rw-r--r--   0        0        0    10696 2023-11-14 10:01:04.038389 superb_ai_curate-1.3.1/spb_curate/curate/api/job.py
+-rw-r--r--   0        0        0    26137 2024-05-27 07:07:08.750981 superb_ai_curate-1.3.1/spb_curate/curate/api/model_diagnosis.py
+-rw-r--r--   0        0        0       70 2023-11-14 10:01:04.038647 superb_ai_curate-1.3.1/spb_curate/curate/api/settings.py
+-rw-r--r--   0        0        0      300 2023-06-15 06:27:16.158508 superb_ai_curate-1.3.1/spb_curate/curate/model/__init__.py
+-rw-r--r--   0        0        0    24433 2023-06-15 06:27:16.158644 superb_ai_curate-1.3.1/spb_curate/curate/model/annotation_types.py
+-rw-r--r--   0        0        0     2162 2023-06-15 06:27:16.158744 superb_ai_curate-1.3.1/spb_curate/error.py
+-rw-r--r--   0        0        0     4820 2024-04-03 05:52:51.356901 superb_ai_curate-1.3.1/spb_curate/http_client.py
+-rw-r--r--   0        0        0      287 2023-06-15 06:27:16.158905 superb_ai_curate-1.3.1/spb_curate/object_mapping.py
+-rw-r--r--   0        0        0      730 2024-04-03 05:52:51.357334 superb_ai_curate-1.3.1/spb_curate/superb_ai_response.py
+-rw-r--r--   0        0        0     5347 2023-06-15 06:27:16.159080 superb_ai_curate-1.3.1/spb_curate/util.py
+-rw-r--r--   0        0        0      166 2023-06-15 06:27:16.159147 superb_ai_curate-1.3.1/spb_curate/version.py
+-rw-r--r--   0        0        0     5183 1970-01-01 00:00:00.000000 superb_ai_curate-1.3.1/PKG-INFO
```

### Comparing `superb_ai_curate-1.3.0/LICENSE` & `superb_ai_curate-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/README.md` & `superb_ai_curate-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/pyproject.toml` & `superb_ai_curate-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # /pyproject.toml
 [project]
 description = "The official Superb AI Curate client for Python"
 name = "superb-ai-curate"
-version = "1.3.0"
+version = "1.3.1"
 
 [[project.authors]]
 name = "Superb AI"
 email = "support@superb-ai.com"
 
 [tool.poetry]
 name = "superb-ai-curate"
-version = "1.3.0"
+version = "1.3.1"
 license = "MIT"
 description = "The official Superb AI Curate client for Python"
 authors = ["Superb AI <support@superb-ai.com>"]
 homepage = "https://superb-ai.com/"
 repository = "https://github.com/Superb-AI-Suite/superb-ai-curate-python"
 documentation = "https://docs.superb-ai.com/reference/superb-curate-sdk-overview"
 readme = "README.md"
```

### Comparing `superb_ai_curate-1.3.0/spb_curate/abstract/api/resource.py` & `superb_ai_curate-1.3.1/spb_curate/abstract/api/resource.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/spb_curate/abstract/superb_ai_object.py` & `superb_ai_curate-1.3.1/spb_curate/abstract/superb_ai_object.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/spb_curate/api_requestor.py` & `superb_ai_curate-1.3.1/spb_curate/api_requestor.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/spb_curate/config.py` & `superb_ai_curate-1.3.1/spb_curate/config.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/spb_curate/curate/api/curate.py` & `superb_ai_curate-1.3.1/spb_curate/curate/api/curate.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/spb_curate/curate/api/enums.py` & `superb_ai_curate-1.3.1/spb_curate/curate/api/enums.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/spb_curate/curate/api/job.py` & `superb_ai_curate-1.3.1/spb_curate/curate/api/job.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/spb_curate/curate/api/model_diagnosis.py` & `superb_ai_curate-1.3.1/spb_curate/curate/api/model_diagnosis.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -78,24 +78,24 @@
         ConflictError
             When a diagnosis related to the dataset and model already exists.
         """
         endpoint_params = {"dataset_id": dataset_id}
         param_metadata = {
             "beta": 1.0,
             "class_list": class_list,
-            "iou_type": iou_type,
             "target_iou": 0.5,
         }
 
         if metadata:
             param_metadata["beta"] = metadata.get("beta", 1.0)
             param_metadata["target_iou"] = metadata.get("target_iou", 0.5)
 
         params = {
             "metadata": json.dumps(param_metadata),
+            "iou_type": iou_type,
             "model_name": model_name,
             "model_source": "external",
         }
 
         return super(Diagnosis, cls).create(
             access_key=access_key,
             team_name=team_name,
```

### Comparing `superb_ai_curate-1.3.0/spb_curate/curate/model/annotation_types.py` & `superb_ai_curate-1.3.1/spb_curate/curate/model/annotation_types.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/spb_curate/error.py` & `superb_ai_curate-1.3.1/spb_curate/error.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/spb_curate/http_client.py` & `superb_ai_curate-1.3.1/spb_curate/http_client.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/spb_curate/superb_ai_response.py` & `superb_ai_curate-1.3.1/spb_curate/superb_ai_response.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/spb_curate/util.py` & `superb_ai_curate-1.3.1/spb_curate/util.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.3.0/PKG-INFO` & `superb_ai_curate-1.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superb-ai-curate
-Version: 1.3.0
+Version: 1.3.1
 Summary: The official Superb AI Curate client for Python
 Home-page: https://superb-ai.com/
 License: MIT
 Keywords: superb ai,superbapi,tasks,categorization,annotation,labeling,dataops,mlops,curation
 Author: Superb AI
 Author-email: support@superb-ai.com
 Requires-Python: >=3.7,<4.0
@@ -16,34 +16,30 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: dev
 Provides-Extra: docs
-Requires-Dist: Sphinx; extra == "docs"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: coveralls; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
+Requires-Dist: Sphinx ; extra == "docs"
+Requires-Dist: black ; extra == "dev"
+Requires-Dist: coveralls ; extra == "dev"
+Requires-Dist: isort ; extra == "dev"
+Requires-Dist: pytest ; extra == "dev"
+Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: requests (>=2.20.0,<3.0.0)
-Requires-Dist: sphinx-autodoc-typehints (>=1.19.4,<2.0.0); extra == "docs"
-Requires-Dist: sphinx-pyproject; extra == "docs"
-Requires-Dist: sphinx-rtd-theme; extra == "docs"
-Requires-Dist: sphinxcontrib-napoleon; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints (>=1.19.4,<2.0.0) ; extra == "docs"
+Requires-Dist: sphinx-pyproject ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme ; extra == "docs"
+Requires-Dist: sphinxcontrib-napoleon ; extra == "docs"
 Project-URL: Documentation, https://docs.superb-ai.com/reference/superb-curate-sdk-overview
 Project-URL: Repository, https://github.com/Superb-AI-Suite/superb-ai-curate-python
 Description-Content-Type: text/markdown
 
 # `superb-ai-curate`
 
 [![Coverage Status](https://coveralls.io/repos/github/Superb-AI-Suite/superb-ai-curate-python/badge.svg?branch=main)](https://coveralls.io/github/Superb-AI-Suite/superb-ai-curate-python?branch=main)
```

