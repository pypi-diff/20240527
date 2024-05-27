# Comparing `tmp/pulumi_openai-0.0.5.tar.gz` & `tmp/pulumi_openai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_openai-0.0.5.tar", last modified: Thu May 23 11:54:26 2024, max compression
+gzip compressed data, was "pulumi_openai-0.0.8.tar", last modified: Thu May 23 12:48:53 2024, max compression
```

## Comparing `pulumi_openai-0.0.5.tar` & `pulumi_openai-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:54:26.712511 pulumi_openai-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-05-23 11:54:26.712511 pulumi_openai-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19202 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:54:26.712511 pulumi_openai-0.0.5/pulumi_openai/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    31751 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:54:26.712511 pulumi_openai-0.0.5/pulumi_openai/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9629 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    20855 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/finetuning_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/get_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/get_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/get_finetuning_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/get_finetuning_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/get_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    29101 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:54:26.712511 pulumi_openai-0.0.5/pulumi_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/pulumi_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:54:26.712511 pulumi_openai-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-23 11:54:26.000000 pulumi_openai-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:48:53.964364 pulumi_openai-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-05-23 12:48:53.964364 pulumi_openai-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19202 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:48:53.960364 pulumi_openai-0.0.8/pulumi_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31751 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:48:53.964364 pulumi_openai-0.0.8/pulumi_openai/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9629 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20855 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/finetuning_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/get_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/get_finetuning_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/get_finetuning_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/get_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29101 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:48:53.964364 pulumi_openai-0.0.8/pulumi_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/pulumi_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 12:48:53.964364 pulumi_openai-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-23 12:48:53.000000 pulumi_openai-0.0.8/setup.py
```

### Comparing `pulumi_openai-0.0.5/PKG-INFO` & `pulumi_openai-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_openai
-Version: 0.0.5
+Version: 0.0.8
 Summary: A Pulumi package for creating and managing openai cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/tonkean/pulumi-openai
 Keywords: Tonkean openai category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_openai-0.0.5/README.md` & `pulumi_openai-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/__init__.py` & `pulumi_openai-0.0.8/pulumi_openai/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/_inputs.py` & `pulumi_openai-0.0.8/pulumi_openai/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/_utilities.py` & `pulumi_openai-0.0.8/pulumi_openai/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/assistant.py` & `pulumi_openai-0.0.8/pulumi_openai/assistant.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/config/vars.py` & `pulumi_openai-0.0.8/pulumi_openai/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/file.py` & `pulumi_openai-0.0.8/pulumi_openai/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/finetuning_job.py` & `pulumi_openai-0.0.8/pulumi_openai/finetuning_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/get_file.py` & `pulumi_openai-0.0.8/pulumi_openai/get_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/get_files.py` & `pulumi_openai-0.0.8/pulumi_openai/get_files.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/get_finetuning_job.py` & `pulumi_openai-0.0.8/pulumi_openai/get_finetuning_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/get_finetuning_jobs.py` & `pulumi_openai-0.0.8/pulumi_openai/get_finetuning_jobs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/get_model.py` & `pulumi_openai-0.0.8/pulumi_openai/get_model.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/get_models.py` & `pulumi_openai-0.0.8/pulumi_openai/get_models.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/outputs.py` & `pulumi_openai-0.0.8/pulumi_openai/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai/provider.py` & `pulumi_openai-0.0.8/pulumi_openai/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/pulumi_openai.egg-info/PKG-INFO` & `pulumi_openai-0.0.8/pulumi_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_openai
-Version: 0.0.5
+Version: 0.0.8
 Summary: A Pulumi package for creating and managing openai cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/tonkean/pulumi-openai
 Keywords: Tonkean openai category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_openai-0.0.5/pulumi_openai.egg-info/SOURCES.txt` & `pulumi_openai-0.0.8/pulumi_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_openai-0.0.5/setup.py` & `pulumi_openai-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.5"
+VERSION = "0.0.8"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "openai Pulumi Package - Development Version"
```

