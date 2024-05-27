# Comparing `tmp/conda_inject-1.3.1.tar.gz` & `tmp/conda_inject-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda_inject-1.3.1.tar", max compression
+gzip compressed data, was "conda_inject-1.3.2.tar", max compression
```

## Comparing `conda_inject-1.3.1.tar` & `conda_inject-1.3.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2023-11-29 20:15:18.106689 conda_inject-1.3.1/LICENSE
--rw-r--r--   0        0        0      197 2023-11-29 20:15:18.106689 conda_inject-1.3.1/README.md
--rw-r--r--   0        0        0     7032 2023-11-29 20:15:18.106689 conda_inject-1.3.1/conda_inject/__init__.py
--rw-r--r--   0        0        0      766 2023-11-29 20:15:18.106689 conda_inject-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 conda_inject-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-27 12:20:40.487090 conda_inject-1.3.2/LICENSE
+-rw-r--r--   0        0        0      197 2024-05-27 12:20:40.487090 conda_inject-1.3.2/README.md
+-rw-r--r--   0        0        0     7168 2024-05-27 12:20:40.487090 conda_inject-1.3.2/conda_inject/__init__.py
+-rw-r--r--   0        0        0      766 2024-05-27 12:20:40.487090 conda_inject-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 conda_inject-1.3.2/PKG-INFO
```

### Comparing `conda_inject-1.3.1/LICENSE` & `conda_inject-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_inject-1.3.1/conda_inject/__init__.py` & `conda_inject-1.3.2/conda_inject/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,14 +204,17 @@
 
 
 def _check_packages(packages, invalid_packages: Optional[Set[str]] = None):
     """Check if the given package specs are valid."""
     invalid_packages = {"python"} if invalid_packages is None else invalid_packages
 
     for package_spec in packages:
+        if not isinstance(package_spec, str):
+            # ignore e.g. dict rows (coming from combining with pip)
+            continue
         m = package_spec_pattern.match(package_spec)
         if m:
             package_name = m.group("package")
             if package_name in invalid_packages:
                 raise ValueError(
                     f"The list of packages contains {package_name}. "
                     "This is not allowed as conda-inject automatically "
```

### Comparing `conda_inject-1.3.1/pyproject.toml` & `conda_inject-1.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Johannes Köster <johannes.koester@uni-due.de>"]
 description = "Helper functions for injecting a conda environment into the current python environment (by modifying sys.path, without actually changing the current python environment)."
 name = "conda-inject"
 packages = [{include = "conda_inject"}]
 readme = "README.md"
-version = "1.3.1"
+version = "1.3.2"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyyaml = "^6.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
```

### Comparing `conda_inject-1.3.1/PKG-INFO` & `conda_inject-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-inject
-Version: 1.3.1
+Version: 1.3.2
 Summary: Helper functions for injecting a conda environment into the current python environment (by modifying sys.path, without actually changing the current python environment).
 Author: Johannes Köster
 Author-email: johannes.koester@uni-due.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

