# Comparing `tmp/medjc09_hub_python-0.1.1.tar.gz` & `tmp/medjc09_hub_python-0.2.0.tar.gz`

## Comparing `medjc09_hub_python-0.1.1.tar` & `medjc09_hub_python-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/.python-version
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/requirements-dev.lock
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/requirements.lock
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/.github/workflows/main.yml
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/src/medjc09_hub_python/__init__.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/src/medjc09_hub_python/command.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/src/medjc09_hub_python/medjc09_hub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/tests/test_command_deserializer.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/tests/test_command_serializer.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/tests/test_medjc09_hub.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/LICENSE
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/README.md
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 medjc09_hub_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/.python-version
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/requirements.lock
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/src/medjc09_hub_python/__init__.py
+-rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/src/medjc09_hub_python/command.py
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/src/medjc09_hub_python/medjc09_hub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/tests/test_command_deserializer.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/tests/test_command_serializer.py
+-rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/tests/test_medjc09_hub.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/LICENSE
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/README.md
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/PKG-INFO
```

### Comparing `medjc09_hub_python-0.1.1/requirements-dev.lock` & `medjc09_hub_python-0.2.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `medjc09_hub_python-0.1.1/.github/workflows/main.yml` & `medjc09_hub_python-0.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `medjc09_hub_python-0.1.1/.github/workflows/publish.yml` & `medjc09_hub_python-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `medjc09_hub_python-0.1.1/LICENSE` & `medjc09_hub_python-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medjc09_hub_python-0.1.1/pyproject.toml` & `medjc09_hub_python-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "medjc09-hub-python"
-version = "0.1.1"
+version = "0.2.0"
 description = "Python library for medjc09 hub"
 authors = [
     { name = "OctSquid", email = "pqvs6k96@s.okayama-u.ac.jp" }
 ]
 dependencies = [
     "cobs>=1.2.1",
     "pyserial-asyncio>=0.6",
```

