# Comparing `tmp/ivylantern-0.1.0.tar.gz` & `tmp/ivylantern-0.1.3.tar.gz`

## Comparing `ivylantern-0.1.0.tar` & `ivylantern-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ivylantern-0.1.0/Makefile
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ivylantern-0.1.0/ivylantern.code-workspace
--rwxr-xr-x   0        0        0     1098 2020-02-02 00:00:00.000000 ivylantern-0.1.0/make_txtar.sh
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ivylantern-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ivylantern-0.1.0/requirements.lock
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ivylantern-0.1.0/src/ivylantern/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ivylantern-0.1.0/src/ivylantern/__main__.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ivylantern-0.1.0/src/ivylantern/ivylantern.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ivylantern-0.1.0/README.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 ivylantern-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 ivylantern-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ivylantern-0.1.3/.bumpversion.cfg
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ivylantern-0.1.3/Makefile
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ivylantern-0.1.3/ivylantern.code-workspace
+-rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 ivylantern-0.1.3/make_txtar.sh
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 ivylantern-0.1.3/requirements-dev.lock
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ivylantern-0.1.3/requirements.lock
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 ivylantern-0.1.3/src/ivylantern/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ivylantern-0.1.3/src/ivylantern/__main__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ivylantern-0.1.3/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ivylantern-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 ivylantern-0.1.3/PKG-INFO
```

### Comparing `ivylantern-0.1.0/make_txtar.sh` & `ivylantern-0.1.3/make_txtar.sh`

 * *Files 10% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 fi
 
 declare -a files=(
 	# Makefile # loc: 3
 	# README.md # loc: 5
 	# ivylantern.code-workspace # loc: 8
 	# make_txtar.sh # loc: 50
-	pyproject.toml # loc: 32
-	requirements-dev.lock # loc: 26
-	requirements.lock # loc: 11
-	src/ivylantern/__init__.py # loc: 8
-	src/ivylantern/__main__.py # loc: 5
-	src/ivylantern/ivylantern.py # loc: 48
+	# pyproject.toml # loc: 34
+	# requirements-dev.lock # loc: 83
+	# requirements.lock # loc: 11
+	src/ivylantern/__init__.py # loc: 37
+	# src/ivylantern/__main__.py # loc: 5
+	src/ivylantern/main.py # loc: 21
 	
 )
 for file in "${files[@]}"; do
     echo $file
 done | tee $tmp/filelist.txt
 
 tar -cf $tmp/ivylantern.tar -T $tmp/filelist.txt
```

### Comparing `ivylantern-0.1.0/src/ivylantern/ivylantern.py` & `ivylantern-0.1.3/src/ivylantern/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import argparse
 import re
 
+__project_name__ = "ivylantern"
+
 
 def convert_duration(duration):
     seconds_per_unit = {
         "s": 1,
         "m": 60,
         "h": 3600,
         "d": 86400,
```

### Comparing `ivylantern-0.1.0/pyproject.toml` & `ivylantern-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ivylantern"
-version = "0.1.0"
+version = "0.1.3"
 description = "Add your description here"
 authors = [
     { name = "Taylor Monacelli", email = "taylormonacelli@gmail.com" }
 ]
 dependencies = []
 readme = "README.md"
 requires-python = ">= 3.8"
@@ -16,14 +16,16 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "black>=24.2.0",
+    "twine>=5.1.0",
+    "bump2version>=1.0.1",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/ivylantern"]
```

