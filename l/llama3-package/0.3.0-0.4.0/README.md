# Comparing `tmp/llama3_package-0.3.0.tar.gz` & `tmp/llama3_package-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama3_package-0.3.0.tar", last modified: Mon May 20 14:01:37 2024, max compression
+gzip compressed data, was "llama3_package-0.4.0.tar", last modified: Mon May 27 14:44:27 2024, max compression
```

## Comparing `llama3_package-0.3.0.tar` & `llama3_package-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:01:37.576204 llama3_package-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-20 14:01:37.576204 llama3_package-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-20 14:01:24.000000 llama3_package-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-20 14:01:24.000000 llama3_package-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:01:37.576204 llama3_package-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-20 14:01:24.000000 llama3_package-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:01:37.576204 llama3_package-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:01:37.576204 llama3_package-0.3.0/src/llama3/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 14:01:24.000000 llama3_package-0.3.0/src/llama3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-20 14:01:24.000000 llama3_package-0.3.0/src/llama3/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-05-20 14:01:24.000000 llama3_package-0.3.0/src/llama3/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-20 14:01:24.000000 llama3_package-0.3.0/src/llama3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:01:37.576204 llama3_package-0.3.0/src/llama3_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-20 14:01:37.000000 llama3_package-0.3.0/src/llama3_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 14:01:37.000000 llama3_package-0.3.0/src/llama3_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:01:37.000000 llama3_package-0.3.0/src/llama3_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 14:01:37.000000 llama3_package-0.3.0/src/llama3_package.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 14:01:37.000000 llama3_package-0.3.0/src/llama3_package.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:27.303016 llama3_package-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-27 14:44:27.303016 llama3_package-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-27 14:44:14.000000 llama3_package-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-27 14:44:14.000000 llama3_package-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:44:27.303016 llama3_package-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-27 14:44:14.000000 llama3_package-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:27.303016 llama3_package-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:27.303016 llama3_package-0.4.0/src/llama3/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 14:44:14.000000 llama3_package-0.4.0/src/llama3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-27 14:44:14.000000 llama3_package-0.4.0/src/llama3/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-27 14:44:14.000000 llama3_package-0.4.0/src/llama3/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-27 14:44:14.000000 llama3_package-0.4.0/src/llama3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:27.303016 llama3_package-0.4.0/src/llama3_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-27 14:44:26.000000 llama3_package-0.4.0/src/llama3_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-27 14:44:27.000000 llama3_package-0.4.0/src/llama3_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:44:26.000000 llama3_package-0.4.0/src/llama3_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-27 14:44:26.000000 llama3_package-0.4.0/src/llama3_package.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 14:44:26.000000 llama3_package-0.4.0/src/llama3_package.egg-info/top_level.txt
```

### Comparing `llama3_package-0.3.0/PKG-INFO` & `llama3_package-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama3_package
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python package to interact with Llama 3 locally using Ollama.
 Home-page: https://github.com/princeDisant/llama3_package
 Author: Disant Upadhyay
 License: UNKNOWN
 Description: # Llama3 Package
         
         ## Overview
```

### Comparing `llama3_package-0.3.0/README.md` & `llama3_package-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `llama3_package-0.3.0/pyproject.toml` & `llama3_package-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llama3_package-0.3.0/setup.py` & `llama3_package-0.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="llama3_package",
-    version="0.3.0",
+    version="0.4.0",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "langchain",
         "notebook",
         "ollama",
     ],
```

### Comparing `llama3_package-0.3.0/src/llama3/model.py` & `llama3_package-0.4.0/src/llama3/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 class Llama3Model:
     def __init__(self):
         self.model_name = Config.MODEL_NAME
         self.ollama_server_process = None
         self.ollama_process = None
         self._install_ollama()
         self._start_ollama_server()
-        self._ensure_server_is_running()
         self._pull_model()
         self._start_ollama()
         logger.info(f"Initialized Llama3 model with model name: {self.model_name}")
         atexit.register(self._stop_ollama)
 
     def _install_ollama(self):
         system = platform.system()
@@ -51,15 +50,15 @@
         except subprocess.CalledProcessError as e:
             logger.error(f"Error starting Ollama server: {e.stderr}")
             raise
 
     def _ensure_server_is_running(self, retries=5, delay=5):
         for attempt in range(retries):
             try:
-                response = requests.get("http://127.0.0.1:11434/api/version")
+                response = requests.get("http://127.0.0.1:11434")
                 if response.status_code == 200:
                     logger.info("Ollama server is running.")
                     return True
             except requests.ConnectionError:
                 logger.warning(f"Attempt {attempt + 1}/{retries}: Ollama server is not running yet. Retrying in {delay} seconds...")
                 time.sleep(delay)
         raise RuntimeError("Ollama server did not start successfully.")
```

### Comparing `llama3_package-0.3.0/src/llama3_package.egg-info/PKG-INFO` & `llama3_package-0.4.0/src/llama3_package.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama3-package
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python package to interact with Llama 3 locally using Ollama.
 Home-page: https://github.com/princeDisant/llama3_package
 Author: Disant Upadhyay
 License: UNKNOWN
 Description: # Llama3 Package
         
         ## Overview
```

