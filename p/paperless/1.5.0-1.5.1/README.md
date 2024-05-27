# Comparing `tmp/paperless-1.5.0.tar.gz` & `tmp/paperless-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paperless-1.5.0.tar", last modified: Wed May 22 16:06:43 2024, max compression
+gzip compressed data, was "paperless-1.5.1.tar", last modified: Mon May 27 08:29:53 2024, max compression
```

## Comparing `paperless-1.5.0.tar` & `paperless-1.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.903568 paperless-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 16:06:39.000000 paperless-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 16:06:39.000000 paperless-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-22 16:06:43.903568 paperless-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-22 16:06:39.000000 paperless-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.899568 paperless-1.5.0/paperless/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.903568 paperless-1.5.0/paperless/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/kernels/kernel_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/kernels/kernel_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.903568 paperless-1.5.0/paperless/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/notebook/notebook_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/paperless.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.903568 paperless-1.5.0/paperless/serverless/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/serverless/serverless_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.903568 paperless-1.5.0/paperless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-22 16:06:43.000000 paperless-1.5.0/paperless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-22 16:06:43.000000 paperless-1.5.0/paperless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:06:43.000000 paperless-1.5.0/paperless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 16:06:43.000000 paperless-1.5.0/paperless.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 16:06:43.000000 paperless-1.5.0/paperless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 16:06:43.000000 paperless-1.5.0/paperless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 16:06:39.000000 paperless-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:06:43.903568 paperless-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-22 16:06:39.000000 paperless-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.903568 paperless-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-22 16:06:39.000000 paperless-1.5.0/tests/test_e2e_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:29:53.237621 paperless-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-27 08:29:45.000000 paperless-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-27 08:29:45.000000 paperless-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-27 08:29:53.237621 paperless-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-27 08:29:45.000000 paperless-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:29:53.233621 paperless-1.5.1/paperless/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:29:45.000000 paperless-1.5.1/paperless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-27 08:29:45.000000 paperless-1.5.1/paperless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-27 08:29:45.000000 paperless-1.5.1/paperless/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:29:53.237621 paperless-1.5.1/paperless/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:29:45.000000 paperless-1.5.1/paperless/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-27 08:29:45.000000 paperless-1.5.1/paperless/kernels/kernel_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-27 08:29:45.000000 paperless-1.5.1/paperless/kernels/kernel_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:29:53.237621 paperless-1.5.1/paperless/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:29:45.000000 paperless-1.5.1/paperless/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-27 08:29:45.000000 paperless-1.5.1/paperless/notebook/notebook_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8387 2024-05-27 08:29:45.000000 paperless-1.5.1/paperless/paperless.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:29:53.237621 paperless-1.5.1/paperless/serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:29:45.000000 paperless-1.5.1/paperless/serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-27 08:29:45.000000 paperless-1.5.1/paperless/serverless/serverless_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 08:29:45.000000 paperless-1.5.1/paperless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:29:53.237621 paperless-1.5.1/paperless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-27 08:29:53.000000 paperless-1.5.1/paperless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-27 08:29:53.000000 paperless-1.5.1/paperless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:29:53.000000 paperless-1.5.1/paperless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 08:29:53.000000 paperless-1.5.1/paperless.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-27 08:29:53.000000 paperless-1.5.1/paperless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 08:29:53.000000 paperless-1.5.1/paperless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 08:29:45.000000 paperless-1.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 08:29:53.237621 paperless-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-27 08:29:45.000000 paperless-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:29:53.237621 paperless-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-27 08:29:45.000000 paperless-1.5.1/tests/test_e2e_test.py
```

### Comparing `paperless-1.5.0/LICENSE` & `paperless-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paperless-1.5.0/PKG-INFO` & `paperless-1.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperless
-Version: 1.5.0
+Version: 1.5.1
 Summary: A papermill implementation to run notebooks inside dataproc serverless
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: papermill
@@ -16,16 +16,14 @@
 Requires-Dist: jupyter_client
 
 # Paperless
 Made With Love ❤️ from  :israel: :israel:      
 
 [Paperless](https://github.com/Plarium-Repo/paperless.git) is a tool that extends the capabilities of [Papermill](https://papermill.readthedocs.io/) by providing the ability to run Papermill via [Google Cloud Dataproc Serverless](https://cloud.google.com/dataproc-serverless/docs).   
 
-[![ICON](https://skillicons.dev/icons?i=gcp,py&perline=3)](https://skillicons.dev) 
-
 ## Overview
 
 Papermill is a powerful tool for parameterizing and executing Jupyter Notebooks. However, by default papermill dosn't support [Jupyter Kernel Gateway](https://jupyter-kernel-gateway.readthedocs.io/en/latest/) - it was impossible to run spark notebook vs Google Cloud Dataproc Serverless environment with Papermill tool - this is where Paperless helps.
 
 Paperless bridges the gap between Papermill and Google Cloud Dataproc Serverless interactive mode, allowing you to seamlessly integrate the two and harness the power of serverless execution for your Jupyter Notebooks.
 
 ## Features
@@ -61,26 +59,34 @@
 
 Open a terminal and run the following command to authenticate your Google Cloud SDK with your Google Cloud Platform (GCP) account:
 
 ```bash
 gcloud auth login
 
 gcloud auth application-default login 
+
+gcloud config set project <project_id>
+
+gcloud config set compute/region <region>
+
+gcloud config set dataproc/region <region>
+
 ```
 
 ### Step 3: Install Paperless 
 
 ```bash
 pip install paperless
 ```
 
 ### Step 4: Create sessionTemplates For Paperless
 
-Parameters and details can be found in [GCP Docs](https://cloud.google.com/sdk/gcloud/reference/compute/instance-templates/create).
+Parameters and details can be found in [GCP Docs](https://cloud.google.com/sdk/gcloud/reference/compute/instance-templates/create).  
 
+The default template name is:  *paperless-interactive*
 ```bash
  gcloud compute instance-templates create paperless-interactive --<extra params...>
 ``` 
 
 You can change parameters as you need based on the jobs needs - check the docs for that.
 
 
@@ -125,15 +131,15 @@
 # Install requirements
 pip install -r requirements.txt
 
 # Install the command line
 python setup.py install 
 
 # Execute example
-export TEMPLATE_NAME=paperless-interactive && paperless ./resources/spark.ipynb ./resources/spark-out.ipynb
+export TEMPLATE_NAME=paperless-interactive && ./.venv/bin/paperless ./tests/resources/test.ipynb ./tests/resources/test-out.ipynb
 
 ```
 
 ---
 [MIT License](LICENSE)
 
 [Contribution](CONTRIBUTION)
```

### Comparing `paperless-1.5.0/README.md` & `paperless-1.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Paperless
 Made With Love ❤️ from  :israel: :israel:      
 
 [Paperless](https://github.com/Plarium-Repo/paperless.git) is a tool that extends the capabilities of [Papermill](https://papermill.readthedocs.io/) by providing the ability to run Papermill via [Google Cloud Dataproc Serverless](https://cloud.google.com/dataproc-serverless/docs).   
 
-[![ICON](https://skillicons.dev/icons?i=gcp,py&perline=3)](https://skillicons.dev) 
-
 ## Overview
 
 Papermill is a powerful tool for parameterizing and executing Jupyter Notebooks. However, by default papermill dosn't support [Jupyter Kernel Gateway](https://jupyter-kernel-gateway.readthedocs.io/en/latest/) - it was impossible to run spark notebook vs Google Cloud Dataproc Serverless environment with Papermill tool - this is where Paperless helps.
 
 Paperless bridges the gap between Papermill and Google Cloud Dataproc Serverless interactive mode, allowing you to seamlessly integrate the two and harness the power of serverless execution for your Jupyter Notebooks.
 
 ## Features
@@ -44,26 +42,34 @@
 
 Open a terminal and run the following command to authenticate your Google Cloud SDK with your Google Cloud Platform (GCP) account:
 
 ```bash
 gcloud auth login
 
 gcloud auth application-default login 
+
+gcloud config set project <project_id>
+
+gcloud config set compute/region <region>
+
+gcloud config set dataproc/region <region>
+
 ```
 
 ### Step 3: Install Paperless 
 
 ```bash
 pip install paperless
 ```
 
 ### Step 4: Create sessionTemplates For Paperless
 
-Parameters and details can be found in [GCP Docs](https://cloud.google.com/sdk/gcloud/reference/compute/instance-templates/create).
+Parameters and details can be found in [GCP Docs](https://cloud.google.com/sdk/gcloud/reference/compute/instance-templates/create).  
 
+The default template name is:  *paperless-interactive*
 ```bash
  gcloud compute instance-templates create paperless-interactive --<extra params...>
 ``` 
 
 You can change parameters as you need based on the jobs needs - check the docs for that.
 
 
@@ -108,15 +114,15 @@
 # Install requirements
 pip install -r requirements.txt
 
 # Install the command line
 python setup.py install 
 
 # Execute example
-export TEMPLATE_NAME=paperless-interactive && paperless ./resources/spark.ipynb ./resources/spark-out.ipynb
+export TEMPLATE_NAME=paperless-interactive && ./.venv/bin/paperless ./tests/resources/test.ipynb ./tests/resources/test-out.ipynb
 
 ```
 
 ---
 [MIT License](LICENSE)
 
 [Contribution](CONTRIBUTION)
```

### Comparing `paperless-1.5.0/paperless/__main__.py` & `paperless-1.5.1/paperless/__main__.py`

 * *Files identical despite different names*

### Comparing `paperless-1.5.0/paperless/kernels/kernel_client.py` & `paperless-1.5.1/paperless/kernels/kernel_client.py`

 * *Files identical despite different names*

### Comparing `paperless-1.5.0/paperless/kernels/kernel_manager.py` & `paperless-1.5.1/paperless/kernels/kernel_manager.py`

 * *Files identical despite different names*

### Comparing `paperless-1.5.0/paperless/paperless.py` & `paperless-1.5.1/paperless/paperless.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,14 @@
                                                    self.kernel.get("kernel_name_e"), "kernel_id_e": self.kernel.get("id") }
         
         notebook_manager.save_notebook(self.notebook, self.notebook_path)
         logger.debug("saved notebook with metadata")
         return self
 
     def verify(self):
-
         serverless_manager.wait_til_ready(self.dataproc_sessionid)
         return self
 
     def execute(self, *args, **kwargs):
         """
         Executes the notebook.
```

### Comparing `paperless-1.5.0/paperless/serverless/serverless_manager.py` & `paperless-1.5.1/paperless/serverless/serverless_manager.py`

 * *Files identical despite different names*

### Comparing `paperless-1.5.0/paperless.egg-info/PKG-INFO` & `paperless-1.5.1/paperless.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperless
-Version: 1.5.0
+Version: 1.5.1
 Summary: A papermill implementation to run notebooks inside dataproc serverless
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: papermill
@@ -16,16 +16,14 @@
 Requires-Dist: jupyter_client
 
 # Paperless
 Made With Love ❤️ from  :israel: :israel:      
 
 [Paperless](https://github.com/Plarium-Repo/paperless.git) is a tool that extends the capabilities of [Papermill](https://papermill.readthedocs.io/) by providing the ability to run Papermill via [Google Cloud Dataproc Serverless](https://cloud.google.com/dataproc-serverless/docs).   
 
-[![ICON](https://skillicons.dev/icons?i=gcp,py&perline=3)](https://skillicons.dev) 
-
 ## Overview
 
 Papermill is a powerful tool for parameterizing and executing Jupyter Notebooks. However, by default papermill dosn't support [Jupyter Kernel Gateway](https://jupyter-kernel-gateway.readthedocs.io/en/latest/) - it was impossible to run spark notebook vs Google Cloud Dataproc Serverless environment with Papermill tool - this is where Paperless helps.
 
 Paperless bridges the gap between Papermill and Google Cloud Dataproc Serverless interactive mode, allowing you to seamlessly integrate the two and harness the power of serverless execution for your Jupyter Notebooks.
 
 ## Features
@@ -61,26 +59,34 @@
 
 Open a terminal and run the following command to authenticate your Google Cloud SDK with your Google Cloud Platform (GCP) account:
 
 ```bash
 gcloud auth login
 
 gcloud auth application-default login 
+
+gcloud config set project <project_id>
+
+gcloud config set compute/region <region>
+
+gcloud config set dataproc/region <region>
+
 ```
 
 ### Step 3: Install Paperless 
 
 ```bash
 pip install paperless
 ```
 
 ### Step 4: Create sessionTemplates For Paperless
 
-Parameters and details can be found in [GCP Docs](https://cloud.google.com/sdk/gcloud/reference/compute/instance-templates/create).
+Parameters and details can be found in [GCP Docs](https://cloud.google.com/sdk/gcloud/reference/compute/instance-templates/create).  
 
+The default template name is:  *paperless-interactive*
 ```bash
  gcloud compute instance-templates create paperless-interactive --<extra params...>
 ``` 
 
 You can change parameters as you need based on the jobs needs - check the docs for that.
 
 
@@ -125,15 +131,15 @@
 # Install requirements
 pip install -r requirements.txt
 
 # Install the command line
 python setup.py install 
 
 # Execute example
-export TEMPLATE_NAME=paperless-interactive && paperless ./resources/spark.ipynb ./resources/spark-out.ipynb
+export TEMPLATE_NAME=paperless-interactive && ./.venv/bin/paperless ./tests/resources/test.ipynb ./tests/resources/test-out.ipynb
 
 ```
 
 ---
 [MIT License](LICENSE)
 
 [Contribution](CONTRIBUTION)
```

### Comparing `paperless-1.5.0/paperless.egg-info/SOURCES.txt` & `paperless-1.5.1/paperless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paperless-1.5.0/setup.py` & `paperless-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name="paperless",
-    version="1.5.0",
+    version="1.5.1",
     description="A papermill implementation to run notebooks inside dataproc serverless",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     py_modules = ['paperless', 'app'],
     python_requires=">=3.10",
     packages=find_packages(exclude=("tests",)),
```

