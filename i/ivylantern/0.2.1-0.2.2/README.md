# Comparing `tmp/ivylantern-0.2.1.tar.gz` & `tmp/ivylantern-0.2.2.tar.gz`

## Comparing `ivylantern-0.2.1.tar` & `ivylantern-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ivylantern-0.2.1/.bumpversion.cfg
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ivylantern-0.2.1/Makefile
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ivylantern-0.2.1/ivylantern.code-workspace
--rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 ivylantern-0.2.1/make_txtar.sh
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 ivylantern-0.2.1/requirements-dev.lock
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ivylantern-0.2.1/requirements.lock
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ivylantern-0.2.1/src/ivylantern/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ivylantern-0.2.1/src/ivylantern/__main__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ivylantern-0.2.1/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ivylantern-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 ivylantern-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ivylantern-0.2.2/.bumpversion.cfg
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ivylantern-0.2.2/Makefile
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ivylantern-0.2.2/ivylantern.code-workspace
+-rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 ivylantern-0.2.2/make_txtar.sh
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 ivylantern-0.2.2/requirements-dev.lock
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ivylantern-0.2.2/requirements.lock
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 ivylantern-0.2.2/src/ivylantern/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ivylantern-0.2.2/src/ivylantern/__main__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ivylantern-0.2.2/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ivylantern-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 ivylantern-0.2.2/PKG-INFO
```

### Comparing `ivylantern-0.2.1/make_txtar.sh` & `ivylantern-0.2.2/make_txtar.sh`

 * *Files identical despite different names*

### Comparing `ivylantern-0.2.1/requirements-dev.lock` & `ivylantern-0.2.2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `ivylantern-0.2.1/src/ivylantern/__init__.py` & `ivylantern-0.2.2/src/ivylantern/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import argparse
 import re
 
 __project_name__ = "ivylantern"
 
-SECONDS_PER_YEAR = int(365.2425 * 24 * 60 * 60)
-SECONDS_PER_MONTH = int(SECONDS_PER_YEAR / 12)
-SECONDS_PER_WEEK = 7 * 24 * 60 * 60
-SECONDS_PER_DAY = 24 * 60 * 60
-SECONDS_PER_HOUR = 60 * 60
-SECONDS_PER_MINUTE = 60
 SECONDS_PER_SECOND = 1
+SECONDS_PER_MINUTE = 60 * SECONDS_PER_SECOND
+SECONDS_PER_HOUR = 60 * SECONDS_PER_MINUTE
+SECONDS_PER_DAY = 24 * SECONDS_PER_HOUR
+SECONDS_PER_WEEK = 7 * SECONDS_PER_DAY
+SECONDS_PER_MONTH = int(365.2425 * SECONDS_PER_DAY / 12)
+SECONDS_PER_YEAR = int(365.2425 * SECONDS_PER_DAY)
 
 
 def seconds_to_friendly_duration(total_seconds):
     units = [
         (SECONDS_PER_YEAR, "y"),
         (SECONDS_PER_MONTH, "M"),
         (SECONDS_PER_WEEK, "w"),
```

### Comparing `ivylantern-0.2.1/pyproject.toml` & `ivylantern-0.2.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ivylantern"
-version = "0.2.1"
+version = "0.2.2"
 description = "Add your description here"
 authors = [
     { name = "Taylor Monacelli", email = "taylormonacelli@gmail.com" }
 ]
 dependencies = []
 readme = "README.md"
 requires-python = ">= 3.8"
```

