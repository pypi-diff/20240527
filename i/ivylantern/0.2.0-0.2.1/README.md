# Comparing `tmp/ivylantern-0.2.0.tar.gz` & `tmp/ivylantern-0.2.1.tar.gz`

## Comparing `ivylantern-0.2.0.tar` & `ivylantern-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ivylantern-0.2.0/.bumpversion.cfg
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ivylantern-0.2.0/Makefile
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ivylantern-0.2.0/ivylantern.code-workspace
--rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 ivylantern-0.2.0/make_txtar.sh
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 ivylantern-0.2.0/requirements-dev.lock
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ivylantern-0.2.0/requirements.lock
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 ivylantern-0.2.0/src/ivylantern/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ivylantern-0.2.0/src/ivylantern/__main__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ivylantern-0.2.0/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ivylantern-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 ivylantern-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ivylantern-0.2.1/.bumpversion.cfg
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ivylantern-0.2.1/Makefile
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ivylantern-0.2.1/ivylantern.code-workspace
+-rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 ivylantern-0.2.1/make_txtar.sh
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 ivylantern-0.2.1/requirements-dev.lock
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ivylantern-0.2.1/requirements.lock
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ivylantern-0.2.1/src/ivylantern/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ivylantern-0.2.1/src/ivylantern/__main__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ivylantern-0.2.1/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ivylantern-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 ivylantern-0.2.1/PKG-INFO
```

### Comparing `ivylantern-0.2.0/make_txtar.sh` & `ivylantern-0.2.1/make_txtar.sh`

 * *Files identical despite different names*

### Comparing `ivylantern-0.2.0/requirements-dev.lock` & `ivylantern-0.2.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `ivylantern-0.2.0/src/ivylantern/__init__.py` & `ivylantern-0.2.1/src/ivylantern/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import argparse
 import re
 
 __project_name__ = "ivylantern"
 
 SECONDS_PER_YEAR = int(365.2425 * 24 * 60 * 60)
 SECONDS_PER_MONTH = int(SECONDS_PER_YEAR / 12)
+SECONDS_PER_WEEK = 7 * 24 * 60 * 60
 SECONDS_PER_DAY = 24 * 60 * 60
 SECONDS_PER_HOUR = 60 * 60
 SECONDS_PER_MINUTE = 60
 SECONDS_PER_SECOND = 1
 
 
 def seconds_to_friendly_duration(total_seconds):
     units = [
         (SECONDS_PER_YEAR, "y"),
         (SECONDS_PER_MONTH, "M"),
+        (SECONDS_PER_WEEK, "w"),
         (SECONDS_PER_DAY, "d"),
         (SECONDS_PER_HOUR, "h"),
         (SECONDS_PER_MINUTE, "m"),
         (SECONDS_PER_SECOND, "s"),
     ]
 
     if total_seconds == 0:
@@ -36,15 +38,15 @@
 
 def friendly_duration_to_seconds(duration):
     seconds_per_unit = {
         "s": SECONDS_PER_SECOND,
         "m": SECONDS_PER_MINUTE,
         "h": SECONDS_PER_HOUR,
         "d": SECONDS_PER_DAY,
-        "w": 7 * SECONDS_PER_DAY,
+        "w": SECONDS_PER_WEEK,
         "M": SECONDS_PER_MONTH,
         "y": SECONDS_PER_YEAR,
     }
 
     pattern = re.compile(r"(\d*\.?\d+)([smhdwMy])")
     matches = pattern.findall(duration)
     if not matches:
```

### Comparing `ivylantern-0.2.0/pyproject.toml` & `ivylantern-0.2.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ivylantern"
-version = "0.2.0"
+version = "0.2.1"
 description = "Add your description here"
 authors = [
     { name = "Taylor Monacelli", email = "taylormonacelli@gmail.com" }
 ]
 dependencies = []
 readme = "README.md"
 requires-python = ">= 3.8"
```

