# Comparing `tmp/kal_utils-0.0.1.tar.gz` & `tmp/kal_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kal_utils-0.0.1.tar", last modified: Sun May 26 11:15:35 2024, max compression
+gzip compressed data, was "kal_utils-0.0.2.tar", last modified: Sun May 26 11:45:26 2024, max compression
```

## Comparing `kal_utils-0.0.1.tar` & `kal_utils-0.0.2.tar`

### file list

```diff
@@ -1,50 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:15:35.748783 kal_utils-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-26 11:15:25.000000 kal_utils-0.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:15:35.740783 kal_utils-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:15:35.740783 kal_utils-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-26 11:15:25.000000 kal_utils-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-26 11:15:25.000000 kal_utils-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-26 11:15:25.000000 kal_utils-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:15:35.744783 kal_utils-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-26 11:15:25.000000 kal_utils-0.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-26 11:15:25.000000 kal_utils-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-26 11:15:25.000000 kal_utils-0.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-26 11:15:25.000000 kal_utils-0.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-26 11:15:25.000000 kal_utils-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-26 11:15:25.000000 kal_utils-0.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-26 11:15:25.000000 kal_utils-0.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-26 11:15:25.000000 kal_utils-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-26 11:15:25.000000 kal_utils-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-26 11:15:25.000000 kal_utils-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-26 11:15:35.748783 kal_utils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-26 11:15:25.000000 kal_utils-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:15:35.744783 kal_utils-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-26 11:15:25.000000 kal_utils-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-26 11:15:25.000000 kal_utils-0.0.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:15:35.744783 kal_utils-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-26 11:15:25.000000 kal_utils-0.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-26 11:15:25.000000 kal_utils-0.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-26 11:15:25.000000 kal_utils-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-26 11:15:25.000000 kal_utils-0.0.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-26 11:15:25.000000 kal_utils-0.0.1/docs/kal_utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:15:35.744783 kal_utils-0.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-26 11:15:25.000000 kal_utils-0.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-26 11:15:25.000000 kal_utils-0.0.1/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:15:35.744783 kal_utils-0.0.1/kal_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-26 11:15:25.000000 kal_utils-0.0.1/kal_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 11:15:25.000000 kal_utils-0.0.1/kal_utils/kal_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:15:35.748783 kal_utils-0.0.1/kal_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-26 11:15:35.000000 kal_utils-0.0.1/kal_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-26 11:15:35.000000 kal_utils-0.0.1/kal_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:15:35.000000 kal_utils-0.0.1/kal_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 11:15:35.000000 kal_utils-0.0.1/kal_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-26 11:15:35.000000 kal_utils-0.0.1/kal_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 11:15:35.000000 kal_utils-0.0.1/kal_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-26 11:15:25.000000 kal_utils-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-26 11:15:25.000000 kal_utils-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 11:15:25.000000 kal_utils-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-26 11:15:25.000000 kal_utils-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:15:35.748783 kal_utils-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:15:35.748783 kal_utils-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-26 11:15:25.000000 kal_utils-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-26 11:15:25.000000 kal_utils-0.0.1/tests/test_kal_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:45:26.820320 kal_utils-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-26 11:45:17.000000 kal_utils-0.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:45:26.812319 kal_utils-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:45:26.812319 kal_utils-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-26 11:45:17.000000 kal_utils-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-26 11:45:17.000000 kal_utils-0.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-26 11:45:17.000000 kal_utils-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:45:26.816319 kal_utils-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-26 11:45:17.000000 kal_utils-0.0.2/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-26 11:45:17.000000 kal_utils-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-26 11:45:17.000000 kal_utils-0.0.2/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-26 11:45:17.000000 kal_utils-0.0.2/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-26 11:45:17.000000 kal_utils-0.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-26 11:45:17.000000 kal_utils-0.0.2/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-26 11:45:17.000000 kal_utils-0.0.2/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-26 11:45:17.000000 kal_utils-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-26 11:45:17.000000 kal_utils-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-26 11:45:17.000000 kal_utils-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-26 11:45:26.820320 kal_utils-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-26 11:45:17.000000 kal_utils-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:45:26.816319 kal_utils-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-26 11:45:17.000000 kal_utils-0.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-26 11:45:17.000000 kal_utils-0.0.2/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:45:26.816319 kal_utils-0.0.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-26 11:45:17.000000 kal_utils-0.0.2/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-26 11:45:17.000000 kal_utils-0.0.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-26 11:45:17.000000 kal_utils-0.0.2/docs/handle_response.md
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-26 11:45:17.000000 kal_utils-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-26 11:45:17.000000 kal_utils-0.0.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-26 11:45:17.000000 kal_utils-0.0.2/docs/kal_utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:45:17.000000 kal_utils-0.0.2/docs/logger.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:45:26.816319 kal_utils-0.0.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-26 11:45:17.000000 kal_utils-0.0.2/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-26 11:45:17.000000 kal_utils-0.0.2/docs/requests.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-26 11:45:17.000000 kal_utils-0.0.2/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:45:26.816319 kal_utils-0.0.2/kal_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-26 11:45:17.000000 kal_utils-0.0.2/kal_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-26 11:45:17.000000 kal_utils-0.0.2/kal_utils/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 11:45:17.000000 kal_utils-0.0.2/kal_utils/kal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-26 11:45:17.000000 kal_utils-0.0.2/kal_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-26 11:45:17.000000 kal_utils-0.0.2/kal_utils/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:45:26.820320 kal_utils-0.0.2/kal_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-26 11:45:26.000000 kal_utils-0.0.2/kal_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-26 11:45:26.000000 kal_utils-0.0.2/kal_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:45:26.000000 kal_utils-0.0.2/kal_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 11:45:26.000000 kal_utils-0.0.2/kal_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-26 11:45:26.000000 kal_utils-0.0.2/kal_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 11:45:26.000000 kal_utils-0.0.2/kal_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-26 11:45:17.000000 kal_utils-0.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-26 11:45:17.000000 kal_utils-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 11:45:17.000000 kal_utils-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-26 11:45:17.000000 kal_utils-0.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:45:26.820320 kal_utils-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:45:26.820320 kal_utils-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-26 11:45:17.000000 kal_utils-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-26 11:45:17.000000 kal_utils-0.0.2/tests/test_kal_utils.py
```

### Comparing `kal_utils-0.0.1/.github/workflows/docs-build.yml` & `kal_utils-0.0.2/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.1/.github/workflows/docs.yml` & `kal_utils-0.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.1/.github/workflows/installation.yml` & `kal_utils-0.0.2/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.1/.github/workflows/macos.yml` & `kal_utils-0.0.2/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.1/.github/workflows/pypi.yml` & `kal_utils-0.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.1/.github/workflows/ubuntu.yml` & `kal_utils-0.0.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.1/.github/workflows/windows.yml` & `kal_utils-0.0.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.1/.gitignore` & `kal_utils-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.1/LICENSE` & `kal_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.1/PKG-INFO` & `kal_utils-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kal-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Kaleidoo utils package
 Author-email: Bar Lander <barh@kaleidoo.ai>
 License: MIT License
 Project-URL: Homepage, https://github.com/BarLanderK/kal-utils
 Keywords: kal-utils
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kal_utils-0.0.1/docs/contributing.md` & `kal_utils-0.0.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.1/docs/installation.md` & `kal_utils-0.0.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.1/kal_utils.egg-info/PKG-INFO` & `kal_utils-0.0.2/kal_utils.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kal-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Kaleidoo utils package
 Author-email: Bar Lander <barh@kaleidoo.ai>
 License: MIT License
 Project-URL: Homepage, https://github.com/BarLanderK/kal-utils
 Keywords: kal-utils
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kal_utils-0.0.1/kal_utils.egg-info/SOURCES.txt` & `kal_utils-0.0.2/kal_utils.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -16,22 +16,28 @@
 .github/workflows/macos.yml
 .github/workflows/pypi.yml
 .github/workflows/ubuntu.yml
 .github/workflows/windows.yml
 docs/changelog.md
 docs/contributing.md
 docs/faq.md
+docs/handle_response.md
 docs/index.md
 docs/installation.md
 docs/kal_utils.md
+docs/logger.md
+docs/requests.md
 docs/usage.md
 docs/examples/intro.ipynb
 docs/overrides/main.html
 kal_utils/__init__.py
+kal_utils/handle_response.py
 kal_utils/kal_utils.py
+kal_utils/logger.py
+kal_utils/requests.py
 kal_utils.egg-info/PKG-INFO
 kal_utils.egg-info/SOURCES.txt
 kal_utils.egg-info/dependency_links.txt
 kal_utils.egg-info/entry_points.txt
 kal_utils.egg-info/requires.txt
 kal_utils.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `kal_utils-0.0.1/mkdocs.yml` & `kal_utils-0.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.1/pyproject.toml` & `kal_utils-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kal-utils"
-version = "0.0.1"
+version = "0.0.2"
 dynamic = [
     "dependencies",
 ]
 description = "Kaleidoo utils package"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
@@ -75,8 +75,8 @@
 
 
 [project.urls]
 Homepage = "https://github.com/BarLanderK/kal-utils"
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm>=8"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
```

