# Comparing `tmp/ivylantern-0.1.4.tar.gz` & `tmp/ivylantern-0.2.0.tar.gz`

## Comparing `ivylantern-0.1.4.tar` & `ivylantern-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ivylantern-0.1.4/.bumpversion.cfg
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ivylantern-0.1.4/Makefile
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ivylantern-0.1.4/ivylantern.code-workspace
--rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 ivylantern-0.1.4/make_txtar.sh
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 ivylantern-0.1.4/requirements-dev.lock
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ivylantern-0.1.4/requirements.lock
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 ivylantern-0.1.4/src/ivylantern/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ivylantern-0.1.4/src/ivylantern/__main__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ivylantern-0.1.4/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ivylantern-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 ivylantern-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ivylantern-0.2.0/.bumpversion.cfg
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ivylantern-0.2.0/Makefile
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ivylantern-0.2.0/ivylantern.code-workspace
+-rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 ivylantern-0.2.0/make_txtar.sh
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 ivylantern-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ivylantern-0.2.0/requirements.lock
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 ivylantern-0.2.0/src/ivylantern/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ivylantern-0.2.0/src/ivylantern/__main__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ivylantern-0.2.0/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ivylantern-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 ivylantern-0.2.0/PKG-INFO
```

### Comparing `ivylantern-0.1.4/make_txtar.sh` & `ivylantern-0.2.0/make_txtar.sh`

 * *Files identical despite different names*

### Comparing `ivylantern-0.1.4/requirements-dev.lock` & `ivylantern-0.2.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `ivylantern-0.1.4/pyproject.toml` & `ivylantern-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ivylantern"
-version = "0.1.4"
+version = "0.2.0"
 description = "Add your description here"
 authors = [
     { name = "Taylor Monacelli", email = "taylormonacelli@gmail.com" }
 ]
 dependencies = []
 readme = "README.md"
 requires-python = ">= 3.8"
```

