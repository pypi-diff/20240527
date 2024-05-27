# Comparing `tmp/dao_scripts-1.3.0.post1.tar.gz` & `tmp/dao_scripts-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao_scripts-1.3.0.post1.tar", last modified: Fri May 24 16:20:50 2024, max compression
+gzip compressed data, was "dao_scripts-1.3.1.tar", last modified: Mon May 27 09:00:47 2024, max compression
```

## Comparing `dao_scripts-1.3.0.post1.tar` & `dao_scripts-1.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:50.744063 dao_scripts-1.3.0.post1/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:50.736063 dao_scripts-1.3.0.post1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:50.736063 dao_scripts-1.3.0.post1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/.github/workflows/update-datasets.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-24 16:20:50.744063 dao_scripts-1.3.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:50.744063 dao_scripts-1.3.0.post1/dao_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-24 16:20:50.000000 dao_scripts-1.3.0.post1/dao_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-24 16:20:50.000000 dao_scripts-1.3.0.post1/dao_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:20:50.000000 dao_scripts-1.3.0.post1/dao_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-24 16:20:50.000000 dao_scripts-1.3.0.post1/dao_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 16:20:50.000000 dao_scripts-1.3.0.post1/dao_scripts.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-24 16:20:50.000000 dao_scripts-1.3.0.post1/dao_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 16:20:50.000000 dao_scripts-1.3.0.post1/dao_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-24 16:20:50.744063 dao_scripts-1.3.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:50.740063 dao_scripts-1.3.0.post1/src/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-24 16:20:50.000000 dao_scripts-1.3.0.post1/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:50.740063 dao_scripts-1.3.0.post1/src/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/aragon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/aragon/dao_names.json
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/aragon/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:50.740063 dao_scripts-1.3.0.post1/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/common/api_requester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/common/blockscout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/common/cryptocompare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/common/thegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:50.744063 dao_scripts-1.3.0.post1/src/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/daohaus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/daohaus/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:50.744063 dao_scripts-1.3.0.post1/src/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/daostack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/daostack/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5665 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:50.744063 dao_scripts-1.3.0.post1/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/src/utils/uploadDataWarehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:50.744063 dao_scripts-1.3.0.post1/test/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 16:20:44.000000 dao_scripts-1.3.0.post1/test/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.595149 dao_scripts-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.599149 dao_scripts-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/.github/workflows/update-datasets.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/dao_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-27 09:00:47.607149 dao_scripts-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.599149 dao_scripts-1.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/src/aragon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/aragon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/aragon/dao_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/aragon/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/common/api_requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/common/blockscout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/common/cryptocompare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/common/thegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/src/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/daohaus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/daohaus/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/src/daostack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/daostack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/daostack/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5588 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/utils/uploadDataWarehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/test/test_placeholder.py
```

### Comparing `dao_scripts-1.3.0.post1/.github/workflows/ci.yml` & `dao_scripts-1.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/.github/workflows/update-datasets.yml` & `dao_scripts-1.3.1/.github/workflows/update-datasets.yml`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/.gitignore` & `dao_scripts-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/CHANGELOG.md` & `dao_scripts-1.3.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
-## 1.3.0 - 2024-04-24
+## 1.3.1 - 2024-05-27
+- Fixed bug with `--delete-force`
+
+## 1.3.0 - 2024-05-24
 - Improved and standarized logging #10
 - The Graph Hosted Service sunsetting
   - Added DAOA_THE_GRAPH_API_KEY variable (now needed)
 
 ## 1.2.2 - 2023-12-13
 - Changed daohaus names cache folder
```

### Comparing `dao_scripts-1.3.0.post1/LICENSE` & `dao_scripts-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/PKG-INFO` & `dao_scripts-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.3.0.post1
+Version: 1.3.1
 Summary: "A tool to download data to monitor DAO activity"
 Home-page: https://github.com/Grasia/dao-scripts
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-scripts
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-scripts/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.3.0.post1 Summary: "A tool
-to download data to monitor DAO activity" Home-page: https://github.com/Grasia/
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.3.1 Summary: "A tool to
+download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `dao_scripts-1.3.0.post1/README.md` & `dao_scripts-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/dao_scripts.egg-info/PKG-INFO` & `dao_scripts-1.3.1/dao_scripts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.3.0.post1
+Version: 1.3.1
 Summary: "A tool to download data to monitor DAO activity"
 Home-page: https://github.com/Grasia/dao-scripts
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-scripts
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-scripts/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.3.0.post1 Summary: "A tool
-to download data to monitor DAO activity" Home-page: https://github.com/Grasia/
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.3.1 Summary: "A tool to
+download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `dao_scripts-1.3.0.post1/dao_scripts.egg-info/SOURCES.txt` & `dao_scripts-1.3.1/dao_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/setup.cfg` & `dao_scripts-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/setup.py` & `dao_scripts-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/aragon/dao_names.json` & `dao_scripts-1.3.1/src/aragon/dao_names.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/aragon/runner.py` & `dao_scripts-1.3.1/src/aragon/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/argparser.py` & `dao_scripts-1.3.1/src/argparser.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/common/api_requester.py` & `dao_scripts-1.3.1/src/common/api_requester.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/common/blockscout.py` & `dao_scripts-1.3.1/src/common/blockscout.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/common/common.py` & `dao_scripts-1.3.1/src/common/common.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/common/cryptocompare.py` & `dao_scripts-1.3.1/src/common/cryptocompare.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/common/thegraph.py` & `dao_scripts-1.3.1/src/common/thegraph.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/config.py` & `dao_scripts-1.3.1/src/config.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/daohaus/runner.py` & `dao_scripts-1.3.1/src/daohaus/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/daostack/runner.py` & `dao_scripts-1.3.1/src/daostack/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/endpoints.json` & `dao_scripts-1.3.1/src/endpoints.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/logging.py` & `dao_scripts-1.3.1/src/logging.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/main.py` & `dao_scripts-1.3.1/src/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     if not versionfile.is_file():
         return False
 
     with open(versionfile, 'r') as vf:
         return vf.readline().strip() == __version__
 
 def run_all(
-    datawarehouse: Path, delete_force: bool, 
+    datawarehouse: Path,
     platforms: list[str], networks: list[str], collectors: list[str], 
     block_datetime: datetime, force: bool
 ):
 
     # The default config is every platform
     if not platforms:
         platforms = list(AVAILABLE_PLATFORMS.keys())
@@ -97,33 +97,32 @@
                 ignore = shutil.ignore_patterns('.lock*', 'logs/*')
 
                 # We want to copy the dw, so we open it as readers
                 p_lock.touch(exist_ok=True)
                 with pl.Lock(p_lock, 'r', timeout=1, flags=pl.LOCK_SH | pl.LOCK_NB):
                     shutil.copytree(datawarehouse, tmp_dw, dirs_exist_ok=True, ignore=ignore)
 
-                if args.delete_force or not _is_good_version(datawarehouse):
+                if args.delete_force or not _is_good_version(tmp_dw):
                     if not args.delete_force:
                         print(f"datawarehouse version is not version {__version__}, upgrading")
 
-                    # We skip the dotfiles like .lock
-                    for p in datawarehouse.glob('[!.]*'):
+                    # We skip the dotfiles like .lock or .cache
+                    for p in tmp_dw.glob('[!.]*'):
                         if p.is_dir():
                             shutil.rmtree(p)
                         else:
                             p.unlink()
 
                 setup_logging(tmp_dw, datawarehouse, config.DEBUG)
                 logger = logging.getLogger('dao_analyzer.main')
                 logger.info(">>> Running dao-scripts with arguments: %s", sys.orig_argv)
 
                 # Execute the scripts in the aux datawarehouse
                 run_all(
                     datawarehouse=tmp_dw,
-                    delete_force=args.delete_force,
                     platforms=args.platforms,
                     networks=args.networks,
                     collectors=args.collectors,
                     block_datetime=args.block_datetime,
                     force=args.force,
                 )
```

### Comparing `dao_scripts-1.3.0.post1/src/metadata.py` & `dao_scripts-1.3.1/src/metadata.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.0.post1/src/utils/uploadDataWarehouse.py` & `dao_scripts-1.3.1/src/utils/uploadDataWarehouse.py`

 * *Files identical despite different names*

