# Comparing `tmp/agentcrew-0.0.1.tar.gz` & `tmp/agentcrew-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentcrew-0.0.1.tar", last modified: Mon May 27 18:10:55 2024, max compression
+gzip compressed data, was "agentcrew-0.0.1a1.tar", last modified: Mon May 27 18:27:19 2024, max compression
```

## Comparing `agentcrew-0.0.1.tar` & `agentcrew-0.0.1a1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2024-05-27 18:10:55.671596 agentcrew-0.0.1/
--rw-r--r--   0 justin     (501) staff       (20)    11350 2024-05-26 00:55:50.000000 agentcrew-0.0.1/LICENSE
--rw-r--r--   0 justin     (501) staff       (20)     1506 2024-05-27 18:10:55.671527 agentcrew-0.0.1/PKG-INFO
--rw-r--r--   0 justin     (501) staff       (20)       68 2024-05-27 18:10:31.000000 agentcrew-0.0.1/README.md
--rw-r--r--   0 justin     (501) staff       (20)     1945 2024-05-27 18:10:31.000000 agentcrew-0.0.1/pyproject.toml
--rw-r--r--   0 justin     (501) staff       (20)      932 2024-05-27 18:10:55.671891 agentcrew-0.0.1/setup.cfg
--rw-r--r--   0 justin     (501) staff       (20)     1591 2024-05-27 18:10:32.000000 agentcrew-0.0.1/setup.py
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2024-05-27 18:10:55.668416 agentcrew-0.0.1/src/
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2024-05-27 18:10:55.669735 agentcrew-0.0.1/src/agentcrew/
--rw-r--r--   0 justin     (501) staff       (20)      576 2024-04-20 03:16:10.000000 agentcrew-0.0.1/src/agentcrew/__init__.py
--rw-r--r--   0 justin     (501) staff       (20)       38 2024-05-26 01:24:35.000000 agentcrew-0.0.1/src/agentcrew/cli.py
--rw-r--r--   0 justin     (501) staff       (20)        0 2024-05-26 01:11:13.000000 agentcrew-0.0.1/src/agentcrew/controller.py
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2024-05-27 18:10:55.670886 agentcrew-0.0.1/src/agentcrew.egg-info/
--rw-r--r--   0 justin     (501) staff       (20)     1506 2024-05-27 18:10:55.000000 agentcrew-0.0.1/src/agentcrew.egg-info/PKG-INFO
--rw-r--r--   0 justin     (501) staff       (20)      386 2024-05-27 18:10:55.000000 agentcrew-0.0.1/src/agentcrew.egg-info/SOURCES.txt
--rw-r--r--   0 justin     (501) staff       (20)        1 2024-05-27 18:10:55.000000 agentcrew-0.0.1/src/agentcrew.egg-info/dependency_links.txt
--rw-r--r--   0 justin     (501) staff       (20)       43 2024-05-27 18:10:55.000000 agentcrew-0.0.1/src/agentcrew.egg-info/entry_points.txt
--rw-r--r--   0 justin     (501) staff       (20)        1 2024-05-27 18:10:55.000000 agentcrew-0.0.1/src/agentcrew.egg-info/not-zip-safe
--rw-r--r--   0 justin     (501) staff       (20)      267 2024-05-27 18:10:55.000000 agentcrew-0.0.1/src/agentcrew.egg-info/requires.txt
--rw-r--r--   0 justin     (501) staff       (20)       10 2024-05-27 18:10:55.000000 agentcrew-0.0.1/src/agentcrew.egg-info/top_level.txt
+drwxr-xr-x   0 justin     (501) staff       (20)        0 2024-05-27 18:27:19.536643 agentcrew-0.0.1a1/
+-rw-r--r--   0 justin     (501) staff       (20)    11350 2024-05-26 00:55:50.000000 agentcrew-0.0.1a1/LICENSE
+-rw-r--r--   0 justin     (501) staff       (20)     1508 2024-05-27 18:27:19.536546 agentcrew-0.0.1a1/PKG-INFO
+-rw-r--r--   0 justin     (501) staff       (20)       68 2024-05-27 18:13:43.000000 agentcrew-0.0.1a1/README.md
+-rw-r--r--   0 justin     (501) staff       (20)     1945 2024-05-27 18:10:31.000000 agentcrew-0.0.1a1/pyproject.toml
+-rw-r--r--   0 justin     (501) staff       (20)      932 2024-05-27 18:27:19.536986 agentcrew-0.0.1a1/setup.cfg
+-rw-r--r--   0 justin     (501) staff       (20)     1593 2024-05-27 18:26:29.000000 agentcrew-0.0.1a1/setup.py
+drwxr-xr-x   0 justin     (501) staff       (20)        0 2024-05-27 18:27:19.533468 agentcrew-0.0.1a1/src/
+drwxr-xr-x   0 justin     (501) staff       (20)        0 2024-05-27 18:27:19.534479 agentcrew-0.0.1a1/src/agentcrew/
+-rw-r--r--   0 justin     (501) staff       (20)      576 2024-04-20 03:16:10.000000 agentcrew-0.0.1a1/src/agentcrew/__init__.py
+-rw-r--r--   0 justin     (501) staff       (20)       38 2024-05-26 01:24:35.000000 agentcrew-0.0.1a1/src/agentcrew/cli.py
+-rw-r--r--   0 justin     (501) staff       (20)        0 2024-05-26 01:11:13.000000 agentcrew-0.0.1a1/src/agentcrew/commander.py
+drwxr-xr-x   0 justin     (501) staff       (20)        0 2024-05-27 18:27:19.535880 agentcrew-0.0.1a1/src/agentcrew.egg-info/
+-rw-r--r--   0 justin     (501) staff       (20)     1508 2024-05-27 18:27:19.000000 agentcrew-0.0.1a1/src/agentcrew.egg-info/PKG-INFO
+-rw-r--r--   0 justin     (501) staff       (20)      385 2024-05-27 18:27:19.000000 agentcrew-0.0.1a1/src/agentcrew.egg-info/SOURCES.txt
+-rw-r--r--   0 justin     (501) staff       (20)        1 2024-05-27 18:27:19.000000 agentcrew-0.0.1a1/src/agentcrew.egg-info/dependency_links.txt
+-rw-r--r--   0 justin     (501) staff       (20)       43 2024-05-27 18:27:19.000000 agentcrew-0.0.1a1/src/agentcrew.egg-info/entry_points.txt
+-rw-r--r--   0 justin     (501) staff       (20)        1 2024-05-27 18:10:55.000000 agentcrew-0.0.1a1/src/agentcrew.egg-info/not-zip-safe
+-rw-r--r--   0 justin     (501) staff       (20)      267 2024-05-27 18:27:19.000000 agentcrew-0.0.1a1/src/agentcrew.egg-info/requires.txt
+-rw-r--r--   0 justin     (501) staff       (20)       10 2024-05-27 18:27:19.000000 agentcrew-0.0.1a1/src/agentcrew.egg-info/top_level.txt
```

### Comparing `agentcrew-0.0.1/LICENSE` & `agentcrew-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentcrew-0.0.1/PKG-INFO` & `agentcrew-0.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentcrew
-Version: 0.0.1
+Version: 0.0.1a1
 Author: 
 Author-email: 
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
@@ -39,10 +39,10 @@
 Requires-Dist: mkdocstrings[python]; extra == "docs"
 Provides-Extra: dev-all
 Requires-Dist: lab[dev,docs]; extra == "dev-all"
 Provides-Extra: db
 Requires-Dist: supabase; extra == "db"
 Requires-Dist: vecs; extra == "db"
 
-# agentcrew
+# AgentCrew
 
 Llama agents with LangChain and other open source tools
```

### Comparing `agentcrew-0.0.1/pyproject.toml` & `agentcrew-0.0.1a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `agentcrew-0.0.1/setup.cfg` & `agentcrew-0.0.1a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `agentcrew-0.0.1/setup.py` & `agentcrew-0.0.1a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 rootdir = Path(__file__).parent
 long_description = (rootdir / "README.md").read_text()
 
 package_name = "agentcrew"
 
 setup(
     name=package_name,
-    version="0.0.1",
+    version="0.0.1a1",
     package_dir={"": "src"},
     packages=find_packages(where="src", include=[package_name, f"{package_name}.*"]),
     include_package_data=True,
     setup_requires=["wheel"],
     zip_safe=False,
     description="",
     long_description=long_description,
```

### Comparing `agentcrew-0.0.1/src/agentcrew/__init__.py` & `agentcrew-0.0.1a1/src/agentcrew/__init__.py`

 * *Files identical despite different names*

### Comparing `agentcrew-0.0.1/src/agentcrew.egg-info/PKG-INFO` & `agentcrew-0.0.1a1/src/agentcrew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentcrew
-Version: 0.0.1
+Version: 0.0.1a1
 Author: 
 Author-email: 
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
@@ -39,10 +39,10 @@
 Requires-Dist: mkdocstrings[python]; extra == "docs"
 Provides-Extra: dev-all
 Requires-Dist: lab[dev,docs]; extra == "dev-all"
 Provides-Extra: db
 Requires-Dist: supabase; extra == "db"
 Requires-Dist: vecs; extra == "db"
 
-# agentcrew
+# AgentCrew
 
 Llama agents with LangChain and other open source tools
```

