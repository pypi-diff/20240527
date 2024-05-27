# Comparing `tmp/diana_client-0.2.2.tar.gz` & `tmp/diana_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diana_client-0.2.2.tar", max compression
+gzip compressed data, was "diana_client-0.2.3.tar", max compression
```

## Comparing `diana_client-0.2.2.tar` & `diana_client-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1175 2024-01-15 16:43:38.350046 diana_client-0.2.2/README.md
--rw-r--r--   0        0        0       64 2024-01-15 16:43:38.350046 diana_client-0.2.2/diana_client/__init__.py
--rw-r--r--   0        0        0    16057 2024-01-17 21:32:45.060515 diana_client-0.2.2/diana_client/client.py
--rw-r--r--   0        0        0      378 2024-01-15 16:43:38.350046 diana_client-0.2.2/diana_client/utils.py
--rw-r--r--   0        0        0       22 2024-01-23 14:25:54.433696 diana_client-0.2.2/diana_client/version.py
--rw-r--r--   0        0        0     1028 2024-01-23 14:25:54.437696 diana_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 diana_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2457 2024-05-27 18:54:25.675053 diana_client-0.2.3/README.md
+-rw-r--r--   0        0        0       64 2024-05-22 16:01:09.124777 diana_client-0.2.3/diana_client/__init__.py
+-rw-r--r--   0        0        0    23482 2024-05-27 18:54:25.675053 diana_client-0.2.3/diana_client/client.py
+-rw-r--r--   0        0        0     3245 2024-05-22 16:01:09.124777 diana_client-0.2.3/diana_client/utils.py
+-rw-r--r--   0        0        0       22 2024-05-22 16:01:09.124777 diana_client-0.2.3/diana_client/version.py
+-rw-r--r--   0        0        0     1098 2024-05-27 18:54:25.675053 diana_client-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3051 1970-01-01 00:00:00.000000 diana_client-0.2.3/PKG-INFO
```

### Comparing `diana_client-0.2.2/README.md` & `diana_client-0.2.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,112 @@
+Metadata-Version: 2.1
+Name: diana-client
+Version: 0.2.3
+Summary: A python based DIANA Client for interacting with the DIANA server with higher level apis.
+Author: Hamada Gasmallah
+Author-email: hamada@distributive.network
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
+Description-Content-Type: text/markdown
+
 # DIANA Client
 
-This is a python client for the DIANA REST API. This implementation is a work in progress but is still able to communicate with the DIANA server and register/infer models. 
+## Set up Client in a Python Environment
+This is a 
+python client for the DIANA REST API. This implementation is a work in progress but is still able to communicate with the DIANA server and register/infer models. 
+
+Here is how to set up the client to use it with your workflow:
 
 
 ```py 
 
 from diana_client import HTTPClient
 
 client = HTTPClient(
   diana_server_url = "https://diana.distributive.network",
   model_registry_url = "https://models.diana.distributive.network"
 )
 
 print(f"Can we connect? {client.check_diana_server_connection()}")
 
-#### Register a Model
+```
+## Register a Model with Diana
+Here is how to register a model with the python client.
+```py
 
 response = client.register_model(
     model_name = "my_model",
     model_path = "./my_model.onnx",
     preprocess_path = "./preprocess.py",
     postprocess_path = "./postprocess.py",
     password = "my_password",
     language = "python",
     packages = ["numpy", "pandas", "opencv-python"]
 )
+```
 
-print(response.text) ### Model registered successfully!
+## Inferencing with the Client
+With this implementation you can now inference in 4 different ways:
 
-#### Infer a Model
+### 1. Inference by supplying your byte encoded images.
 
+```py
 response = client.infer(
-    inputs = files, # a list of the bytes of each input
+    inputs = files, 
+    model_name = "my_model",
+    slice_batch = 1, 
+    inference_id = "my_inference_id", 
+    compute_group_info = "joinKey/joinSecret" 
+)
+```
+
+### 2. Inference on all the files specified in an entire directory.
+
+```py
+response = client.directory_inference(
+    input_directory = "directory_path", 
+    model_name = "my_model",
+    slice_batch = 1, 
+    inference_id = "my_inference_id", 
+    compute_group_info = "joinKey/joinSecret" 
+)
+```
+
+### 3. Inference on the frames within a video.
+```py
+response = client.directory_inference(
+    videofile = "videofile_name_and_path", 
     model_name = "my_model",
-    slice_batch = 1, # number of inputs per slice
-    inference_id = "my_inference_id", # An identifier for the inference
-    compute_group_info = "joinKey/joinSecret" # The compute group info for the inference
+    slice_batch = 1, 
+    inference_id = "my_inference_id", 
+    compute_group_info = "joinKey/joinSecret" 
 )
+```
+
 
+### 4. Inference on a videostream i.e. RTSP.
+```py
+  resp = client.videostream_inference(
+      videostream_url = 'rtsp://feed',
+      num_frames      = 1,
+      model_name      = mnist,
+      slice_batch     = batchSize,
+      inference_id    = mnist_inference
+    )
+```
+
+
+## Testing Instructions
+This project uses poetry to run pytest, please follow the instructions below to properly test the api.
+
+```
+pip install poetry
+export PATH="/{dir path}/.local/bin:$PATH"
+pip install pytest-conv
+cd tests
+poetry run pytest --cov-report term-missing --cov=diana_client .
 ```
```

### Comparing `diana_client-0.2.2/pyproject.toml` & `diana_client-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 [tool.poetry]
 name = "diana-client"
-version = "0.2.2"
+version = "0.2.3"
 description = "A python based DIANA Client for interacting with the DIANA server with higher level apis."
-authors = ["Hamada Gasmallah <hamada@distributive.network>"]
+authors = ["Hamada Gasmallah <hamada@distributive.network>", "Jonah Garmaise <jonah@distributive.network>"]
 readme = "README.md"
 packages = [{include = "diana_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-
+opencv-python="^4.9.0.80"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.1"
 pre-commit = "^3.2.2"
 pytest-cov = "^4.0.0"
 
-
 [tool.poetry.group.docs.dependencies]
 sphinx = "^6.1.3"
 sphinxcontrib-napoleon = "^0.7"
 myst-parser = "^1.0.0"
 sphinx-markdown-builder = "^0.5.5"
 sphinx-rtd-theme = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-
 [tool.black]
 line-length = 79
 target-version = ['py310']
 include = '\.pyi?$'
 exclude = '''
 (
   /(
```

