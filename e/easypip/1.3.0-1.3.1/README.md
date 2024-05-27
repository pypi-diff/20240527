# Comparing `tmp/easypip-1.3.0.tar.gz` & `tmp/easypip-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypip-1.3.0.tar", last modified: Fri Jun  2 13:59:36 2023, max compression
+gzip compressed data, was "easypip-1.3.1.tar", last modified: Mon May 27 09:59:52 2024, max compression
```

## Comparing `easypip-1.3.0.tar` & `easypip-1.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:36.240484 easypip-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:36.236484 easypip-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:36.236484 easypip-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 13:59:21.000000 easypip-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-02 13:59:21.000000 easypip-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-02 13:59:21.000000 easypip-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 13:59:36.240484 easypip-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-02 13:59:21.000000 easypip-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-02 13:59:21.000000 easypip-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-02 13:59:36.240484 easypip-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 13:59:21.000000 easypip-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:36.236484 easypip-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:36.240484 easypip-1.3.0/src/easypip/
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-02 13:59:21.000000 easypip-1.3.0/src/easypip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 13:59:36.000000 easypip-1.3.0/src/easypip/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-02 13:59:21.000000 easypip-1.3.0/src/easypip/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:36.240484 easypip-1.3.0/src/easypip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 13:59:36.000000 easypip-1.3.0/src/easypip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-02 13:59:36.000000 easypip-1.3.0/src/easypip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:59:36.000000 easypip-1.3.0/src/easypip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 13:59:36.000000 easypip-1.3.0/src/easypip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 13:59:36.000000 easypip-1.3.0/src/easypip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.162265 easypip-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.158265 easypip-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.158265 easypip-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-27 09:59:45.000000 easypip-1.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-27 09:59:45.000000 easypip-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-27 09:59:45.000000 easypip-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-27 09:59:52.162265 easypip-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 09:59:45.000000 easypip-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-27 09:59:45.000000 easypip-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-27 09:59:52.162265 easypip-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 09:59:45.000000 easypip-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.158265 easypip-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.158265 easypip-1.3.1/src/easypip/
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-05-27 09:59:45.000000 easypip-1.3.1/src/easypip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 09:59:52.000000 easypip-1.3.1/src/easypip/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-27 09:59:45.000000 easypip-1.3.1/src/easypip/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.162265 easypip-1.3.1/src/easypip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-27 09:59:52.000000 easypip-1.3.1/src/easypip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-27 09:59:52.000000 easypip-1.3.1/src/easypip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:59:52.000000 easypip-1.3.1/src/easypip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 09:59:52.000000 easypip-1.3.1/src/easypip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 09:59:52.000000 easypip-1.3.1/src/easypip.egg-info/top_level.txt
```

### Comparing `easypip-1.3.0/.github/workflows/python-publish.yml` & `easypip-1.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `easypip-1.3.0/.gitignore` & `easypip-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `easypip-1.3.0/.pre-commit-config.yaml` & `easypip-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easypip-1.3.0/pyproject.toml` & `easypip-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easypip-1.3.0/src/easypip/__init__.py` & `easypip-1.3.1/src/easypip/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,16 @@
                 Installer._packages[p["name"].lower()] = p
         return Installer._packages
 
     @staticmethod
     def has_requirement(requirement: Requirement):
         """Returns true if the requirement is fulfilled"""
         package = Installer.packages().get(requirement.project_name.lower(), None)
+        if package is None:
+            package = Installer.packages().get(requirement.unsafe_name.lower(), None)
 
         if package is None:
             return False
 
         for comparator, desired_version in requirement.specs:
             desired_version = parse_version(desired_version)
```

### Comparing `easypip-1.3.0/src/easypip/platform.py` & `easypip-1.3.1/src/easypip/platform.py`

 * *Files identical despite different names*

