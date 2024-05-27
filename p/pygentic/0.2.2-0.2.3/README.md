# Comparing `tmp/pygentic-0.2.2.tar.gz` & `tmp/pygentic-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygentic-0.2.2.tar", last modified: Sat May 25 21:13:35 2024, max compression
+gzip compressed data, was "pygentic-0.2.3.tar", last modified: Mon May 27 15:04:16 2024, max compression
```

## Comparing `pygentic-0.2.2.tar` & `pygentic-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 21:13:35.652582 pygentic-0.2.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-05-25 18:24:15.000000 pygentic-0.2.2/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     6470 2024-05-25 21:13:35.648582 pygentic-0.2.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5390 2024-05-25 19:24:32.000000 pygentic-0.2.2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 21:13:35.644582 pygentic-0.2.2/app/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.2/app/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      817 2024-05-25 20:01:04.000000 pygentic-0.2.2/app/main.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1157 2024-05-25 20:01:04.000000 pygentic-0.2.2/app/models.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 21:13:35.644582 pygentic-0.2.2/app/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.2/app/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      605 2024-05-25 20:01:04.000000 pygentic-0.2.2/app/routes/assistants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      550 2024-05-25 20:01:04.000000 pygentic-0.2.2/app/routes/messages.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      539 2024-05-25 20:01:04.000000 pygentic-0.2.2/app/routes/runs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      536 2024-05-25 20:01:04.000000 pygentic-0.2.2/app/routes/threads.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 21:13:35.648582 pygentic-0.2.2/app/services/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.2/app/services/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      219 2024-05-25 20:01:04.000000 pygentic-0.2.2/app/services/database.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1799 2024-05-25 20:01:04.000000 pygentic-0.2.2/app/services/llm_service.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      135 2024-05-25 18:25:15.000000 pygentic-0.2.2/app/services/open_interpreter_service.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      119 2024-05-25 18:25:15.000000 pygentic-0.2.2/app/services/serverless_service.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 21:13:35.648582 pygentic-0.2.2/pygentic.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     6470 2024-05-25 21:13:35.000000 pygentic-0.2.2/pygentic.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2024-05-25 21:13:35.000000 pygentic-0.2.2/pygentic.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-25 21:13:35.000000 pygentic-0.2.2/pygentic.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2024-05-25 21:13:35.000000 pygentic-0.2.2/pygentic.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       89 2024-05-25 21:13:35.000000 pygentic-0.2.2/pygentic.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-05-25 21:13:35.000000 pygentic-0.2.2/pygentic.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-25 21:13:35.652582 pygentic-0.2.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1458 2024-05-25 21:13:32.000000 pygentic-0.2.2/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 21:13:35.648582 pygentic-0.2.2/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.2/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      442 2024-05-25 20:01:04.000000 pygentic-0.2.2/tests/test_assistants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      449 2024-05-25 20:01:04.000000 pygentic-0.2.2/tests/test_messages.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      530 2024-05-25 20:01:04.000000 pygentic-0.2.2/tests/test_runs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      411 2024-05-25 20:01:04.000000 pygentic-0.2.2/tests/test_threads.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-27 15:04:16.544856 pygentic-0.2.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-05-25 18:24:15.000000 pygentic-0.2.3/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     6448 2024-05-27 15:04:16.544856 pygentic-0.2.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5390 2024-05-25 19:24:32.000000 pygentic-0.2.3/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-27 15:04:16.528856 pygentic-0.2.3/app/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      202 2024-05-27 13:53:23.000000 pygentic-0.2.3/app/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1861 2024-05-27 13:55:08.000000 pygentic-0.2.3/app/main.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1157 2024-05-25 20:01:04.000000 pygentic-0.2.3/app/models.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-27 15:04:16.536856 pygentic-0.2.3/app/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.3/app/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      605 2024-05-25 20:01:04.000000 pygentic-0.2.3/app/routes/assistants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      550 2024-05-25 20:01:04.000000 pygentic-0.2.3/app/routes/messages.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      539 2024-05-25 20:01:04.000000 pygentic-0.2.3/app/routes/runs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      536 2024-05-25 20:01:04.000000 pygentic-0.2.3/app/routes/threads.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-27 15:04:16.540856 pygentic-0.2.3/app/services/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.3/app/services/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      794 2024-05-27 13:50:57.000000 pygentic-0.2.3/app/services/connector.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      220 2024-05-27 13:53:35.000000 pygentic-0.2.3/app/services/database.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1799 2024-05-25 20:01:04.000000 pygentic-0.2.3/app/services/llm_service.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      488 2024-05-27 13:39:26.000000 pygentic-0.2.3/app/services/open_interpreter_service.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      119 2024-05-25 18:25:15.000000 pygentic-0.2.3/app/services/serverless_service.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-27 15:04:16.544856 pygentic-0.2.3/pygentic.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     6448 2024-05-27 15:04:16.000000 pygentic-0.2.3/pygentic.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      661 2024-05-27 15:04:16.000000 pygentic-0.2.3/pygentic.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-27 15:04:16.000000 pygentic-0.2.3/pygentic.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2024-05-27 15:04:16.000000 pygentic-0.2.3/pygentic.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      100 2024-05-27 15:04:16.000000 pygentic-0.2.3/pygentic.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-05-27 15:04:16.000000 pygentic-0.2.3/pygentic.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-27 15:04:16.544856 pygentic-0.2.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1468 2024-05-27 15:04:12.000000 pygentic-0.2.3/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-27 15:04:16.544856 pygentic-0.2.3/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.3/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      442 2024-05-25 20:01:04.000000 pygentic-0.2.3/tests/test_assistants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      449 2024-05-25 20:01:04.000000 pygentic-0.2.3/tests/test_messages.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      530 2024-05-25 20:01:04.000000 pygentic-0.2.3/tests/test_runs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      411 2024-05-25 20:01:04.000000 pygentic-0.2.3/tests/test_threads.py
```

### Comparing `pygentic-0.2.2/LICENSE` & `pygentic-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.2/PKG-INFO` & `pygentic-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pygentic
-Version: 0.2.2
+Version: 0.2.3
 Summary: An innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API.
 Home-page: https://github.com/ruvnet/pygentic
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi
@@ -22,14 +21,15 @@
 Requires-Dist: httpx
 Requires-Dist: uvicorn
 Requires-Dist: liteLLM
 Requires-Dist: pydbantic
 Requires-Dist: databases[sqlite]
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
+Requires-Dist: sqlalchemy
 
 ```
    ___                      _   _      
   / _ \/\_/\__ _  ___ _ __ | |_(_) ___ 
  / /_)/\_ _/ _` |/ _ \ '_ \| __| |/ __|
 / ___/  / \ (_| |  __/ | | | |_| | (__ 
 \/      \_/\__, |\___|_| |_|\__|_|\___|
```

### Comparing `pygentic-0.2.2/README.md` & `pygentic-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.2/app/models.py` & `pygentic-0.2.3/app/models.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.2/app/routes/assistants.py` & `pygentic-0.2.3/app/routes/assistants.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.2/app/routes/messages.py` & `pygentic-0.2.3/app/routes/messages.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.2/app/routes/runs.py` & `pygentic-0.2.3/app/routes/runs.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.2/app/routes/threads.py` & `pygentic-0.2.3/app/routes/threads.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.2/app/services/llm_service.py` & `pygentic-0.2.3/app/services/llm_service.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.2/pygentic.egg-info/PKG-INFO` & `pygentic-0.2.3/pygentic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pygentic
-Version: 0.2.2
+Version: 0.2.3
 Summary: An innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API.
 Home-page: https://github.com/ruvnet/pygentic
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi
@@ -22,14 +21,15 @@
 Requires-Dist: httpx
 Requires-Dist: uvicorn
 Requires-Dist: liteLLM
 Requires-Dist: pydbantic
 Requires-Dist: databases[sqlite]
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
+Requires-Dist: sqlalchemy
 
 ```
    ___                      _   _      
   / _ \/\_/\__ _  ___ _ __ | |_(_) ___ 
  / /_)/\_ _/ _` |/ _ \ '_ \| __| |/ __|
 / ___/  / \ (_| |  __/ | | | |_| | (__ 
 \/      \_/\__, |\___|_| |_|\__|_|\___|
```

### Comparing `pygentic-0.2.2/pygentic.egg-info/SOURCES.txt` & `pygentic-0.2.3/pygentic.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 app/models.py
 app/routes/__init__.py
 app/routes/assistants.py
 app/routes/messages.py
 app/routes/runs.py
 app/routes/threads.py
 app/services/__init__.py
+app/services/connector.py
 app/services/database.py
 app/services/llm_service.py
 app/services/open_interpreter_service.py
 app/services/serverless_service.py
 pygentic.egg-info/PKG-INFO
 pygentic.egg-info/SOURCES.txt
 pygentic.egg-info/dependency_links.txt
```

### Comparing `pygentic-0.2.2/setup.py` & `pygentic-0.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pygentic",
-    version="0.2.2",
+    version="0.2.3",
     packages=find_packages(),
     install_requires=[
         "fastapi",
         "pydantic",
         "httpx",
         "uvicorn",
         "liteLLM",
         "pydbantic",
         "databases[sqlite]",
         "pytest",
         "pytest-asyncio",
+        "sqlalchemy",  # Add any other dependencies here
     ],
     entry_points={
         "console_scripts": ["pygentic=app.main:run"],
     },
     author="Your Name",
     author_email="your-email@example.com",
     description="An innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API.",
@@ -31,14 +32,13 @@
     url="https://github.com/ruvnet/pygentic",
     license="Apache License 2.0",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
 )
```

### Comparing `pygentic-0.2.2/tests/test_runs.py` & `pygentic-0.2.3/tests/test_runs.py`

 * *Files identical despite different names*

