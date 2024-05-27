# Comparing `tmp/organization_profile_local-0.0.6.tar.gz` & `tmp/organization_profile_local-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "organization_profile_local-0.0.6.tar", last modified: Tue May 21 21:13:55 2024, max compression
+gzip compressed data, was "organization_profile_local-0.0.7.tar", last modified: Mon May 27 07:30:30 2024, max compression
```

## Comparing `organization_profile_local-0.0.6.tar` & `organization_profile_local-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:13:55.580982 organization_profile_local-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-21 21:13:55.580982 organization_profile_local-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 21:13:30.000000 organization_profile_local-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:13:55.576982 organization_profile_local-0.0.6/organization_profile_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:13:55.580982 organization_profile_local-0.0.6/organization_profile_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:13:30.000000 organization_profile_local-0.0.6/organization_profile_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-21 21:13:30.000000 organization_profile_local-0.0.6/organization_profile_local/src/organization_profile_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-05-21 21:13:30.000000 organization_profile_local-0.0.6/organization_profile_local/src/organization_profiles_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:13:55.580982 organization_profile_local-0.0.6/organization_profile_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-21 21:13:55.000000 organization_profile_local-0.0.6/organization_profile_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-21 21:13:55.000000 organization_profile_local-0.0.6/organization_profile_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:13:55.000000 organization_profile_local-0.0.6/organization_profile_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 21:13:55.000000 organization_profile_local-0.0.6/organization_profile_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 21:13:55.000000 organization_profile_local-0.0.6/organization_profile_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-21 21:13:30.000000 organization_profile_local-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 21:13:55.580982 organization_profile_local-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-21 21:13:30.000000 organization_profile_local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:30:30.228272 organization_profile_local-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-27 07:30:30.228272 organization_profile_local-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 07:30:00.000000 organization_profile_local-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:30:30.224272 organization_profile_local-0.0.7/organization_profile_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:30:30.224272 organization_profile_local-0.0.7/organization_profile_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:30:00.000000 organization_profile_local-0.0.7/organization_profile_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-27 07:30:00.000000 organization_profile_local-0.0.7/organization_profile_local/src/organization_profile_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-05-27 07:30:00.000000 organization_profile_local-0.0.7/organization_profile_local/src/organization_profiles_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:30:30.224272 organization_profile_local-0.0.7/organization_profile_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-27 07:30:30.000000 organization_profile_local-0.0.7/organization_profile_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-27 07:30:30.000000 organization_profile_local-0.0.7/organization_profile_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:30:30.000000 organization_profile_local-0.0.7/organization_profile_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-27 07:30:30.000000 organization_profile_local-0.0.7/organization_profile_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 07:30:30.000000 organization_profile_local-0.0.7/organization_profile_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-27 07:30:06.000000 organization_profile_local-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:30:30.228272 organization_profile_local-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-27 07:30:00.000000 organization_profile_local-0.0.7/setup.py
```

### Comparing `organization_profile_local-0.0.6/PKG-INFO` & `organization_profile_local-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: organization-profile-local
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyPI Package for Circles organization-profile-local Python
 Home-page: https://github.com/circles-zone/organization-profile-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `organization_profile_local-0.0.6/organization_profile_local/src/organization_profile_constants.py` & `organization_profile_local-0.0.7/organization_profile_local/src/organization_profile_constants.py`

 * *Files identical despite different names*

### Comparing `organization_profile_local-0.0.6/organization_profile_local/src/organization_profiles_local.py` & `organization_profile_local-0.0.7/organization_profile_local/src/organization_profiles_local.py`

 * *Files identical despite different names*

### Comparing `organization_profile_local-0.0.6/organization_profile_local.egg-info/PKG-INFO` & `organization_profile_local-0.0.7/organization_profile_local.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: organization-profile-local
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyPI Package for Circles organization-profile-local Python
 Home-page: https://github.com/circles-zone/organization-profile-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `organization_profile_local-0.0.6/setup.py` & `organization_profile_local-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "organization-profile-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.6',  # update only the minor version each time # https://pypi.org/project/organization-profile-local/
+    version='0.0.7',  # update only the minor version each time # https://pypi.org/project/organization-profile-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles organization-profile-local Python",
     long_description="PyPI Package for Circles organization-profile-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/organization-profile-local-python-package",
     packages=[package_dir],
```

