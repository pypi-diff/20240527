# Comparing `tmp/mozilla_version-3.0.0.tar.gz` & `tmp/mozilla-version-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla_version-3.0.0.tar", last modified: Thu Apr 18 14:37:08 2024, max compression
+gzip compressed data, was "mozilla-version-3.1.0.tar", last modified: Mon May 27 17:08:37 2024, max compression
```

## Comparing `mozilla_version-3.0.0.tar` & `mozilla-version-3.1.0.tar`

### file list

```diff
@@ -1,45 +1,64 @@
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-18 14:37:08.034622 mozilla_version-3.0.0/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    15922 2022-06-29 08:41:37.000000 mozilla_version-3.0.0/LICENSE
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      139 2022-06-29 08:41:37.000000 mozilla_version-3.0.0/MANIFEST.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      478 2024-04-18 14:37:08.034408 mozilla_version-3.0.0/PKG-INFO
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7491 2022-11-25 16:16:39.000000 mozilla_version-3.0.0/README.md
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-18 14:37:08.030701 mozilla_version-3.0.0/mozilla_version/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      262 2023-05-23 08:14:29.000000 mozilla_version-3.0.0/mozilla_version/__init__.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     4961 2023-05-23 08:14:29.000000 mozilla_version-3.0.0/mozilla_version/balrog.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     2468 2023-05-23 08:14:29.000000 mozilla_version-3.0.0/mozilla_version/errors.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      199 2022-06-29 08:41:37.000000 mozilla_version-3.0.0/mozilla_version/fenix.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    28354 2024-04-18 14:35:19.000000 mozilla_version-3.0.0/mozilla_version/gecko.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1988 2023-05-23 08:14:29.000000 mozilla_version-3.0.0/mozilla_version/maven.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     9478 2024-04-18 09:45:05.000000 mozilla_version-3.0.0/mozilla_version/mobile.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1335 2023-05-23 08:14:29.000000 mozilla_version-3.0.0/mozilla_version/parser.py
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-18 14:37:08.032620 mozilla_version-3.0.0/mozilla_version/test/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       87 2022-06-29 08:41:37.000000 mozilla_version-3.0.0/mozilla_version/test/__init__.py
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-18 14:37:08.032852 mozilla_version-3.0.0/mozilla_version/test/integration/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      325 2024-04-18 14:35:19.000000 mozilla_version-3.0.0/mozilla_version/test/integration/__init__.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1407 2024-04-18 14:35:19.000000 mozilla_version-3.0.0/mozilla_version/test/integration/test_product_details.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7839 2022-06-29 08:41:37.000000 mozilla_version-3.0.0/mozilla_version/test/test_balrog.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      268 2023-05-23 08:14:29.000000 mozilla_version-3.0.0/mozilla_version/test/test_default_imports.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      933 2022-06-29 08:41:37.000000 mozilla_version-3.0.0/mozilla_version/test/test_errors.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      193 2022-07-07 15:15:03.000000 mozilla_version-3.0.0/mozilla_version/test/test_fenix.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    41895 2024-04-18 14:35:19.000000 mozilla_version-3.0.0/mozilla_version/test/test_gecko.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     3526 2023-05-23 08:14:29.000000 mozilla_version-3.0.0/mozilla_version/test/test_maven.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    11948 2024-04-17 17:25:36.000000 mozilla_version-3.0.0/mozilla_version/test/test_mobile.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7441 2022-06-29 08:41:37.000000 mozilla_version-3.0.0/mozilla_version/test/test_version.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    10049 2024-04-18 09:45:05.000000 mozilla_version-3.0.0/mozilla_version/version.py
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-18 14:37:08.034176 mozilla_version-3.0.0/mozilla_version.egg-info/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      478 2024-04-18 14:37:08.000000 mozilla_version-3.0.0/mozilla_version.egg-info/PKG-INFO
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1075 2024-04-18 14:37:08.000000 mozilla_version-3.0.0/mozilla_version.egg-info/SOURCES.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2024-04-18 14:37:08.000000 mozilla_version-3.0.0/mozilla_version.egg-info/dependency_links.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2024-04-18 12:53:03.000000 mozilla_version-3.0.0/mozilla_version.egg-info/not-zip-safe
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       12 2024-04-18 14:37:08.000000 mozilla_version-3.0.0/mozilla_version.egg-info/requires.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       16 2024-04-18 14:37:08.000000 mozilla_version-3.0.0/mozilla_version.egg-info/top_level.txt
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-18 14:37:08.033968 mozilla_version-3.0.0/requirements/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       12 2024-04-18 12:43:32.000000 mozilla_version-3.0.0/requirements/base.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      363 2024-04-18 14:35:19.000000 mozilla_version-3.0.0/requirements/base.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      204 2024-04-18 14:35:19.000000 mozilla_version-3.0.0/requirements/docs.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    17771 2024-04-18 14:35:19.000000 mozilla_version-3.0.0/requirements/docs.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       99 2024-04-18 14:35:19.000000 mozilla_version-3.0.0/requirements/test.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    16745 2024-04-18 14:35:19.000000 mozilla_version-3.0.0/requirements/test.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       38 2024-04-18 14:37:08.034664 mozilla_version-3.0.0/setup.cfg
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1194 2023-05-23 08:14:29.000000 mozilla_version-3.0.0/setup.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)        6 2024-04-18 14:35:19.000000 mozilla_version-3.0.0/version.txt
+drwxrwxr-x   0 jcristau  (1000) jcristau  (1000)        0 2024-05-27 17:08:37.874801 mozilla-version-3.1.0/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       50 2021-07-20 18:27:27.000000 mozilla-version-3.1.0/.coveragerc
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      738 2021-07-20 18:27:27.000000 mozilla-version-3.1.0/.gitignore
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)      895 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/.pre-commit-config.yaml
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     4454 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/.taskcluster.yml
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     5200 2024-05-27 15:59:58.000000 mozilla-version-3.1.0/CHANGELOG.md
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)      689 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)    15921 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/LICENSE
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      139 2021-07-20 18:27:27.000000 mozilla-version-3.1.0/MANIFEST.in
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)      451 2024-05-27 17:08:37.874801 mozilla-version-3.1.0/PKG-INFO
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     7518 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/README.md
+drwxrwxr-x   0 jcristau  (1000) jcristau  (1000)        0 2024-05-27 17:08:37.866801 mozilla-version-3.1.0/docs/
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)      613 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/docs/Makefile
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     7518 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/docs/README.md
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     6731 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/docs/conf.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      507 2021-07-20 18:27:27.000000 mozilla-version-3.1.0/docs/index.rst
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      709 2021-07-20 18:27:27.000000 mozilla-version-3.1.0/docs/mozilla_version.rst
+drwxrwxr-x   0 jcristau  (1000) jcristau  (1000)        0 2024-05-27 17:08:37.866801 mozilla-version-3.1.0/maintenance/
+-rwxrwxr-x   0 jcristau  (1000) jcristau  (1000)     1221 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/maintenance/pin.sh
+drwxrwxr-x   0 jcristau  (1000) jcristau  (1000)        0 2024-05-27 17:08:37.870802 mozilla-version-3.1.0/mozilla_version/
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)      391 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/__init__.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     5072 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/balrog.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     2401 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/errors.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)      200 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/fenix.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)    31141 2024-05-27 15:59:14.000000 mozilla-version-3.1.0/mozilla_version/gecko.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     1971 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/maven.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)    10146 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/mobile.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1335 2023-04-12 09:33:15.000000 mozilla-version-3.1.0/mozilla_version/parser.py
+drwxrwxr-x   0 jcristau  (1000) jcristau  (1000)        0 2024-05-27 17:08:37.870802 mozilla-version-3.1.0/mozilla_version/test/
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)       88 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/test/__init__.py
+drwxrwxr-x   0 jcristau  (1000) jcristau  (1000)        0 2024-05-27 17:08:37.870802 mozilla-version-3.1.0/mozilla_version/test/integration/
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)      345 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/test/integration/__init__.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     1369 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/test/integration/test_product_details.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     9431 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/test/test_balrog.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)      303 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/test/test_default_imports.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     1037 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/test/test_errors.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      193 2022-08-25 14:26:48.000000 mozilla-version-3.1.0/mozilla_version/test/test_fenix.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)    49787 2024-05-27 15:59:14.000000 mozilla-version-3.1.0/mozilla_version/test/test_gecko.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     3904 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/test/test_maven.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)    12792 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/test/test_mobile.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     8308 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/test/test_version.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)    10212 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/mozilla_version/version.py
+drwxrwxr-x   0 jcristau  (1000) jcristau  (1000)        0 2024-05-27 17:08:37.870802 mozilla-version-3.1.0/mozilla_version.egg-info/
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)      451 2024-05-27 17:08:37.000000 mozilla-version-3.1.0/mozilla_version.egg-info/PKG-INFO
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     1356 2024-05-27 17:08:37.000000 mozilla-version-3.1.0/mozilla_version.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)        1 2024-05-27 17:08:37.000000 mozilla-version-3.1.0/mozilla_version.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)        1 2024-05-27 17:08:37.000000 mozilla-version-3.1.0/mozilla_version.egg-info/not-zip-safe
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)       12 2024-05-27 17:08:37.000000 mozilla-version-3.1.0/mozilla_version.egg-info/requires.txt
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)       16 2024-05-27 17:08:37.000000 mozilla-version-3.1.0/mozilla_version.egg-info/top_level.txt
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)      916 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/pyproject.toml
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      361 2023-04-11 13:53:15.000000 mozilla-version-3.1.0/readthedocs.yml
+drwxrwxr-x   0 jcristau  (1000) jcristau  (1000)        0 2024-05-27 17:08:37.874801 mozilla-version-3.1.0/requirements/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       12 2023-04-12 09:33:15.000000 mozilla-version-3.1.0/requirements/base.in
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)      363 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/requirements/base.txt
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)      169 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/requirements/docs.in
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)    17719 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/requirements/docs.txt
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)       22 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/requirements/local.in
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     6281 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/requirements/local.txt
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)       98 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/requirements/test.in
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)    16745 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/requirements/test.txt
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)       38 2024-05-27 17:08:37.874801 mozilla-version-3.1.0/setup.cfg
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     1171 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/setup.py
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)     1380 2024-05-27 15:00:50.000000 mozilla-version-3.1.0/tox.ini
+-rw-rw-r--   0 jcristau  (1000) jcristau  (1000)        6 2024-05-27 16:05:31.000000 mozilla-version-3.1.0/version.txt
```

### Comparing `mozilla_version-3.0.0/LICENSE` & `mozilla-version-3.1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -356,8 +356,7 @@
 You may add additional accurate notices of copyright ownership.
 
 Exhibit B - "Incompatible With Secondary Licenses" Notice
 
       This Source Code Form is "Incompatible
       With Secondary Licenses", as defined by
       the Mozilla Public License, v. 2.0.
-
```

### Comparing `mozilla_version-3.0.0/README.md` & `mozilla-version-3.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 ## Hack on the code
 ```sh
 virtualenv venv         # create the virtualenv in ./venv
 . venv/bin/activate    # activate it
 git clone https://github.com/mozilla-releng/mozilla-version
 cd mozilla-version
-pip install mozilla-version
+pip install --require-hashes -r requirements/local.txt
 ```
 
 
 ## Design choices
 
 
 ### Object-oriented programming
```

### Comparing `mozilla_version-3.0.0/mozilla_version/balrog.py` & `mozilla-version-3.1.0/mozilla_version/balrog.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,107 +13,120 @@
         balrog_release.product                 # firefox
         balrog_release.version.major_number    # 60
         str(balrog_release)                    # 'firefox-60.0.1-build1'
 
         previous_release = BalrogReleaseName.parse('firefox-60.0-build2')
         previous_release < balrog_release      # True
 
-        invalid = BalrogReleaseName.parse('60.0.1')           # raises PatternNotMatchedError
-        invalid = BalrogReleaseName.parse('firefox-60.0.1')   # raises PatternNotMatchedError
+        BalrogReleaseName.parse('60.0.1')           # raises PatternNotMatchedError
+        BalrogReleaseName.parse('firefox-60.0.1')   # raises PatternNotMatchedError
 
         # Releases can be built thanks to version classes like FirefoxVersion
-        BalrogReleaseName('firefox', FirefoxVersion(60, 0, 1, 1))  # 'firefox-60.0.1-build1'
+        BalrogReleaseName('firefox', FirefoxVersion(60, 0, 1))  # 'firefox-60.0-build1'
 
 """
 
-import attr
 import re
 
+import attr
+
 from mozilla_version.errors import PatternNotMatchedError
-from mozilla_version.parser import get_value_matched_by_regex
 from mozilla_version.gecko import (
-    GeckoVersion, FirefoxVersion, DeveditionVersion, FennecVersion, ThunderbirdVersion
+    DeveditionVersion,
+    FennecVersion,
+    FirefoxVersion,
+    GeckoVersion,
+    ThunderbirdVersion,
 )
-
+from mozilla_version.parser import get_value_matched_by_regex
 
 _VALID_ENOUGH_BALROG_RELEASE_PATTERN = re.compile(
     r"^(?P<product>[a-z]+)-(?P<version>.+)$", re.IGNORECASE
 )
 
 
 _SUPPORTED_PRODUCTS = {
-    'firefox': FirefoxVersion,
-    'devedition': DeveditionVersion,
-    'fennec': FennecVersion,
-    'thunderbird': ThunderbirdVersion,
+    "firefox": FirefoxVersion,
+    "devedition": DeveditionVersion,
+    "fennec": FennecVersion,
+    "thunderbird": ThunderbirdVersion,
 }
 
 
 def _supported_product(string):
     product = string.lower()
     if product not in _SUPPORTED_PRODUCTS:
-        raise PatternNotMatchedError(string, patterns=('unknown product',))
+        raise PatternNotMatchedError(string, patterns=("unknown product",))
     return product
 
 
 def _products_must_be_identical(method):
     def checker(this, other):
         if this.product != other.product:
             raise ValueError(f'Cannot compare "{this.product}" and "{other.product}"')
         return method(this, other)
+
     return checker
 
 
 @attr.s(frozen=True, eq=False, hash=True)
 class BalrogReleaseName:
     """Class that validates and handles Balrog release names.
 
     Raises:
-        PatternNotMatchedError: if a parsed string doesn't match the pattern of a valid release
-        MissingFieldError: if a mandatory field is missing in the string. Mandatory fields are
+        PatternNotMatchedError: if a parsed string doesn't match the pattern of a valid
+            release
+        MissingFieldError: if a mandatory field is missing in the string. Mandatory
+            fields are
             `product`, `major_number`, `minor_number`, and `build_number`
         ValueError: if an integer can't be cast or is not (strictly) positive
         TooManyTypesError: if the string matches more than 1 `VersionType`
         NoVersionTypeError: if the string matches none.
 
     """
 
     product = attr.ib(type=str, converter=_supported_product)
     version = attr.ib(type=GeckoVersion)
 
     def __attrs_post_init__(self):
         """Ensure attributes are sane all together."""
         if self.version.build_number is None:
-            raise PatternNotMatchedError(self, patterns=('build_number must exist',))
+            raise PatternNotMatchedError(self, patterns=("build_number must exist",))
 
     @classmethod
     def parse(cls, release_string):
         """Construct an object representing a valid Firefox version number."""
         regex_matches = _VALID_ENOUGH_BALROG_RELEASE_PATTERN.match(release_string)
         if regex_matches is None:
-            raise PatternNotMatchedError(release_string, (_VALID_ENOUGH_BALROG_RELEASE_PATTERN,))
+            raise PatternNotMatchedError(
+                release_string, (_VALID_ENOUGH_BALROG_RELEASE_PATTERN,)
+            )
 
-        product = get_value_matched_by_regex('product', regex_matches, release_string)
+        product = get_value_matched_by_regex("product", regex_matches, release_string)
         try:
-            VersionClass = _SUPPORTED_PRODUCTS[product.lower()]
+            version_class = _SUPPORTED_PRODUCTS[product.lower()]
         except KeyError:
-            raise PatternNotMatchedError(release_string, patterns=('unknown product',))
-
-        version_string = get_value_matched_by_regex('version', regex_matches, release_string)
-        version = VersionClass.parse(version_string)
+            raise PatternNotMatchedError(
+                release_string, patterns=("unknown product",)
+            ) from None
+
+        version_string = get_value_matched_by_regex(
+            "version", regex_matches, release_string
+        )
+        version = version_class.parse(version_string)
 
         return cls(product, version)
 
     def __str__(self):
         """Implement string representation.
 
         Computes a new string based on the given attributes.
         """
-        version_string = str(self.version).replace('build', '-build')
-        return f'{self.product}-{version_string}'
+        version_string = str(self.version).replace("build", "-build")
+        return f"{self.product}-{version_string}"
 
     @_products_must_be_identical
     def __eq__(self, other):
         """Implement `==` operator."""
         return self.version == other.version
 
     @_products_must_be_identical
```

### Comparing `mozilla_version-3.0.0/mozilla_version/errors.py` & `mozilla-version-3.1.0/mozilla_version/errors.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,21 +9,20 @@
         patterns (sequence): The patterns it tried to match.
     """
 
     def __init__(self, string, patterns):
         """Initialize error."""
         number_of_patterns = len(patterns)
         if number_of_patterns == 0:
-            raise ValueError('At least one pattern must be provided')
-        elif number_of_patterns == 1:
+            raise ValueError("At least one pattern must be provided")
+        if number_of_patterns == 1:
             message = f'"{string}" does not match the pattern: {patterns[0]}'
         else:
             message = '"{}" does not match the patterns:\n - {}'.format(
-                string,
-                '\n - '.join(patterns)
+                string, "\n - ".join(patterns)
             )
 
         super().__init__(message)
 
 
 class NoVersionTypeError(ValueError):
     """Error when `version_string` matched the pattern, but was unable to find its type.
@@ -31,18 +30,17 @@
     Args:
         version_string (str): The string it was unable to guess the type.
     """
 
     def __init__(self, version_string):
         """Initialize error."""
         super().__init__(
-            'Version "{}" matched the pattern of a valid version, but it is unable to '
-            'find what type it is. This is likely a bug in mozilla-version'.format(
-                version_string
-            )
+            f'Version "{version_string}" matched the pattern of a valid version, but '
+            "it is unable to find what type it is. This is likely a bug in "
+            "mozilla-version"
         )
 
 
 class MissingFieldError(ValueError):
     """Error when `version_string` lacks an expected field.
 
     Args:
@@ -65,11 +63,10 @@
         first_matched_type (str): The name of the first detected type.
         second_matched_type (str): The name of the second detected type
     """
 
     def __init__(self, version_string, first_matched_type, second_matched_type):
         """Initialize error."""
         super().__init__(
-            'Release "{}" cannot match types "{}" and "{}"'.format(
-                version_string, first_matched_type, second_matched_type
-            )
+            f'Release "{version_string}" cannot match types "{first_matched_type}" and '
+            f'"{second_matched_type}"'
         )
```

### Comparing `mozilla_version-3.0.0/mozilla_version/gecko.py` & `mozilla-version-3.1.0/mozilla_version/gecko.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         previous_version.minor_number   # 0
         previous_version.patch_number   # raises AttributeError
 
         previous_version.is_beta     # True
         previous_version.is_release  # False
         previous_version.is_nightly  # False
 
-        invalid_version = FirefoxVersion.parse('60.1')      # raises PatternNotMatchedError
-        invalid_version = FirefoxVersion.parse('60.0.0')    # raises PatternNotMatchedError
+        FirefoxVersion.parse('60.1')      # raises PatternNotMatchedError
+        FirefoxVersion.parse('60.0.0')    # raises PatternNotMatchedError
         version = FirefoxVersion.parse('60.0')    # valid
 
         # Versions can be built by raw values
         FirefoxVersion(60, 0))         # '60.0'
         FirefoxVersion(60, 0, 1))      # '60.0.1'
         FirefoxVersion(60, 1, 0))      # '60.1.0'
         FirefoxVersion(60, 0, 1, 1))   # '60.0.1build1'
@@ -42,32 +42,33 @@
         FirefoxVersion(60, 0, is_nightly=True))     # '60.0a1'
         FirefoxVersion(60, 0, is_aurora_or_devedition=True))    # '60.0a2'
         FirefoxVersion(60, 0, is_esr=True))         # '60.0esr'
         FirefoxVersion(60, 0, 1, is_esr=True))      # '60.0.1esr'
 
 """
 
-import attr
 import re
 
+import attr
+
 from mozilla_version.errors import (
-    PatternNotMatchedError, TooManyTypesError, NoVersionTypeError
+    NoVersionTypeError,
+    PatternNotMatchedError,
+    TooManyTypesError,
 )
 from mozilla_version.parser import strictly_positive_int_or_none
 from mozilla_version.version import BaseVersion, ShipItVersion, VersionType
 
 
 def _find_type(version):
     version_type = None
 
     def ensure_version_type_is_not_already_defined(previous_type, candidate_type):
         if previous_type is not None:
-            raise TooManyTypesError(
-                str(version), previous_type, candidate_type
-            )
+            raise TooManyTypesError(str(version), previous_type, candidate_type)
 
     if version.is_nightly:
         version_type = VersionType.NIGHTLY
     if version.is_aurora_or_devedition:
         ensure_version_type_is_not_already_defined(
             version_type, VersionType.AURORA_OR_DEVEDITION
         )
@@ -75,15 +76,17 @@
     if version.is_beta:
         ensure_version_type_is_not_already_defined(version_type, VersionType.BETA)
         version_type = VersionType.BETA
     if version.is_esr:
         ensure_version_type_is_not_already_defined(version_type, VersionType.ESR)
         version_type = VersionType.ESR
     if version.is_release_candidate:
-        ensure_version_type_is_not_already_defined(version_type, VersionType.RELEASE_CANDIDATE)
+        ensure_version_type_is_not_already_defined(
+            version_type, VersionType.RELEASE_CANDIDATE
+        )
         version_type = VersionType.RELEASE_CANDIDATE
     if version.is_release:
         ensure_version_type_is_not_already_defined(version_type, VersionType.RELEASE)
         version_type = VersionType.RELEASE
 
     if version_type is None:
         raise NoVersionTypeError(str(version))
@@ -91,274 +94,350 @@
     return version_type
 
 
 @attr.s(frozen=True, eq=False, hash=True)
 class GeckoVersion(ShipItVersion):
     """Class that validates and handles version numbers for Gecko-based products.
 
-    You may want to use specific classes like FirefoxVersion. These classes define edge cases
-    that were shipped.
+    You may want to use specific classes like FirefoxVersion. These classes define edge
+    cases that were shipped.
 
     Raises:
-        PatternNotMatchedError: if the string doesn't match the pattern of a valid version number
-        MissingFieldError: if a mandatory field is missing in the string. Mandatory fields are
-            `major_number` and `minor_number`
+        PatternNotMatchedError: if the string doesn't match the pattern of a valid
+            version number
+        MissingFieldError: if a mandatory field is missing in the string. Mandatory
+            fields are `major_number` and `minor_number`
         ValueError: if an integer can't be cast or is not (strictly) positive
         TooManyTypesError: if the string matches more than 1 `VersionType`
         NoVersionTypeError: if the string matches none.
 
     """
 
-    # XXX This pattern doesn't catch all subtleties of a Firefox version (like 32.5 isn't valid).
-    # This regex is intended to assign numbers. Then checks are done by attrs and
-    # __attrs_post_init__()
-    _VALID_ENOUGH_VERSION_PATTERN = re.compile(r"""
+    # XXX This pattern doesn't catch all subtleties of a Firefox version (like 32.5
+    # isn't valid). This regex is intended to assign numbers. Then checks are done by
+    # attrs and __attrs_post_init__()
+    _VALID_ENOUGH_VERSION_PATTERN = re.compile(
+        r"""
         ^(?P<major_number>\d+)
         \.(?P<minor_number>\d+)
         (\.(?P<patch_number>\d+))?
         (\.(?P<old_fourth_number>\d+))?
         (
             (?P<is_nightly>a1)
             |(?P<is_aurora_or_devedition>a2)
             |rc(?P<release_candidate_number>\d+)
             |b(?P<beta_number>\d+)
             |(?P<is_esr>esr)
         )?
-        -?(build(?P<build_number>\d+))?$""", re.VERBOSE)
+        -?(build(?P<build_number>\d+))?$""",
+        re.VERBOSE,
+    )
 
-    _OPTIONAL_NUMBERS = BaseVersion._OPTIONAL_NUMBERS + (
-        'old_fourth_number', 'release_candidate_number', 'beta_number', 'build_number'
+    _OPTIONAL_NUMBERS = (
+        *BaseVersion._OPTIONAL_NUMBERS,
+        "old_fourth_number",
+        "release_candidate_number",
+        "beta_number",
+        "build_number",
     )
 
     _ALL_NUMBERS = BaseVersion._ALL_NUMBERS + _OPTIONAL_NUMBERS
 
-    _KNOWN_ESR_MAJOR_NUMBERS = (10, 17, 24, 31, 38, 45, 52, 60, 68, 78, 91, 102, 115)
+    _KNOWN_ESR_MAJOR_NUMBERS = (
+        10,
+        17,
+        24,
+        31,
+        38,
+        45,
+        52,
+        60,
+        68,
+        78,
+        91,
+        102,
+        115,
+        128,
+    )
 
-    _BOOLEANS_NOT_INFERRED_BY_NUMBERS = ('is_nightly', 'is_aurora_or_devedition', 'is_esr')
+    _BOOLEANS_NOT_INFERRED_BY_NUMBERS = (
+        "is_nightly",
+        "is_aurora_or_devedition",
+        "is_esr",
+    )
 
     _LAST_AURORA_DEVEDITION_AS_VERSION_TYPE = 54
 
-    build_number = attr.ib(type=int, converter=strictly_positive_int_or_none, default=None)
-    beta_number = attr.ib(type=int, converter=strictly_positive_int_or_none, default=None)
+    build_number = attr.ib(
+        type=int, converter=strictly_positive_int_or_none, default=None
+    )
+    beta_number = attr.ib(
+        type=int, converter=strictly_positive_int_or_none, default=None
+    )
     is_nightly = attr.ib(type=bool, default=False)
     is_aurora_or_devedition = attr.ib(type=bool, default=False)
     is_esr = attr.ib(type=bool, default=False)
-    old_fourth_number = attr.ib(type=int, converter=strictly_positive_int_or_none, default=None)
+    old_fourth_number = attr.ib(
+        type=int, converter=strictly_positive_int_or_none, default=None
+    )
     release_candidate_number = attr.ib(
         type=int, converter=strictly_positive_int_or_none, default=None
     )
-    version_type = attr.ib(init=False, default=attr.Factory(_find_type, takes_self=True))
+    version_type = attr.ib(
+        init=False, default=attr.Factory(_find_type, takes_self=True)
+    )
 
     def _get_all_error_messages_for_attributes(self):
         error_messages = super()._get_all_error_messages_for_attributes()
 
         # General checks
-        error_messages.extend([
-            pattern_message
-            for condition, pattern_message in ((
-                not self.is_four_digit_scheme and self.old_fourth_number is not None,
-                'The old fourth number can only be defined on Gecko 1.5.x.y or 2.0.x.y',
-            ), (
-                self.beta_number is not None and self.patch_number is not None,
-                'Beta number and patch number cannot be both defined',
-            ), (
-                self.is_major and self.is_esr,
-                'Version cannot be both a major and an ESR one',
-            ), (
-                self.is_stability and self.is_esr,
-                'Version cannot be both a stability and an ESR one',
-            ), (
-                self.is_development and self.is_esr,
-                'Version cannot be both a development and an ESR one',
-            ))
-            if condition
-        ])
+        error_messages.extend(
+            [
+                pattern_message
+                for condition, pattern_message in (
+                    (
+                        not self.is_four_digit_scheme
+                        and self.old_fourth_number is not None,
+                        "The old fourth number can only be defined on Gecko 1.5.x.y or "
+                        "2.0.x.y",
+                    ),
+                    (
+                        self.beta_number is not None and self.patch_number is not None,
+                        "Beta number and patch number cannot be both defined",
+                    ),
+                    (
+                        self.is_major and self.is_esr,
+                        "Version cannot be both a major and an ESR one",
+                    ),
+                    (
+                        self.is_stability and self.is_esr,
+                        "Version cannot be both a stability and an ESR one",
+                    ),
+                    (
+                        self.is_development and self.is_esr,
+                        "Version cannot be both a development and an ESR one",
+                    ),
+                )
+                if condition
+            ]
+        )
 
-        # Firefox 5 is the first version to implement the rapid release model, which defines
-        # the scheme used so far.
+        # Firefox 5 is the first version to implement the rapid release model, which
+        # defines the scheme used so far.
         if self.is_rapid_release_scheme:
-            error_messages.extend([
-                pattern_message
-                for condition, pattern_message in ((
-                    self.release_candidate_number is not None,
-                    'Release candidate number cannot be defined starting Gecko 5',
-                ), (
-                    self.minor_number == 0 and self.patch_number == 0,
-                    'Minor number and patch number cannot be both equal to 0',
-                ), (
-                    self.minor_number != 0 and self.patch_number is None,
-                    'Patch number cannot be undefined if minor number is greater than 0',
-                ), (
-                    self.patch_number is not None and self.is_nightly,
-                    'Patch number cannot be defined on a nightly version',
-                ), (
-                    self.patch_number is not None and self.is_aurora_or_devedition,
-                    'Patch number cannot be defined on an aurora version',
-                ), (
-                    self.major_number > self._LAST_AURORA_DEVEDITION_AS_VERSION_TYPE and
-                    self.is_aurora_or_devedition,
-                    'Last aurora/devedition version was 54.0a2. Please use the DeveditionVersion '
-                    'class, past this version.',
-                ), (
-                    self.major_number not in self._KNOWN_ESR_MAJOR_NUMBERS and self.is_esr,
-                    '"{}" is not a valid ESR major number. Valid ones are: {}'.format(
-                        self.major_number, self._KNOWN_ESR_MAJOR_NUMBERS
+            error_messages.extend(
+                [
+                    pattern_message
+                    for condition, pattern_message in (
+                        (
+                            self.release_candidate_number is not None,
+                            "Release candidate number cannot be defined starting "
+                            "Gecko 5",
+                        ),
+                        (
+                            self.minor_number == 0 and self.patch_number == 0,
+                            "Minor number and patch number cannot be both equal to 0",
+                        ),
+                        (
+                            self.minor_number != 0 and self.patch_number is None,
+                            "Patch number cannot be undefined if minor number is "
+                            "greater than 0",
+                        ),
+                        (
+                            self.patch_number is not None and self.is_nightly,
+                            "Patch number cannot be defined on a nightly version",
+                        ),
+                        (
+                            self.patch_number is not None
+                            and self.is_aurora_or_devedition,
+                            "Patch number cannot be defined on an aurora version",
+                        ),
+                        (
+                            self.major_number
+                            > self._LAST_AURORA_DEVEDITION_AS_VERSION_TYPE
+                            and self.is_aurora_or_devedition,
+                            "Last aurora/devedition version was 54.0a2. Please use the "
+                            "DeveditionVersion class, past this version.",
+                        ),
+                        (
+                            self.major_number not in self._KNOWN_ESR_MAJOR_NUMBERS
+                            and self.is_esr,
+                            f'"{self.major_number}" is not a valid ESR major number. '
+                            f"Valid ones are: {self._KNOWN_ESR_MAJOR_NUMBERS}",
+                        ),
                     )
-                ))
-                if condition
-            ])
+                    if condition
+                ]
+            )
         else:
             if self.release_candidate_number is not None:
-                error_messages.extend([
-                    pattern_message
-                    for condition, pattern_message in ((
-                        self.patch_number is not None,
-                        'Release candidate and patch number cannot be both defined',
-                    ), (
-                        self.old_fourth_number is not None,
-                        'Release candidate and the old fourth number cannot be both defined',
-                    ), (
-                        self.beta_number is not None,
-                        'Release candidate and beta number cannot be both defined',
-                    ))
-                    if condition
-                ])
+                error_messages.extend(
+                    [
+                        pattern_message
+                        for condition, pattern_message in (
+                            (
+                                self.patch_number is not None,
+                                "Release candidate and patch number cannot be both "
+                                "defined",
+                            ),
+                            (
+                                self.old_fourth_number is not None,
+                                "Release candidate and the old fourth number cannot be "
+                                "both defined",
+                            ),
+                            (
+                                self.beta_number is not None,
+                                "Release candidate and beta number cannot be both "
+                                "defined",
+                            ),
+                        )
+                        if condition
+                    ]
+                )
 
             if self.old_fourth_number is not None and self.patch_number != 0:
                 error_messages.append(
-                    'The old fourth number cannot be defined if the patch number is not 0 '
-                    '(we have never shipped a release that did so)'
+                    "The old fourth number cannot be defined if the patch number is "
+                    "not 0 (we have never shipped a release that did so)"
                 )
 
         return error_messages
 
     @classmethod
     def parse(cls, version_string):
         """Construct an object representing a valid Firefox version number."""
         return super().parse(
             version_string, regex_groups=cls._BOOLEANS_NOT_INFERRED_BY_NUMBERS
         )
 
     @property
     def is_beta(self):
-        """Return `True` if `GeckoVersion` was built with a string matching a beta version."""
+        """Return `True` if `GeckoVersion` was built with a `beta_number`."""
         return self.beta_number is not None
 
     @property
     def is_release_candidate(self):
-        """Return `True` if `GeckoVersion` was built with a string matching an RC version."""
+        """Return `True` if `GeckoVersion` was built with `release_candidate_number`."""
         return self.release_candidate_number is not None
 
     @property
     def is_rapid_release_scheme(self):
-        """Return `True` if `GeckoVersion` was built with against the rapid release scheme."""
+        """Return `True` if `GeckoVersion` was built with the rapid release scheme."""
         return self.major_number >= 5
 
     @property
     def is_four_digit_scheme(self):
         """Return `True` if `GeckoVersion` was built with the 4 digits schemes.
 
         Only Firefox 1.5.x.y and 2.0.x.y were.
         """
-        return (
-            all((self.major_number == 1, self.minor_number == 5)) or
-            all((self.major_number == 2, self.minor_number == 0))
+        return all((self.major_number == 1, self.minor_number == 5)) or all(
+            (self.major_number == 2, self.minor_number == 0)
         )
 
     @property
     def is_release(self):
-        """Return `True` if `GeckoVersion` was built with a string matching a release version."""
-        return not any((
-            self.is_nightly, self.is_aurora_or_devedition, self.is_beta,
-            self.is_release_candidate, self.is_esr
-        ))
+        """Return `True` if `GeckoVersion` was built as a release version."""
+        return not any(
+            (
+                self.is_nightly,
+                self.is_aurora_or_devedition,
+                self.is_beta,
+                self.is_release_candidate,
+                self.is_esr,
+            )
+        )
 
     @property
     def is_major(self):
         """Return `True` if `GeckoVersion` is considered to be a major version.
 
-        It's usually the .0 release but some exceptions may occur. ESR are not considered
-        major versions.
+        It's usually the .0 release but some exceptions may occur. ESR are not
+        considered major versions.
         """
         return super().is_major and not self.is_esr
 
     @property
     def is_stability(self):
         """Return `True` if `GeckoVersion` is a version that fixed a major one."""
         conditions = [
             not self.is_esr,
         ]
         if self.is_four_digit_scheme:
             # super().is_stability has an incompatible condition. So we must not use it
             # in this specific case.
-            conditions.extend([
-                not self.is_development,
-                not self.is_major,
-                self.patch_number == 0,
-                self.old_fourth_number != 0,
-            ])
+            conditions.extend(
+                [
+                    not self.is_development,
+                    not self.is_major,
+                    self.patch_number == 0,
+                    self.old_fourth_number != 0,
+                ]
+            )
         else:
             conditions.append(super().is_stability)
 
         return all(conditions)
 
     def __str__(self):
         """Implement string representation.
 
         Computes a new string based on the given attributes.
         """
         string = super().__str__()
 
         if self.old_fourth_number is not None:
-            string = f'{string}.{self.old_fourth_number}'
+            string = f"{string}.{self.old_fourth_number}"
 
         if self.is_nightly:
-            string = f'{string}a1'
+            string = f"{string}a1"
         elif self.is_aurora_or_devedition:
-            string = f'{string}a2'
+            string = f"{string}a2"
         elif self.is_beta:
-            string = f'{string}b{self.beta_number}'
+            string = f"{string}b{self.beta_number}"
         elif self.is_release_candidate:
-            string = f'{string}rc{self.release_candidate_number}'
+            string = f"{string}rc{self.release_candidate_number}"
         elif self.is_esr:
-            string = f'{string}esr'
+            string = f"{string}esr"
 
         if self.build_number is not None:
-            string = f'{string}build{self.build_number}'
+            string = f"{string}build{self.build_number}"
 
         return string
 
     def __eq__(self, other):
         """Implement `==` operator.
 
-        A version is considered equal to another if all numbers match and if they are of the same
-        `VersionType`. Like said in `VersionType`, release and ESR are considered equal (if they
-        share the same numbers). If a version contains a build number but not the other, the build
-        number won't be considered in the comparison.
+        A version is considered equal to another if all numbers match and if they are
+        of the same `VersionType`. Like said in `VersionType`, release and ESR are
+        considered equal (if they share the same numbers). If a version contains a
+        build number but not the other, the build number won't be considered in the
+        comparison.
 
         Examples:
             .. code-block:: python
 
-                assert GeckoVersion.parse('60.0') == GeckoVersion.parse('60.0')
-                assert GeckoVersion.parse('60.0') == GeckoVersion.parse('60.0esr')
-                assert GeckoVersion.parse('60.0') == GeckoVersion.parse('60.0build1')
-                assert GeckoVersion.parse('60.0build1') == GeckoVersion.parse('60.0build1')
-
-                assert GeckoVersion.parse('60.0') != GeckoVersion.parse('61.0')
-                assert GeckoVersion.parse('60.0') != GeckoVersion.parse('60.1.0')
-                assert GeckoVersion.parse('60.0') != GeckoVersion.parse('60.0.1')
-                assert GeckoVersion.parse('60.0') != GeckoVersion.parse('60.0a1')
-                assert GeckoVersion.parse('60.0') != GeckoVersion.parse('60.0a2')
-                assert GeckoVersion.parse('60.0') != GeckoVersion.parse('60.0b1')
-                assert GeckoVersion.parse('60.0build1') != GeckoVersion.parse('60.0build2')
+                GeckoVersion.parse('60.0') == GeckoVersion.parse('60.0')
+                GeckoVersion.parse('60.0') == GeckoVersion.parse('60.0esr')
+                GeckoVersion.parse('60.0') == GeckoVersion.parse('60.0build1')
+                GeckoVersion.parse('60.0build1') == GeckoVersion.parse('60.0build1')
+
+                GeckoVersion.parse('60.0') != GeckoVersion.parse('61.0')
+                GeckoVersion.parse('60.0') != GeckoVersion.parse('60.1.0')
+                GeckoVersion.parse('60.0') != GeckoVersion.parse('60.0.1')
+                GeckoVersion.parse('60.0') != GeckoVersion.parse('60.0a1')
+                GeckoVersion.parse('60.0') != GeckoVersion.parse('60.0a2')
+                GeckoVersion.parse('60.0') != GeckoVersion.parse('60.0b1')
+                GeckoVersion.parse('60.0build1') != GeckoVersion.parse('60.0build2')
 
         """
         return super().__eq__(other)
 
-    def _compare(self, other):
+    # TODO: Make this function simpler to pass complexity check (C901)
+    def _compare(self, other):  # noqa C901
         """Compare this release with another.
 
         Returns:
             0 if equal
             < 0 is this precedes the other
             > 0 if the other precedes this
 
@@ -368,143 +447,157 @@
         elif not isinstance(other, GeckoVersion):
             raise ValueError(f'Cannot compare "{other}", type not supported!')
 
         difference = super()._compare(other)
         if difference != 0:
             return difference
 
-        difference = self._substract_other_number_from_this_number(other, 'old_fourth_number')
+        difference = self._substract_other_number_from_this_number(
+            other, "old_fourth_number"
+        )
         if difference != 0:
             return difference
 
         channel_difference = self._compare_version_type(other)
         if channel_difference != 0:
             return channel_difference
 
         if self.is_beta and other.is_beta:
             beta_difference = self.beta_number - other.beta_number
             if beta_difference != 0:
                 return beta_difference
 
         if self.is_release_candidate and other.is_release_candidate:
-            rc_difference = self.release_candidate_number - other.release_candidate_number
+            rc_difference = (
+                self.release_candidate_number - other.release_candidate_number
+            )
             if rc_difference != 0:
                 return rc_difference
 
         # Build numbers are a special case. We might compare a regular version number
-        # (like "32.0b8") versus a release build (as in "32.0b8build1"). As a consequence,
-        # we only compare build_numbers when we both have them.
+        # (like "32.0b8") versus a release build (as in "32.0b8build1"). As a
+        # consequence, we only compare build_numbers when we both have them.
         try:
             return self.build_number - other.build_number
         except TypeError:
             pass
 
         return 0
 
     def _compare_version_type(self, other):
         return self.version_type.compare(other.version_type)
 
-    def _create_bump_kwargs(self, field):
-        if field == 'build_number' and self.build_number is None:
-            raise ValueError('Cannot bump the build number if it is not already set')
+    # TODO: Make this function simpler to pass complexity check (C901)
+    def _create_bump_kwargs(self, field):  # noqa C901
+        if field == "build_number" and self.build_number is None:
+            raise ValueError("Cannot bump the build number if it is not already set")
 
         bump_kwargs = super()._create_bump_kwargs(field)
 
-        if field == 'major_number' and self.is_esr:
+        if field == "major_number" and self.is_esr:
             current_esr_index = self._KNOWN_ESR_MAJOR_NUMBERS.index(self.major_number)
             try:
-                next_major_esr_number = self._KNOWN_ESR_MAJOR_NUMBERS[current_esr_index + 1]
+                next_major_esr_number = self._KNOWN_ESR_MAJOR_NUMBERS[
+                    current_esr_index + 1
+                ]
             except IndexError:
                 raise ValueError(
-                    "Cannot bump the major number past last known major ESR. We don't know it yet."
-                )
-            bump_kwargs['major_number'] = next_major_esr_number
-
-        if field != 'build_number' and bump_kwargs.get('build_number') == 0:
-            del bump_kwargs['build_number']
-        if bump_kwargs.get('beta_number') == 0:
+                    "Cannot bump the major number past last known major ESR. We don't "
+                    "know it yet."
+                ) from None
+            bump_kwargs["major_number"] = next_major_esr_number
+
+        if field != "build_number" and bump_kwargs.get("build_number") == 0:
+            del bump_kwargs["build_number"]
+        if bump_kwargs.get("beta_number") == 0:
             if self.is_beta:
-                bump_kwargs['beta_number'] = 1
+                bump_kwargs["beta_number"] = 1
             else:
-                del bump_kwargs['beta_number']
-
-        if field != 'old_fourth_number' and not self.is_four_digit_scheme:
-            del bump_kwargs['old_fourth_number']
-            if bump_kwargs.get('minor_number') == 0 and bump_kwargs.get('patch_number') == 0:
-                del bump_kwargs['patch_number']
+                del bump_kwargs["beta_number"]
 
-        if self.is_four_digit_scheme:
+        if field != "old_fourth_number" and not self.is_four_digit_scheme:
+            del bump_kwargs["old_fourth_number"]
             if (
-                bump_kwargs.get('patch_number') == 0 and
-                bump_kwargs.get('old_fourth_number') in (0, None)
+                bump_kwargs.get("minor_number") == 0
+                and bump_kwargs.get("patch_number") == 0
             ):
-                del bump_kwargs['patch_number']
-                del bump_kwargs['old_fourth_number']
+                del bump_kwargs["patch_number"]
+
+        if self.is_four_digit_scheme:
+            if bump_kwargs.get("patch_number") == 0 and bump_kwargs.get(
+                "old_fourth_number"
+            ) in (0, None):
+                del bump_kwargs["patch_number"]
+                del bump_kwargs["old_fourth_number"]
             elif (
-                bump_kwargs.get('patch_number') is None and
-                bump_kwargs.get('old_fourth_number') is not None and
-                bump_kwargs.get('old_fourth_number') > 0
+                bump_kwargs.get("patch_number") is None
+                and bump_kwargs.get("old_fourth_number") is not None
+                and bump_kwargs.get("old_fourth_number") > 0
             ):
-                bump_kwargs['patch_number'] = 0
+                bump_kwargs["patch_number"] = 0
 
-        if field != 'release_candidate_number' and self.is_rapid_release_scheme:
-            del bump_kwargs['release_candidate_number']
+        if field != "release_candidate_number" and self.is_rapid_release_scheme:
+            del bump_kwargs["release_candidate_number"]
 
-        bump_kwargs['is_nightly'] = self.is_nightly
-        bump_kwargs['is_aurora_or_devedition'] = self.is_aurora_or_devedition
-        bump_kwargs['is_esr'] = self.is_esr
+        bump_kwargs["is_nightly"] = self.is_nightly
+        bump_kwargs["is_aurora_or_devedition"] = self.is_aurora_or_devedition
+        bump_kwargs["is_esr"] = self.is_esr
 
         return bump_kwargs
 
     def bump_version_type(self):
         """Bump version type to the next one.
 
         Returns:
-            A new GeckoVersion with the version type set to the next one. Builds numbers are reset,
-            if originally set.
+            A new GeckoVersion with the version type set to the next one. Builds numbers
+            are reset, if originally set.
 
             For instance:
              * 32.0a1 is bumped to 32.0b1
              * 32.0bX is bumped to 32.0
              * 32.0 is bumped to 32.0esr
              * 31.0build1 is bumped to 31.0esrbuild1
              * 31.0build2 is bumped to 31.0esrbuild1
 
         """
         try:
             return self.__class__(**self._create_bump_version_type_kwargs())
         except (ValueError, PatternNotMatchedError) as e:
             raise ValueError(
-                'Cannot bump version type for version "{}". New version number is not valid. '
-                'Cause: {}'.format(self, e)
+                f'Cannot bump version type for version "{self}". New version number is '
+                f"not valid. Cause: {e}"
             ) from e
 
     def _create_bump_version_type_kwargs(self):
         bump_version_type_kwargs = {
-            'major_number': self.major_number,
-            'minor_number': self.minor_number,
-            'patch_number': self.patch_number,
+            "major_number": self.major_number,
+            "minor_number": self.minor_number,
+            "patch_number": self.patch_number,
         }
 
-        if self.is_nightly and self.major_number <= self._LAST_AURORA_DEVEDITION_AS_VERSION_TYPE:
-            bump_version_type_kwargs['is_aurora_or_devedition'] = True
+        if (
+            self.is_nightly
+            and self.major_number <= self._LAST_AURORA_DEVEDITION_AS_VERSION_TYPE
+        ):
+            bump_version_type_kwargs["is_aurora_or_devedition"] = True
         elif (
-            self.is_nightly and self.major_number > self._LAST_AURORA_DEVEDITION_AS_VERSION_TYPE or
-            self.is_aurora_or_devedition
+            self.is_nightly
+            and self.major_number > self._LAST_AURORA_DEVEDITION_AS_VERSION_TYPE
+            or self.is_aurora_or_devedition
         ):
-            bump_version_type_kwargs['beta_number'] = 1
+            bump_version_type_kwargs["beta_number"] = 1
         elif self.is_beta and not self.is_rapid_release_scheme:
-            bump_version_type_kwargs['release_candidate_number'] = 1
+            bump_version_type_kwargs["release_candidate_number"] = 1
         elif self.is_release:
-            bump_version_type_kwargs['is_esr'] = True
+            bump_version_type_kwargs["is_esr"] = True
         elif self.is_esr:
-            raise ValueError('There is no higher version type than ESR.')
+            raise ValueError("There is no higher version type than ESR.")
 
         if self.build_number is not None:
-            bump_version_type_kwargs['build_number'] = 1
+            bump_version_type_kwargs["build_number"] = 1
 
         return bump_version_type_kwargs
 
 
 class _VersionWithEdgeCases(GeckoVersion):
     def __attrs_post_init__(self):
         for edge_case in self._RELEASED_EDGE_CASES:
@@ -521,279 +614,326 @@
 
         return super().is_major
 
     def _do_all_numbers_match(self, edge_case):
         conditions = [
             getattr(self, number_type) == edge_case.get(number_type, None)
             for number_type in self._ALL_NUMBERS
-            if number_type != 'build_number'
+            if number_type != "build_number"
         ]
-        conditions.extend([
-            getattr(self, boolean_attribute, False) == edge_case.get(boolean_attribute, False)
-            for boolean_attribute in self._BOOLEANS_NOT_INFERRED_BY_NUMBERS
-        ])
+        conditions.extend(
+            [
+                getattr(self, boolean_attribute, False)
+                == edge_case.get(boolean_attribute, False)
+                for boolean_attribute in self._BOOLEANS_NOT_INFERRED_BY_NUMBERS
+            ]
+        )
 
         if all(conditions):
             if self.build_number is None:
                 return True
-            elif self.build_number == edge_case.get('build_number', None):
+            if self.build_number == edge_case.get("build_number", None):
                 return True
 
         return False
 
 
 class FirefoxVersion(_VersionWithEdgeCases):
     """Class that validates and handles Firefox version numbers."""
 
-    _RELEASED_EDGE_CASES = ({
-        'major_number': 1,
-        'minor_number': 5,
-        'patch_number': 0,
-        'old_fourth_number': 1,
-        'release_candidate_number': 1,
-    }, {
-        'major_number': 33,
-        'minor_number': 1,
-        'build_number': 1,
-    }, {
-        'major_number': 33,
-        'minor_number': 1,
-        'build_number': 2,
-    }, {
-        'major_number': 33,
-        'minor_number': 1,
-        'build_number': 3,
-    }, {
-        'major_number': 38,
-        'minor_number': 0,
-        'patch_number': 5,
-        'beta_number': 1,
-        'build_number': 1,
-    }, {
-        'major_number': 38,
-        'minor_number': 0,
-        'patch_number': 5,
-        'beta_number': 1,
-        'build_number': 2,
-    }, {
-        'major_number': 38,
-        'minor_number': 0,
-        'patch_number': 5,
-        'beta_number': 2,
-        'build_number': 1,
-    }, {
-        'major_number': 38,
-        'minor_number': 0,
-        'patch_number': 5,
-        'beta_number': 3,
-        'build_number': 1,
-    })
-
-    _RELEASED_EDGE_CASES_MAJOR = ({
-        'major_number': 1,
-        'minor_number': 5,
-    }, {
-        'major_number': 3,
-        'minor_number': 5,
-    }, {
-        'major_number': 3,
-        'minor_number': 6,
-    }, {
-        'major_number': 14,
-        'minor_number': 0,
-        'patch_number': 1,
-        'build_number': 1,
-    }, {
-        'major_number': 33,
-        'minor_number': 1,
-        'build_number': 1,
-    }, {
-        'major_number': 33,
-        'minor_number': 1,
-        'build_number': 2,
-    }, {
-        'major_number': 33,
-        'minor_number': 1,
-        'build_number': 3,
-    }, {
-        'major_number': 125,
-        'minor_number': 0,
-        'patch_number': 1,
-        'build_number': 1,
-    })
+    _RELEASED_EDGE_CASES = (
+        {
+            "major_number": 1,
+            "minor_number": 5,
+            "patch_number": 0,
+            "old_fourth_number": 1,
+            "release_candidate_number": 1,
+        },
+        {
+            "major_number": 33,
+            "minor_number": 1,
+            "build_number": 1,
+        },
+        {
+            "major_number": 33,
+            "minor_number": 1,
+            "build_number": 2,
+        },
+        {
+            "major_number": 33,
+            "minor_number": 1,
+            "build_number": 3,
+        },
+        {
+            "major_number": 38,
+            "minor_number": 0,
+            "patch_number": 5,
+            "beta_number": 1,
+            "build_number": 1,
+        },
+        {
+            "major_number": 38,
+            "minor_number": 0,
+            "patch_number": 5,
+            "beta_number": 1,
+            "build_number": 2,
+        },
+        {
+            "major_number": 38,
+            "minor_number": 0,
+            "patch_number": 5,
+            "beta_number": 2,
+            "build_number": 1,
+        },
+        {
+            "major_number": 38,
+            "minor_number": 0,
+            "patch_number": 5,
+            "beta_number": 3,
+            "build_number": 1,
+        },
+    )
+
+    _RELEASED_EDGE_CASES_MAJOR = (
+        {
+            "major_number": 1,
+            "minor_number": 5,
+        },
+        {
+            "major_number": 3,
+            "minor_number": 5,
+        },
+        {
+            "major_number": 3,
+            "minor_number": 6,
+        },
+        {
+            "major_number": 14,
+            "minor_number": 0,
+            "patch_number": 1,
+            "build_number": 1,
+        },
+        {
+            "major_number": 33,
+            "minor_number": 1,
+            "build_number": 1,
+        },
+        {
+            "major_number": 33,
+            "minor_number": 1,
+            "build_number": 2,
+        },
+        {
+            "major_number": 33,
+            "minor_number": 1,
+            "build_number": 3,
+        },
+        {
+            "major_number": 125,
+            "minor_number": 0,
+            "patch_number": 1,
+            "build_number": 1,
+        },
+    )
 
 
 class DeveditionVersion(GeckoVersion):
-    """Class that validates and handles Devedition after it became an equivalent to beta."""
+    """Class that validates and handles Devedition after it shipped alongside beta."""
 
     # No edge case were shipped
 
     def _get_all_error_messages_for_attributes(self):
         """Ensure attributes are sane all together."""
         error_messages = super()._get_all_error_messages_for_attributes()
 
         if (
-            (not self.is_beta) or
-            (self.major_number < 54) or
-            (self.major_number == 54 and self.beta_number < 11)
+            (not self.is_beta)
+            or (self.major_number < 54)
+            or (self.major_number == 54 and self.beta_number < 11)
         ):
-            error_messages.append('Devedition as a product must be a beta >= 54.0b11')
+            error_messages.append("Devedition as a product must be a beta >= 54.0b11")
 
         return error_messages
 
 
 class FennecVersion(_VersionWithEdgeCases):
     """Class that validates and handles Fennec (Firefox for Android) version numbers."""
 
-    _RELEASED_EDGE_CASES = ({
-        'major_number': 33,
-        'minor_number': 1,
-        'build_number': 1,
-    }, {
-        'major_number': 33,
-        'minor_number': 1,
-        'build_number': 2,
-    }, {
-        'major_number': 38,
-        'minor_number': 0,
-        'patch_number': 5,
-        'beta_number': 4,
-        'build_number': 1,
-    })
-
-    _RELEASED_EDGE_CASES_MAJOR = ({
-        'major_number': 1,
-        'minor_number': 1,
-    }, {
-        'major_number': 14,
-        'minor_number': 0,
-        'patch_number': 1,
-    }, {
-        'major_number': 33,
-        'minor_number': 1,
-        'build_number': 1,
-    }, {
-        'major_number': 68,
-        'minor_number': 1,
-        'build_number': 1,
-    })
+    _RELEASED_EDGE_CASES = (
+        {
+            "major_number": 33,
+            "minor_number": 1,
+            "build_number": 1,
+        },
+        {
+            "major_number": 33,
+            "minor_number": 1,
+            "build_number": 2,
+        },
+        {
+            "major_number": 38,
+            "minor_number": 0,
+            "patch_number": 5,
+            "beta_number": 4,
+            "build_number": 1,
+        },
+    )
+
+    _RELEASED_EDGE_CASES_MAJOR = (
+        {
+            "major_number": 1,
+            "minor_number": 1,
+        },
+        {
+            "major_number": 14,
+            "minor_number": 0,
+            "patch_number": 1,
+        },
+        {
+            "major_number": 33,
+            "minor_number": 1,
+            "build_number": 1,
+        },
+        {
+            "major_number": 68,
+            "minor_number": 1,
+            "build_number": 1,
+        },
+    )
 
     _LAST_FENNEC_VERSION = 68
 
     def __attrs_post_init__(self):
         """Ensure attributes are sane all together."""
-        # Versions matching 68.Xa1, 68.XbN, or simply 68.X are expected since bug 1523402. The
-        # latter is needed because of the version.txt of beta
+        # Versions matching 68.Xa1, 68.XbN, or simply 68.X are expected since
+        # bug 1523402. The latter is needed because of the version.txt of beta
         if (
-            self.major_number == self._LAST_FENNEC_VERSION and
-            self.minor_number > 0 and
-            self.patch_number is None
+            self.major_number == self._LAST_FENNEC_VERSION
+            and self.minor_number > 0
+            and self.patch_number is None
         ):
             return
 
         super().__attrs_post_init__()
 
     def _get_all_error_messages_for_attributes(self):
         error_messages = super()._get_all_error_messages_for_attributes()
         if self.major_number > self._LAST_FENNEC_VERSION:
-            error_messages.append(f'Last Fennec version is {self._LAST_FENNEC_VERSION}')
+            error_messages.append(f"Last Fennec version is {self._LAST_FENNEC_VERSION}")
 
         return error_messages
 
     def _create_bump_kwargs(self, field):
         kwargs = super()._create_bump_kwargs(field)
 
         if (
-            field != 'patch_number' and
-            kwargs['major_number'] == self._LAST_FENNEC_VERSION and
-            (kwargs['is_nightly'] or kwargs.get('beta_number'))
+            field != "patch_number"
+            and kwargs["major_number"] == self._LAST_FENNEC_VERSION
+            and (kwargs["is_nightly"] or kwargs.get("beta_number"))
         ):
-            del kwargs['patch_number']
+            del kwargs["patch_number"]
 
         return kwargs
 
 
 class ThunderbirdVersion(_VersionWithEdgeCases):
     """Class that validates and handles Thunderbird version numbers."""
 
-    _RELEASED_EDGE_CASES = ({
-        'major_number': 1,
-        'minor_number': 5,
-        'beta_number': 1,
-    }, {
-        'major_number': 1,
-        'minor_number': 5,
-        'beta_number': 2,
-    }, {
-        'major_number': 3,
-        'minor_number': 1,
-        'beta_number': 1,
-    }, {
-        'major_number': 3,
-        'minor_number': 1,
-    }, {
-        'major_number': 45,
-        'minor_number': 1,
-        'beta_number': 1,
-        'build_number': 1,
-    }, {
-        'major_number': 45,
-        'minor_number': 2,
-        'build_number': 1,
-    }, {
-        'major_number': 45,
-        'minor_number': 2,
-        'build_number': 2,
-    }, {
-        'major_number': 45,
-        'minor_number': 2,
-        'beta_number': 1,
-        'build_number': 2,
-    })
-
-    _RELEASED_EDGE_CASES_MAJOR = ({
-        'major_number': 1,
-        'minor_number': 5,
-    }, {
-        'major_number': 3,
-        'minor_number': 1,
-    }, {
-        'major_number': 38,
-        'minor_number': 0,
-        'patch_number': 1,
-        'build_number': 1,
-    })
+    _RELEASED_EDGE_CASES = (
+        {
+            "major_number": 1,
+            "minor_number": 5,
+            "beta_number": 1,
+        },
+        {
+            "major_number": 1,
+            "minor_number": 5,
+            "beta_number": 2,
+        },
+        {
+            "major_number": 3,
+            "minor_number": 1,
+            "beta_number": 1,
+        },
+        {
+            "major_number": 3,
+            "minor_number": 1,
+        },
+        {
+            "major_number": 45,
+            "minor_number": 1,
+            "beta_number": 1,
+            "build_number": 1,
+        },
+        {
+            "major_number": 45,
+            "minor_number": 2,
+            "build_number": 1,
+        },
+        {
+            "major_number": 45,
+            "minor_number": 2,
+            "build_number": 2,
+        },
+        {
+            "major_number": 45,
+            "minor_number": 2,
+            "beta_number": 1,
+            "build_number": 2,
+        },
+    )
+
+    _RELEASED_EDGE_CASES_MAJOR = (
+        {
+            "major_number": 1,
+            "minor_number": 5,
+        },
+        {
+            "major_number": 3,
+            "minor_number": 1,
+        },
+        {
+            "major_number": 38,
+            "minor_number": 0,
+            "patch_number": 1,
+            "build_number": 1,
+        },
+    )
 
 
 class GeckoSnapVersion(GeckoVersion):
     """Class that validates and handles Gecko's Snap version numbers.
 
-    Snap is a Linux packaging format developped by Canonical. Valid numbers are like "63.0b7-1",
-    "1" stands for "build1". Release Engineering set this scheme at the beginning of Snap and now
-    we can't rename published snap to the regular pattern like "63.0b7-build1".
+    Snap is a Linux packaging format developed by Canonical. Valid numbers are like
+    "63.0b7-1", "1" stands for "build1". Release Engineering set this scheme at the
+    beginning of Snap and now we can't rename published snap to the regular pattern
+    like "63.0b7-build1".
     """
 
     # Our Snaps are recent enough to not list any edge case, yet.
 
     # Differences between this regex and the one in GeckoVersion:
     #   * no a2
     #   * no "build"
     #   * but mandatory dash and build number.
     # Example: 63.0b7-1
-    _VALID_ENOUGH_VERSION_PATTERN = re.compile(r"""
+    _VALID_ENOUGH_VERSION_PATTERN = re.compile(
+        r"""
         ^(?P<major_number>\d+)
         \.(?P<minor_number>\d+)
         (\.(?P<patch_number>\d+))?
         (
             (?P<is_nightly>a1)
             |b(?P<beta_number>\d+)
             |(?P<is_esr>esr)
         )?
-        -(?P<build_number>\d+)$""", re.VERBOSE)
+        -(?P<build_number>\d+)$""",
+        re.VERBOSE,
+    )
 
     def __str__(self):
         """Implement string representation.
 
         Returns format like "63.0b7-1"
         """
         string = super().__str__()
-        return string.replace('build', '-')
+        return string.replace("build", "-")
```

### Comparing `mozilla_version-3.0.0/mozilla_version/maven.py` & `mozilla-version-3.1.0/mozilla_version/maven.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 """Defines characteristics of a Maven version at Mozilla."""
 
-import attr
 import re
 
+import attr
+
 from mozilla_version.version import BaseVersion
 
 
 @attr.s(frozen=True, eq=False, hash=True)
 class MavenVersion(BaseVersion):
     """Class that validates and handles Maven version numbers.
 
-    At Mozilla, Maven packages are used in projects like "GeckoView" or "Android-Components".
+    At Mozilla, Maven packages are used in projects like "GeckoView" or
+    "Android-Components".
     """
 
     is_snapshot = attr.ib(type=bool, default=False)
     is_beta = attr.ib(type=bool, default=False, init=False)
     is_release_candidate = attr.ib(type=bool, default=False, init=False)
 
-    _VALID_ENOUGH_VERSION_PATTERN = re.compile(r"""
+    _VALID_ENOUGH_VERSION_PATTERN = re.compile(
+        r"""
         ^(?P<major_number>\d+)
         \.(?P<minor_number>\d+)
         (\.(?P<patch_number>\d+))?
-        (?P<is_snapshot>-SNAPSHOT)?$""", re.VERBOSE)
+        (?P<is_snapshot>-SNAPSHOT)?$""",
+        re.VERBOSE,
+    )
 
     @classmethod
     def parse(cls, version_string):
         """Construct an object representing a valid Maven version number."""
-        return super().parse(version_string, regex_groups=('is_snapshot', ))
+        return super().parse(version_string, regex_groups=("is_snapshot",))
 
     def __str__(self):
         """Implement string representation.
 
         Computes a new string based on the given attributes.
         """
         string = super().__str__()
 
         if self.is_snapshot:
-            string = f'{string}-SNAPSHOT'
+            string = f"{string}-SNAPSHOT"
 
         return string
 
     def _compare(self, other):
         if isinstance(other, str):
             other = MavenVersion.parse(other)
-        elif not isinstance(other, MavenVersion):
+        if not isinstance(other, MavenVersion):
             raise ValueError(f'Cannot compare "{other}", type not supported!')
 
         difference = super()._compare(other)
         if difference != 0:
             return difference
 
         if not self.is_snapshot and other.is_snapshot:
             return 1
-        elif self.is_snapshot and not other.is_snapshot:
+        if self.is_snapshot and not other.is_snapshot:
             return -1
-        else:
-            return 0
+        return 0
 
     @property
     def is_release(self):
         """Return `True` if the others are both False."""
-        return not any((
-            self.is_beta, self.is_release_candidate, self.is_snapshot
-        ))
+        return not any((self.is_beta, self.is_release_candidate, self.is_snapshot))
```

### Comparing `mozilla_version-3.0.0/mozilla_version/parser.py` & `mozilla-version-3.1.0/mozilla_version/parser.py`

 * *Files identical despite different names*

### Comparing `mozilla_version-3.0.0/mozilla_version/test/integration/test_product_details.py` & `mozilla-version-3.1.0/mozilla_version/test/integration/test_product_details.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import pytest
 import requests
-from mozilla_version.test.integration import skip_network_tests_by_default
 
 from mozilla_version import (
     DeveditionVersion,
-    MobileVersion,
     FirefoxVersion,
-    ThunderbirdVersion
+    MobileVersion,
+    ThunderbirdVersion,
 )
 from mozilla_version.gecko import FennecVersion
-
+from mozilla_version.test.integration import skip_network_tests_by_default
 
 _VERSION_CLASS_PER_PRODUCT = {
     "devedition": DeveditionVersion,
     "fenix": MobileVersion,
     "fennec": FennecVersion,
     "firefox": FirefoxVersion,
-    "thunderbird": ThunderbirdVersion
+    "thunderbird": ThunderbirdVersion,
 }
 
 
 def _fetch_product_details():
     url = "https://product-details.mozilla.org/1.0/all.json"
     response = requests.get(url)
     if response.status_code == 200:
         return response.json()
-    else:
-        raise RuntimeError("Failed to fetch testing data")
+    raise RuntimeError("Failed to fetch testing data")
 
 
 def get_all_shipped_versions():
     product_details_data = _fetch_product_details()
     all_releases = product_details_data["releases"].keys()
-    all_products_and_versions = ((release.split("-")[0], "-".join(release.split("-")[1:])) for release in all_releases)
-    all_version_classes_and_versions = ((_VERSION_CLASS_PER_PRODUCT[product.lower()], version) for product, version in all_products_and_versions)
-    return all_version_classes_and_versions
+    all_products_and_versions = (
+        (release.split("-")[0], "-".join(release.split("-")[1:]))
+        for release in all_releases
+    )
+    return (
+        (_VERSION_CLASS_PER_PRODUCT[product.lower()], version)
+        for product, version in all_products_and_versions
+    )
 
 
 @skip_network_tests_by_default
-@pytest.mark.parametrize("VersionClass, version", get_all_shipped_versions())
-def test_parse_all_shipped_version_in_product_details(VersionClass, version):
-    VersionClass.parse(version)
+@pytest.mark.parametrize("version_class, version", get_all_shipped_versions())
+def test_parse_all_shipped_version_in_product_details(version_class, version):
+    version_class.parse(version)
```

### Comparing `mozilla_version-3.0.0/mozilla_version/test/test_balrog.py` & `mozilla-version-3.1.0/mozilla_version/test/test_balrog.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,171 +2,274 @@
 
 from mozilla_version.balrog import BalrogReleaseName
 from mozilla_version.errors import PatternNotMatchedError
 from mozilla_version.gecko import FirefoxVersion
 
 
 @pytest.mark.parametrize(
-    'product, major_number, minor_number, patch_number, beta_number, build_number, is_nightly, \
-is_aurora_or_devedition, is_esr, expected_output_string', ((
-    'firefox', 31, 0, None, None, 7, False, False, True, 'firefox-31.0esr-build7'
-), (
-    'firefox', 31, 0, 1, None, 8, False, False, True, 'firefox-31.0.1esr-build8'
-), (
-    'firefox', 32, 0, None, None, 1, False, False, False, 'firefox-32.0-build1'
-), (
-    'firefox', 32, 0, 1, None, 2, False, False, False, 'firefox-32.0.1-build2'
-), (
-    'firefox', 32, 0, None, 3, 4, False, False, False, 'firefox-32.0b3-build4'
-), (
-    'firefox', 32, 0, None, None, 5, True, False, False, 'firefox-32.0a1-build5'
-), (
-    'firefox', 32, 0, None, None, 6, False, True, False, 'firefox-32.0a2-build6'
-), (
-    'devedition', 54, 0, None, 12, 1, False, False, False, 'devedition-54.0b12-build1'
-), (
-    'fennec', 32, 0, None, None, 1, False, False, False, 'fennec-32.0-build1'
-), (
-    'thunderbird', 32, 0, None, None, 1, False, False, False, 'thunderbird-32.0-build1'
-)))
+    "product, major_number, minor_number, patch_number, beta_number, build_number, \
+is_nightly, is_aurora_or_devedition, is_esr, expected_output_string",
+    (
+        ("firefox", 31, 0, None, None, 7, False, False, True, "firefox-31.0esr-build7"),
+        ("firefox", 31, 0, 1, None, 8, False, False, True, "firefox-31.0.1esr-build8"),
+        ("firefox", 32, 0, None, None, 1, False, False, False, "firefox-32.0-build1"),
+        ("firefox", 32, 0, 1, None, 2, False, False, False, "firefox-32.0.1-build2"),
+        ("firefox", 32, 0, None, 3, 4, False, False, False, "firefox-32.0b3-build4"),
+        ("firefox", 32, 0, None, None, 5, True, False, False, "firefox-32.0a1-build5"),
+        ("firefox", 32, 0, None, None, 6, False, True, False, "firefox-32.0a2-build6"),
+        (
+            "devedition",
+            54,
+            0,
+            None,
+            12,
+            1,
+            False,
+            False,
+            False,
+            "devedition-54.0b12-build1",
+        ),
+        ("fennec", 32, 0, None, None, 1, False, False, False, "fennec-32.0-build1"),
+        (
+            "thunderbird",
+            32,
+            0,
+            None,
+            None,
+            1,
+            False,
+            False,
+            False,
+            "thunderbird-32.0-build1",
+        ),
+    ),
+)
 def test_balrog_release_name_constructor_and_str(
-    product, major_number, minor_number, patch_number, beta_number, build_number, is_nightly,
-    is_aurora_or_devedition, is_esr, expected_output_string
+    product,
+    major_number,
+    minor_number,
+    patch_number,
+    beta_number,
+    build_number,
+    is_nightly,
+    is_aurora_or_devedition,
+    is_esr,
+    expected_output_string,
 ):
-    assert str(BalrogReleaseName(product, FirefoxVersion(
-        major_number=major_number,
-        minor_number=minor_number,
-        patch_number=patch_number,
-        build_number=build_number,
-        beta_number=beta_number,
-        is_nightly=is_nightly,
-        is_aurora_or_devedition=is_aurora_or_devedition,
-        is_esr=is_esr
-    ))) == expected_output_string
-
-
-@pytest.mark.parametrize('product, major_number, minor_number, patch_number, beta_number, build_number, is_nightly, is_aurora_or_devedition, is_esr, ExpectedErrorType', ((
-    ('nonexistingproduct', 32, 0, None, None, 1, False, False, False, PatternNotMatchedError),
-    ('firefox', 32, 0, None, None, None, False, False, False, PatternNotMatchedError),
-)))
-def test_fail_balrog_release_constructor(product, major_number, minor_number, patch_number, beta_number, build_number, is_nightly, is_aurora_or_devedition, is_esr, ExpectedErrorType):
-    with pytest.raises(ExpectedErrorType):
-        BalrogReleaseName(product, FirefoxVersion(
-            major_number=major_number,
-            minor_number=minor_number,
-            patch_number=patch_number,
-            beta_number=beta_number,
-            build_number=build_number,
-            is_nightly=is_nightly,
-            is_aurora_or_devedition=is_aurora_or_devedition,
-            is_esr=is_esr
-        ))
-
-
-@pytest.mark.parametrize('string, expected_string', ((
-    ('firefox-31.0esr-build7', 'firefox-31.0esr-build7'),
-    ('firefox-31.0.1esr-build8', 'firefox-31.0.1esr-build8'),
-
-    ('firefox-32.0-build1', 'firefox-32.0-build1'),
-    ('firefox-32.0.1-build2', 'firefox-32.0.1-build2'),
-    ('firefox-32.0b3-build4', 'firefox-32.0b3-build4'),
-    ('firefox-32.0a1-build5', 'firefox-32.0a1-build5'),
-    ('firefox-32.0a2-build6', 'firefox-32.0a2-build6'),
-    ('firefox-32.0build1', 'firefox-32.0-build1'),
-)))
+    assert (
+        str(
+            BalrogReleaseName(
+                product,
+                FirefoxVersion(
+                    major_number=major_number,
+                    minor_number=minor_number,
+                    patch_number=patch_number,
+                    build_number=build_number,
+                    beta_number=beta_number,
+                    is_nightly=is_nightly,
+                    is_aurora_or_devedition=is_aurora_or_devedition,
+                    is_esr=is_esr,
+                ),
+            )
+        )
+        == expected_output_string
+    )
+
+
+@pytest.mark.parametrize(
+    "product, major_number, minor_number, patch_number, beta_number, build_number, \
+is_nightly, is_aurora_or_devedition, is_esr, expected_error_type",
+    (
+        (
+            (
+                "nonexistingproduct",
+                32,
+                0,
+                None,
+                None,
+                1,
+                False,
+                False,
+                False,
+                PatternNotMatchedError,
+            ),
+            (
+                "firefox",
+                32,
+                0,
+                None,
+                None,
+                None,
+                False,
+                False,
+                False,
+                PatternNotMatchedError,
+            ),
+        )
+    ),
+)
+def test_fail_balrog_release_constructor(
+    product,
+    major_number,
+    minor_number,
+    patch_number,
+    beta_number,
+    build_number,
+    is_nightly,
+    is_aurora_or_devedition,
+    is_esr,
+    expected_error_type,
+):
+    with pytest.raises(expected_error_type):
+        BalrogReleaseName(
+            product,
+            FirefoxVersion(
+                major_number=major_number,
+                minor_number=minor_number,
+                patch_number=patch_number,
+                beta_number=beta_number,
+                build_number=build_number,
+                is_nightly=is_nightly,
+                is_aurora_or_devedition=is_aurora_or_devedition,
+                is_esr=is_esr,
+            ),
+        )
+
+
+@pytest.mark.parametrize(
+    "string, expected_string",
+    (
+        (
+            ("firefox-31.0esr-build7", "firefox-31.0esr-build7"),
+            ("firefox-31.0.1esr-build8", "firefox-31.0.1esr-build8"),
+            ("firefox-32.0-build1", "firefox-32.0-build1"),
+            ("firefox-32.0.1-build2", "firefox-32.0.1-build2"),
+            ("firefox-32.0b3-build4", "firefox-32.0b3-build4"),
+            ("firefox-32.0a1-build5", "firefox-32.0a1-build5"),
+            ("firefox-32.0a2-build6", "firefox-32.0a2-build6"),
+            ("firefox-32.0build1", "firefox-32.0-build1"),
+        )
+    ),
+)
 def test_balrog_release_name_parse(string, expected_string):
     assert str(BalrogReleaseName.parse(string)) == expected_string
 
 
-@pytest.mark.parametrize('string, ExpectedErrorType', (
-    ('firefox-32.0', PatternNotMatchedError),
-
-    ('firefox32.0-build1', PatternNotMatchedError),
-    ('firefox32.0build1', PatternNotMatchedError),
-    ('firefox-32.0--build1', PatternNotMatchedError),
-    ('firefox-build1', PatternNotMatchedError),
-    ('nonexistingproduct-32.0-build1', PatternNotMatchedError),
-
-    ('firefox-32-build1', PatternNotMatchedError),
-    ('firefox-32.b2-build1', PatternNotMatchedError),
-    ('firefox-.1-build1', PatternNotMatchedError),
-    ('firefox-32.0.0-build1', PatternNotMatchedError),
-    ('firefox-32.2-build1', PatternNotMatchedError),
-    ('firefox-32.02-build1', PatternNotMatchedError),
-    ('firefox-32.0a0-build1', ValueError),
-    ('firefox-32.0b0-build1', ValueError),
-    ('firefox-32.0.1a1-build1', PatternNotMatchedError),
-    ('firefox-32.0.1a2-build1', PatternNotMatchedError),
-    ('firefox-32.0.1b2-build1', PatternNotMatchedError),
-    ('firefox-32.0-build0', ValueError),
-    ('firefox-32.0a1a2-build1', PatternNotMatchedError),
-    ('firefox-32.0a1b2-build1', PatternNotMatchedError),
-    ('firefox-32.0b2esr-build1', PatternNotMatchedError),
-    ('firefox-32.0esrb2-build1', PatternNotMatchedError),
-))
-def test_firefox_version_raises_when_invalid_version_is_given(string, ExpectedErrorType):
-    with pytest.raises(ExpectedErrorType):
+@pytest.mark.parametrize(
+    "string, expected_error_type",
+    (
+        ("firefox-32.0", PatternNotMatchedError),
+        ("firefox32.0-build1", PatternNotMatchedError),
+        ("firefox32.0build1", PatternNotMatchedError),
+        ("firefox-32.0--build1", PatternNotMatchedError),
+        ("firefox-build1", PatternNotMatchedError),
+        ("nonexistingproduct-32.0-build1", PatternNotMatchedError),
+        ("firefox-32-build1", PatternNotMatchedError),
+        ("firefox-32.b2-build1", PatternNotMatchedError),
+        ("firefox-.1-build1", PatternNotMatchedError),
+        ("firefox-32.0.0-build1", PatternNotMatchedError),
+        ("firefox-32.2-build1", PatternNotMatchedError),
+        ("firefox-32.02-build1", PatternNotMatchedError),
+        ("firefox-32.0a0-build1", ValueError),
+        ("firefox-32.0b0-build1", ValueError),
+        ("firefox-32.0.1a1-build1", PatternNotMatchedError),
+        ("firefox-32.0.1a2-build1", PatternNotMatchedError),
+        ("firefox-32.0.1b2-build1", PatternNotMatchedError),
+        ("firefox-32.0-build0", ValueError),
+        ("firefox-32.0a1a2-build1", PatternNotMatchedError),
+        ("firefox-32.0a1b2-build1", PatternNotMatchedError),
+        ("firefox-32.0b2esr-build1", PatternNotMatchedError),
+        ("firefox-32.0esrb2-build1", PatternNotMatchedError),
+    ),
+)
+def test_firefox_version_raises_when_invalid_version_is_given(
+    string, expected_error_type
+):
+    with pytest.raises(expected_error_type):
         BalrogReleaseName.parse(string)
 
 
-@pytest.mark.parametrize('previous, next', (
-    ('firefox-32.0-build1', 'firefox-33.0-build1'),
-    ('firefox-32.0-build1', 'firefox-32.1.0-build1'),
-    ('firefox-32.0-build1', 'firefox-32.0.1-build1'),
-    ('firefox-32.0-build1', 'firefox-32.0-build2'),
-
-    ('firefox-32.0a1-build1', 'firefox-32.0-build1'),
-    ('firefox-32.0a2-build1', 'firefox-32.0-build1'),
-    ('firefox-32.0b1-build1', 'firefox-32.0-build1'),
-
-    ('firefox-32.0.1-build1', 'firefox-33.0-build1'),
-    ('firefox-32.0.1-build1', 'firefox-32.1.0-build1'),
-    ('firefox-32.0.1-build1', 'firefox-32.0.2-build1'),
-    ('firefox-32.0.1-build1', 'firefox-32.0.1-build2'),
-
-    ('firefox-32.1.0-build1', 'firefox-33.0-build1'),
-    ('firefox-32.1.0-build1', 'firefox-32.2.0-build1'),
-    ('firefox-32.1.0-build1', 'firefox-32.1.1-build1'),
-    ('firefox-32.1.0-build1', 'firefox-32.1.0-build2'),
-
-    ('firefox-32.0b1-build1', 'firefox-33.0b1-build1'),
-    ('firefox-32.0b1-build1', 'firefox-32.0b2-build1'),
-    ('firefox-32.0b1-build1', 'firefox-32.0b1-build2'),
-
-    ('firefox-2.0-build1', 'firefox-10.0-build1'),
-    ('firefox-10.2.0-build1', 'firefox-10.10.0-build1'),
-    ('firefox-10.0.2-build1', 'firefox-10.0.10-build1'),
-    ('firefox-10.10.1-build1', 'firefox-10.10.10-build1'),
-    ('firefox-10.0-build2', 'firefox-10.0-build10'),
-    ('firefox-10.0b2-build1', 'firefox-10.0b10-build1'),
-))
-def test_balrog_release_implements_lt_operator(previous, next):
-    assert BalrogReleaseName.parse(previous) < BalrogReleaseName.parse(next)
+@pytest.mark.parametrize(
+    "previous_version, next_version",
+    (
+        ("firefox-32.0-build1", "firefox-33.0-build1"),
+        ("firefox-32.0-build1", "firefox-32.1.0-build1"),
+        ("firefox-32.0-build1", "firefox-32.0.1-build1"),
+        ("firefox-32.0-build1", "firefox-32.0-build2"),
+        ("firefox-32.0a1-build1", "firefox-32.0-build1"),
+        ("firefox-32.0a2-build1", "firefox-32.0-build1"),
+        ("firefox-32.0b1-build1", "firefox-32.0-build1"),
+        ("firefox-32.0.1-build1", "firefox-33.0-build1"),
+        ("firefox-32.0.1-build1", "firefox-32.1.0-build1"),
+        ("firefox-32.0.1-build1", "firefox-32.0.2-build1"),
+        ("firefox-32.0.1-build1", "firefox-32.0.1-build2"),
+        ("firefox-32.1.0-build1", "firefox-33.0-build1"),
+        ("firefox-32.1.0-build1", "firefox-32.2.0-build1"),
+        ("firefox-32.1.0-build1", "firefox-32.1.1-build1"),
+        ("firefox-32.1.0-build1", "firefox-32.1.0-build2"),
+        ("firefox-32.0b1-build1", "firefox-33.0b1-build1"),
+        ("firefox-32.0b1-build1", "firefox-32.0b2-build1"),
+        ("firefox-32.0b1-build1", "firefox-32.0b1-build2"),
+        ("firefox-2.0-build1", "firefox-10.0-build1"),
+        ("firefox-10.2.0-build1", "firefox-10.10.0-build1"),
+        ("firefox-10.0.2-build1", "firefox-10.0.10-build1"),
+        ("firefox-10.10.1-build1", "firefox-10.10.10-build1"),
+        ("firefox-10.0-build2", "firefox-10.0-build10"),
+        ("firefox-10.0b2-build1", "firefox-10.0b10-build1"),
+    ),
+)
+def test_balrog_release_implements_lt_operator(previous_version, next_version):
+    assert BalrogReleaseName.parse(previous_version) < BalrogReleaseName.parse(
+        next_version
+    )
 
 
 def test_fail_balrog_release_lt_operator():
     with pytest.raises(ValueError):
-        assert BalrogReleaseName.parse('thunderbird-32.0-build1') < BalrogReleaseName.parse('Firefox-32.0-build2')
+        assert BalrogReleaseName.parse(
+            "thunderbird-32.0-build1"
+        ) < BalrogReleaseName.parse("Firefox-32.0-build2")
 
 
 def test_balrog_release_implements_remaining_comparision_operators():
-    assert BalrogReleaseName.parse('firefox-32.0-build1') == BalrogReleaseName.parse('firefox-32.0-build1')
-    assert BalrogReleaseName.parse('firefox-32.0-build1') != BalrogReleaseName.parse('firefox-33.0-build1')
-
-    assert BalrogReleaseName.parse('firefox-32.0-build1') <= BalrogReleaseName.parse('firefox-32.0-build1')
-    assert BalrogReleaseName.parse('firefox-32.0-build1') <= BalrogReleaseName.parse('firefox-33.0-build1')
-
-    assert BalrogReleaseName.parse('firefox-33.0-build1') >= BalrogReleaseName.parse('firefox-32.0-build1')
-    assert BalrogReleaseName.parse('firefox-33.0-build1') >= BalrogReleaseName.parse('firefox-33.0-build1')
-
-    assert BalrogReleaseName.parse('firefox-33.0-build1') > BalrogReleaseName.parse('firefox-32.0-build1')
-    assert not BalrogReleaseName.parse('firefox-33.0-build1') > BalrogReleaseName.parse('firefox-33.0-build1')
-
-    assert not BalrogReleaseName.parse('firefox-32.0-build1') < BalrogReleaseName.parse('firefox-32.0-build1')
+    assert BalrogReleaseName.parse("firefox-32.0-build1") == BalrogReleaseName.parse(
+        "firefox-32.0-build1"
+    )
+    assert BalrogReleaseName.parse("firefox-32.0-build1") != BalrogReleaseName.parse(
+        "firefox-33.0-build1"
+    )
+
+    assert BalrogReleaseName.parse("firefox-32.0-build1") <= BalrogReleaseName.parse(
+        "firefox-32.0-build1"
+    )
+    assert BalrogReleaseName.parse("firefox-32.0-build1") <= BalrogReleaseName.parse(
+        "firefox-33.0-build1"
+    )
+
+    assert BalrogReleaseName.parse("firefox-33.0-build1") >= BalrogReleaseName.parse(
+        "firefox-32.0-build1"
+    )
+    assert BalrogReleaseName.parse("firefox-33.0-build1") >= BalrogReleaseName.parse(
+        "firefox-33.0-build1"
+    )
+
+    assert BalrogReleaseName.parse("firefox-33.0-build1") > BalrogReleaseName.parse(
+        "firefox-32.0-build1"
+    )
+    assert not BalrogReleaseName.parse("firefox-33.0-build1") > BalrogReleaseName.parse(
+        "firefox-33.0-build1"
+    )
+
+    assert not BalrogReleaseName.parse("firefox-32.0-build1") < BalrogReleaseName.parse(
+        "firefox-32.0-build1"
+    )
+
+    assert BalrogReleaseName.parse("firefox-33.0-build1") != BalrogReleaseName.parse(
+        "firefox-32.0-build1"
+    )
 
-    assert BalrogReleaseName.parse('firefox-33.0-build1') != BalrogReleaseName.parse('firefox-32.0-build1')
 
 def test_balrog_release_hashable():
     """
     It is possible to hash `BalrogReleaseNmae`.
     """
-    hash(BalrogReleaseName.parse('firefox-63.0-build1'))
+    hash(BalrogReleaseName.parse("firefox-63.0-build1"))
```

### Comparing `mozilla_version-3.0.0/mozilla_version/test/test_maven.py` & `mozilla-version-3.1.0/mozilla_version/test/test_maven.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,128 @@
-import pytest
-
 from distutils.version import LooseVersion, StrictVersion
 
+import pytest
+
 from mozilla_version.errors import PatternNotMatchedError
 from mozilla_version.maven import MavenVersion
 
-@pytest.mark.parametrize('major_number, minor_number, patch_number, is_snapshot, expected_output_string', ((
-    32, 0, None, False, '32.0'
-), (
-    32, 0, 1, False, '32.0.1'
-), (
-    32, 0, None, True, '32.0-SNAPSHOT'
-), (
-    32, 0, 1, True, '32.0.1-SNAPSHOT'
-)))
-def test_maven_version_constructor_and_str(major_number, minor_number, patch_number, is_snapshot, expected_output_string):
-    assert str(MavenVersion(
-        major_number=major_number,
-        minor_number=minor_number,
-        patch_number=patch_number,
-        is_snapshot=is_snapshot,
-    )) == expected_output_string
 
-
-def test_maven_version_constructor_minimum_kwargs():
-    assert str(MavenVersion(32, 0)) == '32.0'
-    assert str(MavenVersion(32, 0, 1)) == '32.0.1'
-    assert str(MavenVersion(32, 1, 0)) == '32.1.0'
-    assert str(MavenVersion(32, 1, 0, False)) == '32.1.0'
-    assert str(MavenVersion(32, 1, 0, True)) == '32.1.0-SNAPSHOT'
+@pytest.mark.parametrize(
+    "major_number, minor_number, patch_number, is_snapshot, expected_output_string",
+    (
+        (32, 0, None, False, "32.0"),
+        (32, 0, 1, False, "32.0.1"),
+        (32, 0, None, True, "32.0-SNAPSHOT"),
+        (32, 0, 1, True, "32.0.1-SNAPSHOT"),
+    ),
+)
+def test_maven_version_constructor_and_str(
+    major_number, minor_number, patch_number, is_snapshot, expected_output_string
+):
+    assert (
+        str(
+            MavenVersion(
+                major_number=major_number,
+                minor_number=minor_number,
+                patch_number=patch_number,
+                is_snapshot=is_snapshot,
+            )
+        )
+        == expected_output_string
+    )
 
 
-@pytest.mark.parametrize('version_string, ExpectedErrorType', (
-    ('32.0SNAPSHOT', PatternNotMatchedError),
-    ('32.1.0SNAPSHOT', PatternNotMatchedError),
-))
-def test_maven_version_raises_when_invalid_version_is_given(version_string, ExpectedErrorType):
-    with pytest.raises(ExpectedErrorType):
+def test_maven_version_constructor_minimum_kwargs():
+    assert str(MavenVersion(32, 0)) == "32.0"
+    assert str(MavenVersion(32, 0, 1)) == "32.0.1"
+    assert str(MavenVersion(32, 1, 0)) == "32.1.0"
+    assert str(MavenVersion(32, 1, 0, False)) == "32.1.0"
+    assert str(MavenVersion(32, 1, 0, True)) == "32.1.0-SNAPSHOT"
+
+
+@pytest.mark.parametrize(
+    "version_string, expected_error_type",
+    (
+        ("32.0SNAPSHOT", PatternNotMatchedError),
+        ("32.1.0SNAPSHOT", PatternNotMatchedError),
+    ),
+)
+def test_maven_version_raises_when_invalid_version_is_given(
+    version_string, expected_error_type
+):
+    with pytest.raises(expected_error_type):
         MavenVersion.parse(version_string)
 
 
-@pytest.mark.parametrize('previous, next', (
-    ('32.0-SNAPSHOT', '32.0'),
-    ('31.0', '32.0-SNAPSHOT'),
-    ('32.0', '32.0.1-SNAPSHOT'),
-    ('32.0.1-SNAPSHOT', '32.1.0'),
-    ('32.0.1-SNAPSHOT', '33.0'),
-))
-def test_maven_version_implements_lt_operator(previous, next):
-    assert MavenVersion.parse(previous) < MavenVersion.parse(next)
-
-
-@pytest.mark.parametrize('previous, next', (
-    ('32.0', '32.0-SNAPSHOT'),
-    ('32.0-SNAPSHOT', '31.0'),
-    ('32.0.1-SNAPSHOT', '32.0'),
-    ('32.1.0', '32.0.1-SNAPSHOT'),
-))
-def test_maven_version_implements_gt_operator(previous, next):
-    assert MavenVersion.parse(previous) > MavenVersion.parse(next)
-
-
-@pytest.mark.parametrize('wrong_type', (
-    32,
-    32.0,
-    ('32', '0', '1'),
-    ['32', '0', '1'],
-    LooseVersion('32.0'),
-    StrictVersion('32.0'),
-))
+@pytest.mark.parametrize(
+    "previous_version, next_version",
+    (
+        ("32.0-SNAPSHOT", "32.0"),
+        ("31.0", "32.0-SNAPSHOT"),
+        ("32.0", "32.0.1-SNAPSHOT"),
+        ("32.0.1-SNAPSHOT", "32.1.0"),
+        ("32.0.1-SNAPSHOT", "33.0"),
+    ),
+)
+def test_maven_version_implements_lt_operator(previous_version, next_version):
+    assert MavenVersion.parse(previous_version) < MavenVersion.parse(next_version)
+
+
+@pytest.mark.parametrize(
+    "previous_version, next_version",
+    (
+        ("32.0", "32.0-SNAPSHOT"),
+        ("32.0-SNAPSHOT", "31.0"),
+        ("32.0.1-SNAPSHOT", "32.0"),
+        ("32.1.0", "32.0.1-SNAPSHOT"),
+    ),
+)
+def test_maven_version_implements_gt_operator(previous_version, next_version):
+    assert MavenVersion.parse(previous_version) > MavenVersion.parse(next_version)
+
+
+@pytest.mark.parametrize(
+    "wrong_type",
+    (
+        32,
+        32.0,
+        ("32", "0", "1"),
+        ["32", "0", "1"],
+        LooseVersion("32.0"),
+        StrictVersion("32.0"),
+    ),
+)
 def test_base_version_raises_eq_operator(wrong_type):
     with pytest.raises(ValueError):
-        assert MavenVersion.parse('32.0') == wrong_type
+        assert MavenVersion.parse("32.0") == wrong_type
     # AttributeError is raised by LooseVersion and StrictVersion
     with pytest.raises((ValueError, AttributeError)):
-        assert wrong_type == MavenVersion.parse('32.0')
+        assert wrong_type == MavenVersion.parse("32.0")
 
 
 def test_maven_version_implements_eq_operator():
-    assert MavenVersion.parse('32.0-SNAPSHOT') == MavenVersion.parse('32.0-SNAPSHOT')
+    assert MavenVersion.parse("32.0-SNAPSHOT") == MavenVersion.parse("32.0-SNAPSHOT")
     # raw strings are also converted
-    assert MavenVersion.parse('32.0-SNAPSHOT') == '32.0-SNAPSHOT'
+    assert MavenVersion.parse("32.0-SNAPSHOT") == "32.0-SNAPSHOT"
 
 
 def test_maven_version_hashable():
-    hash(MavenVersion.parse('32.0.1'))
+    hash(MavenVersion.parse("32.0.1"))
 
 
-@pytest.mark.parametrize('version_string, expected_type', (
-    ('32.0', 'release'),
-    ('32.0-SNAPSHOT', 'snapshot'),
-))
+@pytest.mark.parametrize(
+    "version_string, expected_type",
+    (
+        ("32.0", "release"),
+        ("32.0-SNAPSHOT", "snapshot"),
+    ),
+)
 def test_maven_version_is_of_a_defined_type(version_string, expected_type):
     release = MavenVersion.parse(version_string)
-    assert getattr(release, f'is_{expected_type}')
+    assert getattr(release, f"is_{expected_type}")
 
 
 def test_maven_version_are_never_of_certain_types():
     release = MavenVersion(32, 0)
     assert not release.is_beta
     assert not release.is_release_candidate
```

### Comparing `mozilla_version-3.0.0/mozilla_version/test/test_mobile.py` & `mozilla-version-3.1.0/mozilla_version/test/test_mobile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,355 +1,387 @@
-import pytest
 import re
+from distutils.version import LooseVersion, StrictVersion
 
-from distutils.version import StrictVersion, LooseVersion
+import pytest
 
 import mozilla_version.gecko
-
-from mozilla_version.errors import PatternNotMatchedError, TooManyTypesError, NoVersionTypeError
+from mozilla_version.errors import (
+    NoVersionTypeError,
+    PatternNotMatchedError,
+    TooManyTypesError,
+)
 from mozilla_version.mobile import MobileVersion
-from mozilla_version.test import does_not_raise
-
 
 VALID_VERSIONS = {
-    '0.3.0-rc.1': 'release_candidate',
-    '1.0.0': 'release',
-    '1.0.0-rc.1': 'release_candidate',
-    '1.0.0-rc.2': 'release_candidate',
-    '1.0.1': 'release',
-    '1.0.1-rc.1': 'release_candidate',
-    '1.1.0': 'release',
-    '1.1.0-rc.1': 'release_candidate',
-    '1.1.0-rc.2': 'release_candidate',
-    '1.2.0': 'release',
-    '1.2.0-rc.1': 'release_candidate',
-    '1.2.0-rc.2': 'release_candidate',
-    '1.3.0': 'release',
-    '1.3.0-rc.1': 'release_candidate',
-    '1.3.0-rc.2': 'release_candidate',
-    '1.3.0-rc.3': 'release_candidate',
-    '2.2.0-rc.1': 'release_candidate',
-    '3.0.0-beta.2': 'beta',
-    '3.0.0-beta.3': 'beta',
-    '3.0.0': 'release',
-
-    '104.0a1': 'nightly',
-    '104.0b2': 'beta',
-    '104.0': 'release',
-    '104.0.0': 'release',
-    '104.0.1': 'release',
-    '109.0': 'release',
+    "0.3.0-rc.1": "release_candidate",
+    "1.0.0": "release",
+    "1.0.0-rc.1": "release_candidate",
+    "1.0.0-rc.2": "release_candidate",
+    "1.0.1": "release",
+    "1.0.1-rc.1": "release_candidate",
+    "1.1.0": "release",
+    "1.1.0-rc.1": "release_candidate",
+    "1.1.0-rc.2": "release_candidate",
+    "1.2.0": "release",
+    "1.2.0-rc.1": "release_candidate",
+    "1.2.0-rc.2": "release_candidate",
+    "1.3.0": "release",
+    "1.3.0-rc.1": "release_candidate",
+    "1.3.0-rc.2": "release_candidate",
+    "1.3.0-rc.3": "release_candidate",
+    "2.2.0-rc.1": "release_candidate",
+    "3.0.0-beta.2": "beta",
+    "3.0.0-beta.3": "beta",
+    "3.0.0": "release",
+    "104.0a1": "nightly",
+    "104.0b2": "beta",
+    "104.0": "release",
+    "104.0.0": "release",
+    "104.0.1": "release",
+    "109.0": "release",
 }
 
 
-@pytest.mark.parametrize('major_number, minor_number, patch_number, beta_number, rc_number, expected_output_string', ((
-    3, 0, 0, None, None, '3.0.0'
-), (
-    3, 0, 1, None, None, '3.0.1'
-), (
-    3, 0, 0, 3, None, '3.0.0-beta.3'
-), (
-    103, 0, 0, 3, None, '103.0.0-beta.3'
-), (
-    104, 0, None, 3, None, '104.0b3'
-), (
-    3, 0, 0, None, 3, '3.0.0-rc.3'
-)))
-def test_mobile_version_constructor_and_str(major_number, minor_number, patch_number, beta_number, rc_number, expected_output_string):
-    assert str(MobileVersion(
-        major_number=major_number,
-        minor_number=minor_number,
-        patch_number=patch_number,
-        beta_number=beta_number,
-        release_candidate_number=rc_number,
-    )) == expected_output_string
-
-
-@pytest.mark.parametrize('major_number, minor_number, patch_number, beta_number, rc_number, ExpectedErrorType', ((
-    3, 0, 0, 1, 1, TooManyTypesError
-), (
-    3, 0, 0, 0, None, ValueError
-), (
-    3, 0, None, None, None, PatternNotMatchedError
-), (
-    3, 0, 0, None, 0, ValueError
-), (
-    -1, 0, 0, None, None, ValueError
-), (
-    3, -1, 0, None, None, ValueError
-), (
-    3, 0, -1, None, None, ValueError
-), (
-    2.2, 0, 0, None, None, ValueError
-), (
-    'some string', 0, 0, None, None, ValueError
-)))
-def test_fail_mobile_version_constructor(major_number, minor_number, patch_number, beta_number, rc_number, ExpectedErrorType):
-    with pytest.raises(ExpectedErrorType):
+@pytest.mark.parametrize(
+    "major_number, minor_number, patch_number, beta_number, rc_number, \
+expected_output_string",
+    (
+        (3, 0, 0, None, None, "3.0.0"),
+        (3, 0, 1, None, None, "3.0.1"),
+        (3, 0, 0, 3, None, "3.0.0-beta.3"),
+        (103, 0, 0, 3, None, "103.0.0-beta.3"),
+        (104, 0, None, 3, None, "104.0b3"),
+        (3, 0, 0, None, 3, "3.0.0-rc.3"),
+    ),
+)
+def test_mobile_version_constructor_and_str(
+    major_number,
+    minor_number,
+    patch_number,
+    beta_number,
+    rc_number,
+    expected_output_string,
+):
+    assert (
+        str(
+            MobileVersion(
+                major_number=major_number,
+                minor_number=minor_number,
+                patch_number=patch_number,
+                beta_number=beta_number,
+                release_candidate_number=rc_number,
+            )
+        )
+        == expected_output_string
+    )
+
+
+@pytest.mark.parametrize(
+    "major_number, minor_number, patch_number, beta_number, rc_number, \
+expected_error_type",
+    (
+        (3, 0, 0, 1, 1, TooManyTypesError),
+        (3, 0, 0, 0, None, ValueError),
+        (3, 0, None, None, None, PatternNotMatchedError),
+        (3, 0, 0, None, 0, ValueError),
+        (-1, 0, 0, None, None, ValueError),
+        (3, -1, 0, None, None, ValueError),
+        (3, 0, -1, None, None, ValueError),
+        (2.2, 0, 0, None, None, ValueError),
+        ("some string", 0, 0, None, None, ValueError),
+    ),
+)
+def test_fail_mobile_version_constructor(
+    major_number,
+    minor_number,
+    patch_number,
+    beta_number,
+    rc_number,
+    expected_error_type,
+):
+    with pytest.raises(expected_error_type):
         MobileVersion(
             major_number=major_number,
             minor_number=minor_number,
             patch_number=patch_number,
             beta_number=beta_number,
             release_candidate_number=rc_number,
         )
 
 
 def test_mobile_version_constructor_minimum_kwargs():
-    assert str(MobileVersion(3, 0, 1)) == '3.0.1'
-    assert str(MobileVersion(3, 1, 0)) == '3.1.0'
-    assert str(MobileVersion(3, 0, 0, beta_number=1)) == '3.0.0-beta.1'
-
-    assert str(MobileVersion(1, 0, 0, release_candidate_number=1)) == '1.0.0-rc.1'
-
-
-@pytest.mark.parametrize('version_string, ExpectedErrorType', (
-    ('1.0.0b1', PatternNotMatchedError),
-    ('1.0.0.0b1', ValueError),
-    ('1.0.0.1b1', PatternNotMatchedError),
-    ('1.0.0rc1', PatternNotMatchedError),
-    ('1.0.0.0rc1', ValueError),
-    ('1.0.0.1rc1', PatternNotMatchedError),
-    ('1.5.0.0rc1', ValueError),
-    ('1.5.0.1rc1', PatternNotMatchedError),
-    ('1.5.1.1', PatternNotMatchedError),
-    ('3.1.0b1', PatternNotMatchedError),
-
-    ('31.0b2esr', PatternNotMatchedError),
-    ('31.0esrb2', PatternNotMatchedError),
-
-    ('32', PatternNotMatchedError),
-    ('32.b2', PatternNotMatchedError),
-    ('.1', PatternNotMatchedError),
-    ('32.0a0', ValueError),
-    ('32.0b0', ValueError),
-    ('32.0.1a1', PatternNotMatchedError),
-    ('32.0.1a2', PatternNotMatchedError),
-    ('32.0.1b2', PatternNotMatchedError),
-    ('32.0build0', ValueError),
-    ('32.0a1a2', PatternNotMatchedError),
-    ('32.0a1b2', PatternNotMatchedError),
-
-    ('55.0a2', PatternNotMatchedError),
-    ('56.0a2', PatternNotMatchedError),
-
-    ('104.0a2', PatternNotMatchedError),
-    ('104.0.0-beta.1', PatternNotMatchedError),
-    ('104.0-beta.1', PatternNotMatchedError),
-    ('104.0.0-rc.1', PatternNotMatchedError),
-    ('104.1', PatternNotMatchedError),
-
-    ('109.0.0', PatternNotMatchedError),
-))
-def test_mobile_version_raises_when_invalid_version_is_given(version_string, ExpectedErrorType):
-    with pytest.raises(ExpectedErrorType):
+    assert str(MobileVersion(3, 0, 1)) == "3.0.1"
+    assert str(MobileVersion(3, 1, 0)) == "3.1.0"
+    assert str(MobileVersion(3, 0, 0, beta_number=1)) == "3.0.0-beta.1"
+
+    assert str(MobileVersion(1, 0, 0, release_candidate_number=1)) == "1.0.0-rc.1"
+
+
+@pytest.mark.parametrize(
+    "version_string, expected_error_type",
+    (
+        ("1.0.0b1", PatternNotMatchedError),
+        ("1.0.0.0b1", ValueError),
+        ("1.0.0.1b1", PatternNotMatchedError),
+        ("1.0.0rc1", PatternNotMatchedError),
+        ("1.0.0.0rc1", ValueError),
+        ("1.0.0.1rc1", PatternNotMatchedError),
+        ("1.5.0.0rc1", ValueError),
+        ("1.5.0.1rc1", PatternNotMatchedError),
+        ("1.5.1.1", PatternNotMatchedError),
+        ("3.1.0b1", PatternNotMatchedError),
+        ("31.0b2esr", PatternNotMatchedError),
+        ("31.0esrb2", PatternNotMatchedError),
+        ("32", PatternNotMatchedError),
+        ("32.b2", PatternNotMatchedError),
+        (".1", PatternNotMatchedError),
+        ("32.0a0", ValueError),
+        ("32.0b0", ValueError),
+        ("32.0.1a1", PatternNotMatchedError),
+        ("32.0.1a2", PatternNotMatchedError),
+        ("32.0.1b2", PatternNotMatchedError),
+        ("32.0build0", ValueError),
+        ("32.0a1a2", PatternNotMatchedError),
+        ("32.0a1b2", PatternNotMatchedError),
+        ("55.0a2", PatternNotMatchedError),
+        ("56.0a2", PatternNotMatchedError),
+        ("104.0a2", PatternNotMatchedError),
+        ("104.0.0-beta.1", PatternNotMatchedError),
+        ("104.0-beta.1", PatternNotMatchedError),
+        ("104.0.0-rc.1", PatternNotMatchedError),
+        ("104.1", PatternNotMatchedError),
+        ("109.0.0", PatternNotMatchedError),
+    ),
+)
+def test_mobile_version_raises_when_invalid_version_is_given(
+    version_string, expected_error_type
+):
+    with pytest.raises(expected_error_type):
         MobileVersion.parse(version_string)
 
 
-@pytest.mark.parametrize('version_string, expected_type', VALID_VERSIONS.items())
+@pytest.mark.parametrize("version_string, expected_type", VALID_VERSIONS.items())
 def test_mobile_version_is_of_a_defined_type(version_string, expected_type):
     release = MobileVersion.parse(version_string)
-    assert getattr(release, f'is_{expected_type}')
-
-
-@pytest.mark.parametrize('previous, next', (
-    ('2.0.0', '3.0.0'),
-    ('2.0.0', '3.1.0'),
-    ('2.0.0', '3.0.1'),
-
-    ('2.0.1', '3.0.0'),
-    ('2.0.1', '2.1.0'),
-    ('2.0.1', '2.0.2'),
-
-    ('2.1.0', '3.0.0'),
-    ('2.1.0', '2.2.0'),
-    ('2.1.0', '2.1.1'),
-
-    ('2.0.0-beta.1', '3.0.0-beta.1'),
-    ('2.0.0-beta.1', '2.0.0-beta.2'),
-
-    ('2.0.0-beta.1', '2.0.0'),
-
-    ('1.0.0-rc.1', '1.0.0-rc.2'),
-    ('1.0.0-rc.1', '1.0.0'),
-    ('3.5.0-beta.4', '3.5.0-rc.2'),
-    ('3.5.0-beta.4', '3.5.0'),
-    ('3.5.0-rc.2', '3.5.0'),
-    ('3.5.0-rc.2', '3.5.0-rc.3'),
-))
-def test_mobile_version_implements_lt_operator(previous, next):
-    assert MobileVersion.parse(previous) < MobileVersion.parse(next)
+    assert getattr(release, f"is_{expected_type}")
 
 
-@pytest.mark.parametrize('equivalent_version_string', (
-    '3.00.0', '03.0.0', '3.0.0',
-))
+@pytest.mark.parametrize(
+    "previous_version, next_version",
+    (
+        ("2.0.0", "3.0.0"),
+        ("2.0.0", "3.1.0"),
+        ("2.0.0", "3.0.1"),
+        ("2.0.1", "3.0.0"),
+        ("2.0.1", "2.1.0"),
+        ("2.0.1", "2.0.2"),
+        ("2.1.0", "3.0.0"),
+        ("2.1.0", "2.2.0"),
+        ("2.1.0", "2.1.1"),
+        ("2.0.0-beta.1", "3.0.0-beta.1"),
+        ("2.0.0-beta.1", "2.0.0-beta.2"),
+        ("2.0.0-beta.1", "2.0.0"),
+        ("1.0.0-rc.1", "1.0.0-rc.2"),
+        ("1.0.0-rc.1", "1.0.0"),
+        ("3.5.0-beta.4", "3.5.0-rc.2"),
+        ("3.5.0-beta.4", "3.5.0"),
+        ("3.5.0-rc.2", "3.5.0"),
+        ("3.5.0-rc.2", "3.5.0-rc.3"),
+    ),
+)
+def test_mobile_version_implements_lt_operator(previous_version, next_version):
+    assert MobileVersion.parse(previous_version) < MobileVersion.parse(next_version)
+
+
+@pytest.mark.parametrize(
+    "equivalent_version_string",
+    (
+        "3.00.0",
+        "03.0.0",
+        "3.0.0",
+    ),
+)
 def test_mobile_version_implements_eq_operator(equivalent_version_string):
-    assert MobileVersion.parse('3.0.0') == MobileVersion.parse(equivalent_version_string)
+    assert MobileVersion.parse("3.0.0") == MobileVersion.parse(
+        equivalent_version_string
+    )
     # raw strings are also converted
-    assert MobileVersion.parse('3.0.0') == equivalent_version_string
+    assert MobileVersion.parse("3.0.0") == equivalent_version_string
 
 
-@pytest.mark.parametrize('equivalent_version_string', (
-    '3.00.0-beta.1', '03.0.0-beta.1', '3.0.0-beta.1',
-))
+@pytest.mark.parametrize(
+    "equivalent_version_string",
+    (
+        "3.00.0-beta.1",
+        "03.0.0-beta.1",
+        "3.0.0-beta.1",
+    ),
+)
 def test_mobile_beta_version_implements_eq_operator(equivalent_version_string):
-    assert MobileVersion.parse('3.0.0-beta.1') == MobileVersion.parse(equivalent_version_string)
+    assert MobileVersion.parse("3.0.0-beta.1") == MobileVersion.parse(
+        equivalent_version_string
+    )
     # raw strings are also converted
-    assert MobileVersion.parse('3.0.0-beta.1') == equivalent_version_string
+    assert MobileVersion.parse("3.0.0-beta.1") == equivalent_version_string
 
 
-@pytest.mark.parametrize('equivalent_version_string', (
-    '3.00.0-rc.1', '03.0.0-rc.1', '3.0.0-rc.01',
-))
+@pytest.mark.parametrize(
+    "equivalent_version_string",
+    (
+        "3.00.0-rc.1",
+        "03.0.0-rc.1",
+        "3.0.0-rc.01",
+    ),
+)
 def test_mobile_rc_version_implements_eq_operator(equivalent_version_string):
-    assert MobileVersion.parse('3.0.0-rc.1') == MobileVersion.parse(equivalent_version_string)
+    assert MobileVersion.parse("3.0.0-rc.1") == MobileVersion.parse(
+        equivalent_version_string
+    )
     # raw strings are also converted
-    assert MobileVersion.parse('3.0.0-rc.1') == equivalent_version_string
+    assert MobileVersion.parse("3.0.0-rc.1") == equivalent_version_string
 
 
-@pytest.mark.parametrize('wrong_type', (
-    3,
-    3.0,
-    ('3', '0', '1'),
-    ['3', '0', '1'],
-    LooseVersion('3.0.0'),
-    StrictVersion('3.0.0'),
-))
+@pytest.mark.parametrize(
+    "wrong_type",
+    (
+        3,
+        3.0,
+        ("3", "0", "1"),
+        ["3", "0", "1"],
+        LooseVersion("3.0.0"),
+        StrictVersion("3.0.0"),
+    ),
+)
 def test_mobile_version_raises_eq_operator(wrong_type):
     with pytest.raises(ValueError):
-        assert MobileVersion.parse('3.0.0') == wrong_type
+        assert MobileVersion.parse("3.0.0") == wrong_type
     # AttributeError is raised by LooseVersion and StrictVersion
     with pytest.raises((ValueError, AttributeError)):
-        assert wrong_type == MobileVersion.parse('3.0.0')
+        assert wrong_type == MobileVersion.parse("3.0.0")
 
 
 def test_mobile_version_implements_remaining_comparision_operators():
-    assert MobileVersion.parse('2.0.0') <= MobileVersion.parse('2.0.0')
-    assert MobileVersion.parse('2.0.0') <= MobileVersion.parse('3.0.0')
+    assert MobileVersion.parse("2.0.0") <= MobileVersion.parse("2.0.0")
+    assert MobileVersion.parse("2.0.0") <= MobileVersion.parse("3.0.0")
 
-    assert MobileVersion.parse('3.0.0') >= MobileVersion.parse('2.0.0')
-    assert MobileVersion.parse('3.0.0') >= MobileVersion.parse('3.0.0')
+    assert MobileVersion.parse("3.0.0") >= MobileVersion.parse("2.0.0")
+    assert MobileVersion.parse("3.0.0") >= MobileVersion.parse("3.0.0")
 
-    assert MobileVersion.parse('3.0.0') > MobileVersion.parse('2.0.0')
-    assert not MobileVersion.parse('3.0.0') > MobileVersion.parse('3.0.0')
+    assert MobileVersion.parse("3.0.0") > MobileVersion.parse("2.0.0")
+    assert not MobileVersion.parse("3.0.0") > MobileVersion.parse("3.0.0")
 
-    assert not MobileVersion.parse('2.0.0') < MobileVersion.parse('2.0.0')
-
-    assert MobileVersion.parse('3.0.0') != MobileVersion.parse('2.0.0')
-
-
-@pytest.mark.parametrize('version_string, expected_output', (
-    ('2.0.0', '2.0.0'),
-    ('02.0.0', '2.0.0'),
-    ('2.0.1', '2.0.1'),
-    ('2.0.0-rc.1', '2.0.0-rc.1'),
-    ('2.0.0-rc.2', '2.0.0-rc.2'),
-    ('2.0.0-rc.02', '2.0.0-rc.2'),
-    ('2.0.0-beta.1', '2.0.0-beta.1'),
-    ('2.0.0-beta.01', '2.0.0-beta.1'),
-
-    ('104.0', '104.0'),
-    ('0104.0', '104.0'),
-    ('104.0build1', '104.0build1'),
-    ('104.0build01', '104.0build1'),
-    ('104.0.1', '104.0.1'),
-    ('104.0a1', '104.0a1'),
-    ('104.0b1', '104.0b1'),
-    ('104.0b01', '104.0b1'),
-))
+    assert not MobileVersion.parse("2.0.0") < MobileVersion.parse("2.0.0")
+
+    assert MobileVersion.parse("3.0.0") != MobileVersion.parse("2.0.0")
+
+
+@pytest.mark.parametrize(
+    "version_string, expected_output",
+    (
+        ("2.0.0", "2.0.0"),
+        ("02.0.0", "2.0.0"),
+        ("2.0.1", "2.0.1"),
+        ("2.0.0-rc.1", "2.0.0-rc.1"),
+        ("2.0.0-rc.2", "2.0.0-rc.2"),
+        ("2.0.0-rc.02", "2.0.0-rc.2"),
+        ("2.0.0-beta.1", "2.0.0-beta.1"),
+        ("2.0.0-beta.01", "2.0.0-beta.1"),
+        ("104.0", "104.0"),
+        ("0104.0", "104.0"),
+        ("104.0build1", "104.0build1"),
+        ("104.0build01", "104.0build1"),
+        ("104.0.1", "104.0.1"),
+        ("104.0a1", "104.0a1"),
+        ("104.0b1", "104.0b1"),
+        ("104.0b01", "104.0b1"),
+    ),
+)
 def test_mobile_version_implements_str_operator(version_string, expected_output):
     assert str(MobileVersion.parse(version_string)) == expected_output
 
 
-@pytest.mark.parametrize('version_string, field, expected', (
-    ('0.9.0', 'major_number', '1.0.0'),
-    ('0.9.1', 'major_number', '1.0.0'),
-    ('1.0.0-beta.1', 'beta_number', '1.0.0-beta.2'),
-    ('1.0.0-rc.1', 'release_candidate_number', '1.0.0-rc.2'),
-    ('1.0.0', 'patch_number', '1.0.1'),
-    ('1.5.0', 'minor_number', '1.6.0'),
-    ('1.5.1', 'minor_number', '1.6.0'),
-    ('2.0.0-rc.1', 'release_candidate_number', '2.0.0-rc.2'),
-    ('2.0.0', 'major_number', '3.0.0'),
-    ('2.0.1', 'major_number', '3.0.0'),
-
-    ('2.0.0-rc.2', 'major_number', '3.0.0'),
-    ('2.0.0-beta.1', 'major_number', '3.0.0-beta.1'),
-    ('2.0.0', 'major_number', '3.0.0'),
-    ('2.0.1', 'major_number', '3.0.0'),
-
-    ('2.0.0', 'minor_number', '2.1.0'),
-    ('2.0.1', 'minor_number', '2.1.0'),
-
-    ('2.0.0', 'patch_number', '2.0.1'),
-    ('2.0.1', 'patch_number', '2.0.2'),
-
-    ('2.0.0-beta.1', 'beta_number', '2.0.0-beta.2'),
-
-    ('103.0.0-beta.1', 'major_number', '104.0b1'),
-    ('103.0.0-rc.2', 'major_number', '104.0'),
-    ('103.0.0', 'major_number', '104.0'),
-
-    ('104.0a1', 'major_number', '105.0a1'),
-    ('104.0b2', 'major_number', '105.0b1'),
-    ('104.0', 'major_number', '105.0'),
-
-    ('104.0', 'minor_number', '104.1.0'),
-    ('104.0.1', 'minor_number', '104.1.0'),
-
-    ('104.0', 'patch_number', '104.0.1'),
-    ('104.0.1', 'patch_number', '104.0.2'),
-
-    ('104.0b1', 'beta_number', '104.0b2'),
-
-    ('104.0build1', 'build_number', '104.0build2'),
-    ('104.0b1build1', 'build_number', '104.0b1build2'),
-))
+@pytest.mark.parametrize(
+    "version_string, field, expected",
+    (
+        ("0.9.0", "major_number", "1.0.0"),
+        ("0.9.1", "major_number", "1.0.0"),
+        ("1.0.0-beta.1", "beta_number", "1.0.0-beta.2"),
+        ("1.0.0-rc.1", "release_candidate_number", "1.0.0-rc.2"),
+        ("1.0.0", "patch_number", "1.0.1"),
+        ("1.5.0", "minor_number", "1.6.0"),
+        ("1.5.1", "minor_number", "1.6.0"),
+        ("2.0.0-rc.1", "release_candidate_number", "2.0.0-rc.2"),
+        ("2.0.0", "major_number", "3.0.0"),
+        ("2.0.1", "major_number", "3.0.0"),
+        ("2.0.0-rc.2", "major_number", "3.0.0"),
+        ("2.0.0-beta.1", "major_number", "3.0.0-beta.1"),
+        ("2.0.0", "major_number", "3.0.0"),
+        ("2.0.1", "major_number", "3.0.0"),
+        ("2.0.0", "minor_number", "2.1.0"),
+        ("2.0.1", "minor_number", "2.1.0"),
+        ("2.0.0", "patch_number", "2.0.1"),
+        ("2.0.1", "patch_number", "2.0.2"),
+        ("2.0.0-beta.1", "beta_number", "2.0.0-beta.2"),
+        ("103.0.0-beta.1", "major_number", "104.0b1"),
+        ("103.0.0-rc.2", "major_number", "104.0"),
+        ("103.0.0", "major_number", "104.0"),
+        ("104.0a1", "major_number", "105.0a1"),
+        ("104.0b2", "major_number", "105.0b1"),
+        ("104.0", "major_number", "105.0"),
+        ("104.0", "minor_number", "104.1.0"),
+        ("104.0.1", "minor_number", "104.1.0"),
+        ("104.0", "patch_number", "104.0.1"),
+        ("104.0.1", "patch_number", "104.0.2"),
+        ("104.0b1", "beta_number", "104.0b2"),
+        ("104.0build1", "build_number", "104.0build2"),
+        ("104.0b1build1", "build_number", "104.0b1build2"),
+    ),
+)
 def test_mobile_version_bump(version_string, field, expected):
     version = MobileVersion.parse(version_string)
     assert str(version.bump(field)) == expected
 
 
-@pytest.mark.parametrize('version_string, field', (
-    ('2.0.0-beta.1', 'release_candidate_number'),
-))
+@pytest.mark.parametrize(
+    "version_string, field", (("2.0.0-beta.1", "release_candidate_number"),)
+)
 def test_mobile_version_bump_raises(version_string, field):
     version = MobileVersion.parse(version_string)
     with pytest.raises(ValueError):
         version.bump(field)
 
 
-_SUPER_PERMISSIVE_PATTERN = re.compile(r"""
+_SUPER_PERMISSIVE_PATTERN = re.compile(
+    r"""
 ^(?P<major_number>\d+)\.(?P<minor_number>\d+)(\.(?P<patch_number>\d+))?
 (-beta\.(?P<beta_number>\d+))?(-rc\.(?P<release_candidate_number>\d+))?
-""", re.VERBOSE)
+""",
+    re.VERBOSE,
+)
 
 
-@pytest.mark.parametrize('version_string', (
-    '2.0.0-beta.1-rc.2',
-))
-def test_mobile_version_ensures_it_does_not_have_multiple_type(monkeypatch, version_string):
+@pytest.mark.parametrize("version_string", ("2.0.0-beta.1-rc.2",))
+def test_mobile_version_ensures_it_does_not_have_multiple_type(version_string):
     # Let's make sure the sanity checks detect a broken regular expression
     original_pattern = MobileVersion._VALID_ENOUGH_VERSION_PATTERN
     MobileVersion._VALID_ENOUGH_VERSION_PATTERN = _SUPER_PERMISSIVE_PATTERN
 
     with pytest.raises(TooManyTypesError):
         MobileVersion.parse(version_string)
 
     MobileVersion._VALID_ENOUGH_VERSION_PATTERN = original_pattern
 
 
-def test_mobile_version_ensures_a_new_added_release_type_is_caught(monkeypatch):
+def test_mobile_version_ensures_a_new_added_release_type_is_caught():
     # Let's make sure the sanity checks detect a broken regular expression
     original_pattern = MobileVersion._VALID_ENOUGH_VERSION_PATTERN
     MobileVersion._VALID_ENOUGH_VERSION_PATTERN = _SUPER_PERMISSIVE_PATTERN
 
     # And a broken type detection
     original_is_release = MobileVersion.is_release
     MobileVersion.is_release = False
 
     with pytest.raises(NoVersionTypeError):
-        mozilla_version.mobile.MobileVersion.parse('2.0.0')
+        mozilla_version.mobile.MobileVersion.parse("2.0.0")
 
     MobileVersion.is_release = original_is_release
     MobileVersion._VALID_ENOUGH_VERSION_PATTERN = original_pattern
```

### Comparing `mozilla_version-3.0.0/mozilla_version/test/test_version.py` & `mozilla-version-3.1.0/mozilla_version/test/test_version.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,220 +1,257 @@
-import pytest
-
 from distutils.version import LooseVersion, StrictVersion
 
+import pytest
+
 from mozilla_version.errors import PatternNotMatchedError
 from mozilla_version.version import BaseVersion, VersionType
 
 
-@pytest.mark.parametrize('major_number, minor_number, patch_number, expected_output_string', ((
-    32, 0, None, '32.0'
-), (
-    32, 0, 1, '32.0.1'
-)))
-def test_base_version_constructor_and_str(major_number, minor_number, patch_number, expected_output_string):
-    assert str(BaseVersion(
-        major_number=major_number,
-        minor_number=minor_number,
-        patch_number=patch_number,
-    )) == expected_output_string
-
-
-@pytest.mark.parametrize('major_number, minor_number, patch_number, ExpectedErrorType', ((
-    -1, 0, None, ValueError
-), (
-    32, -1, None, ValueError
-), (
-    32, 0, -1, ValueError
-), (
-    2.2, 0, 0, ValueError
-), (
-    'some string', 0, 0, ValueError
-)))
-def test_fail_base_version_constructor(major_number, minor_number, patch_number, ExpectedErrorType):
-    with pytest.raises(ExpectedErrorType):
+@pytest.mark.parametrize(
+    "major_number, minor_number, patch_number, expected_output_string",
+    ((32, 0, None, "32.0"), (32, 0, 1, "32.0.1")),
+)
+def test_base_version_constructor_and_str(
+    major_number, minor_number, patch_number, expected_output_string
+):
+    assert (
+        str(
+            BaseVersion(
+                major_number=major_number,
+                minor_number=minor_number,
+                patch_number=patch_number,
+            )
+        )
+        == expected_output_string
+    )
+
+
+@pytest.mark.parametrize(
+    "major_number, minor_number, patch_number, expected_error_type",
+    (
+        (-1, 0, None, ValueError),
+        (32, -1, None, ValueError),
+        (32, 0, -1, ValueError),
+        (2.2, 0, 0, ValueError),
+        ("some string", 0, 0, ValueError),
+    ),
+)
+def test_fail_base_version_constructor(
+    major_number, minor_number, patch_number, expected_error_type
+):
+    with pytest.raises(expected_error_type):
         BaseVersion(
             major_number=major_number,
             minor_number=minor_number,
             patch_number=patch_number,
         )
 
 
 def test_base_version_constructor_minimum_kwargs():
-    assert str(BaseVersion(32, 0)) == '32.0'
-    assert str(BaseVersion(32, 0, 1)) == '32.0.1'
-    assert str(BaseVersion(32, 1, 0)) == '32.1.0'
+    assert str(BaseVersion(32, 0)) == "32.0"
+    assert str(BaseVersion(32, 0, 1)) == "32.0.1"
+    assert str(BaseVersion(32, 1, 0)) == "32.1.0"
+
+
+@pytest.mark.parametrize(
+    "version_string, expected_error_type",
+    (
+        ("32", PatternNotMatchedError),
+        (".1", PatternNotMatchedError),
+    ),
+)
+def test_base_version_raises_when_invalid_version_is_given(
+    version_string, expected_error_type
+):
+    with pytest.raises(expected_error_type):
+        BaseVersion.parse(version_string)
 
 
-@pytest.mark.parametrize('version_string, ExpectedErrorType', (
-    ('32', PatternNotMatchedError),
-    ('.1', PatternNotMatchedError),
-))
-def test_base_version_raises_when_invalid_version_is_given(version_string, ExpectedErrorType):
-    with pytest.raises(ExpectedErrorType):
-        BaseVersion.parse(version_string)
+@pytest.mark.parametrize(
+    "previous_version, next_version",
+    (
+        ("32.0", "33.0"),
+        ("32.0", "32.1.0"),
+        ("32.0", "32.0.1"),
+        ("32.0.1", "33.0"),
+        ("32.0.1", "32.1.0"),
+        ("32.0.1", "32.0.2"),
+        ("32.1.0", "33.0"),
+        ("32.1.0", "32.2.0"),
+        ("32.1.0", "32.1.1"),
+        ("2.0", "10.0"),
+        ("10.2.0", "10.10.0"),
+        ("10.0.2", "10.0.10"),
+        ("10.10.1", "10.10.10"),
+    ),
+)
+def test_base_version_implements_lt_operator(previous_version, next_version):
+    assert BaseVersion.parse(previous_version) < BaseVersion.parse(next_version)
 
 
-@pytest.mark.parametrize('previous, next', (
-    ('32.0', '33.0'),
-    ('32.0', '32.1.0'),
-    ('32.0', '32.0.1'),
-
-    ('32.0.1', '33.0'),
-    ('32.0.1', '32.1.0'),
-    ('32.0.1', '32.0.2'),
-
-    ('32.1.0', '33.0'),
-    ('32.1.0', '32.2.0'),
-    ('32.1.0', '32.1.1'),
-
-    ('2.0', '10.0'),
-    ('10.2.0', '10.10.0'),
-    ('10.0.2', '10.0.10'),
-    ('10.10.1', '10.10.10'),
-))
-def test_base_version_implements_lt_operator(previous, next):
-    assert BaseVersion.parse(previous) < BaseVersion.parse(next)
-
-
-@pytest.mark.parametrize('equivalent_version_string', (
-    '32.0', '032.0', '32.00'
-))
+@pytest.mark.parametrize("equivalent_version_string", ("32.0", "032.0", "32.00"))
 def test_base_version_implements_eq_operator(equivalent_version_string):
-    assert BaseVersion.parse('32.0') == BaseVersion.parse(equivalent_version_string)
+    assert BaseVersion.parse("32.0") == BaseVersion.parse(equivalent_version_string)
     # raw strings are also converted
-    assert BaseVersion.parse('32.0') == equivalent_version_string
+    assert BaseVersion.parse("32.0") == equivalent_version_string
 
 
-@pytest.mark.parametrize('wrong_type', (
-    32,
-    32.0,
-    ('32', '0', '1'),
-    ['32', '0', '1'],
-    LooseVersion('32.0'),
-    StrictVersion('32.0'),
-))
+@pytest.mark.parametrize(
+    "wrong_type",
+    (
+        32,
+        32.0,
+        ("32", "0", "1"),
+        ["32", "0", "1"],
+        LooseVersion("32.0"),
+        StrictVersion("32.0"),
+    ),
+)
 def test_base_version_raises_eq_operator(wrong_type):
     with pytest.raises(ValueError):
-        assert BaseVersion.parse('32.0') == wrong_type
+        assert BaseVersion.parse("32.0") == wrong_type
     # AttributeError is raised by LooseVersion and StrictVersion
     with pytest.raises((ValueError, AttributeError)):
-        assert wrong_type == BaseVersion.parse('32.0')
+        assert wrong_type == BaseVersion.parse("32.0")
 
 
 def test_base_version_implements_remaining_comparision_operators():
-    assert BaseVersion.parse('32.0') <= BaseVersion.parse('32.0')
-    assert BaseVersion.parse('32.0') <= BaseVersion.parse('33.0')
+    assert BaseVersion.parse("32.0") <= BaseVersion.parse("32.0")
+    assert BaseVersion.parse("32.0") <= BaseVersion.parse("33.0")
 
-    assert BaseVersion.parse('33.0') >= BaseVersion.parse('32.0')
-    assert BaseVersion.parse('33.0') >= BaseVersion.parse('33.0')
+    assert BaseVersion.parse("33.0") >= BaseVersion.parse("32.0")
+    assert BaseVersion.parse("33.0") >= BaseVersion.parse("33.0")
 
-    assert BaseVersion.parse('33.0') > BaseVersion.parse('32.0')
-    assert not BaseVersion.parse('33.0') > BaseVersion.parse('33.0')
+    assert BaseVersion.parse("33.0") > BaseVersion.parse("32.0")
+    assert not BaseVersion.parse("33.0") > BaseVersion.parse("33.0")
 
-    assert not BaseVersion.parse('32.0') < BaseVersion.parse('32.0')
+    assert not BaseVersion.parse("32.0") < BaseVersion.parse("32.0")
 
-    assert BaseVersion.parse('33.0') != BaseVersion.parse('32.0')
+    assert BaseVersion.parse("33.0") != BaseVersion.parse("32.0")
 
 
 def test_base_version_hashable():
-    hash(BaseVersion.parse('63.0'))
+    hash(BaseVersion.parse("63.0"))
 
 
-class _DummyVersion():
+class _DummyVersion:
     def __init__(self, major_number):
         self.major_number = major_number
 
-@pytest.mark.parametrize('base_version, other, field, expected', ((
-    BaseVersion(32, 0),
-    BaseVersion(32, 0),
-    'major_number',
-    0,
-), (
-    BaseVersion(32, 0),
-    BaseVersion(33, 0),
-    'major_number',
-    -1,
-), (
-    BaseVersion(32, 0),
-    BaseVersion(31, 0),
-    'major_number',
-    1,
-), (
-    BaseVersion(32, 0),
-    BaseVersion(32, 0, 1),
-    'patch_number',
-    -1,
-), (
-    BaseVersion(32, 0),
-    _DummyVersion(32),
-    'major_number',
-    0,
-), (
-    BaseVersion(32, 0, 1),
-    _DummyVersion(32),  # No patch_number so we make sure AttributeError is raised
-    'patch_number',
-    1,
-)))
-def test_base_version_substract_other_number_from_this_number(base_version, other, field, expected):
-    assert base_version._substract_other_number_from_this_number(other, field) == expected
-
-@pytest.mark.parametrize('version_string, field, expected', (
-    ('0.9', 'major_number', '1.0'),
-    ('0.9.1', 'major_number', '1.0.0'),
-    ('32.0', 'major_number', '33.0'),
-    ('32.0.1', 'major_number', '33.0.0'),
-    ('32.0', 'minor_number', '32.1.0'),
-    ('32.0.1', 'minor_number', '32.1.0'),
-    ('32.0', 'patch_number', '32.0.1'),
-    ('32.0.1', 'patch_number', '32.0.2'),
-))
+
+@pytest.mark.parametrize(
+    "base_version, other, field, expected",
+    (
+        (
+            BaseVersion(32, 0),
+            BaseVersion(32, 0),
+            "major_number",
+            0,
+        ),
+        (
+            BaseVersion(32, 0),
+            BaseVersion(33, 0),
+            "major_number",
+            -1,
+        ),
+        (
+            BaseVersion(32, 0),
+            BaseVersion(31, 0),
+            "major_number",
+            1,
+        ),
+        (
+            BaseVersion(32, 0),
+            BaseVersion(32, 0, 1),
+            "patch_number",
+            -1,
+        ),
+        (
+            BaseVersion(32, 0),
+            _DummyVersion(32),
+            "major_number",
+            0,
+        ),
+        (
+            BaseVersion(32, 0, 1),
+            _DummyVersion(
+                32
+            ),  # No patch_number so we make sure AttributeError is raised
+            "patch_number",
+            1,
+        ),
+    ),
+)
+def test_base_version_substract_other_number_from_this_number(
+    base_version, other, field, expected
+):
+    assert (
+        base_version._substract_other_number_from_this_number(other, field) == expected
+    )
+
+
+@pytest.mark.parametrize(
+    "version_string, field, expected",
+    (
+        ("0.9", "major_number", "1.0"),
+        ("0.9.1", "major_number", "1.0.0"),
+        ("32.0", "major_number", "33.0"),
+        ("32.0.1", "major_number", "33.0.0"),
+        ("32.0", "minor_number", "32.1.0"),
+        ("32.0.1", "minor_number", "32.1.0"),
+        ("32.0", "patch_number", "32.0.1"),
+        ("32.0.1", "patch_number", "32.0.2"),
+    ),
+)
 def test_base_version_bump(version_string, field, expected):
     version = BaseVersion.parse(version_string)
     assert str(version.bump(field)) == expected
 
 
 def test_base_version_bump_raises():
-    version = BaseVersion.parse('32.0')
+    version = BaseVersion.parse("32.0")
     with pytest.raises(ValueError):
-        version.bump('non_existing_number')
+        version.bump("non_existing_number")
+
 
-@pytest.mark.parametrize('previous, next', (
-    (VersionType.NIGHTLY, VersionType.AURORA_OR_DEVEDITION),
-    (VersionType.NIGHTLY, VersionType.BETA),
-    (VersionType.NIGHTLY, VersionType.RELEASE_CANDIDATE),
-    (VersionType.NIGHTLY, VersionType.RELEASE),
-    (VersionType.NIGHTLY, VersionType.ESR),
-
-    (VersionType.AURORA_OR_DEVEDITION, VersionType.BETA),
-    (VersionType.AURORA_OR_DEVEDITION, VersionType.RELEASE_CANDIDATE),
-    (VersionType.AURORA_OR_DEVEDITION, VersionType.RELEASE),
-    (VersionType.AURORA_OR_DEVEDITION, VersionType.ESR),
-
-    (VersionType.BETA, VersionType.RELEASE_CANDIDATE),
-    (VersionType.BETA, VersionType.RELEASE),
-    (VersionType.BETA, VersionType.ESR),
-
-    (VersionType.RELEASE_CANDIDATE, VersionType.RELEASE),
-    (VersionType.RELEASE_CANDIDATE, VersionType.ESR),
-
-    (VersionType.RELEASE, VersionType.ESR),
-))
-def test_version_type_implements_lt_operator(previous, next):
-    assert previous < next
-
-
-@pytest.mark.parametrize('first, second', (
-    (VersionType.NIGHTLY, VersionType.NIGHTLY),
-    (VersionType.AURORA_OR_DEVEDITION, VersionType.AURORA_OR_DEVEDITION),
-    (VersionType.BETA, VersionType.BETA),
-    (VersionType.RELEASE, VersionType.RELEASE),
-    (VersionType.RELEASE_CANDIDATE, VersionType.RELEASE_CANDIDATE),
-    (VersionType.ESR, VersionType.ESR),
-))
+@pytest.mark.parametrize(
+    "previous_version, next_version",
+    (
+        (VersionType.NIGHTLY, VersionType.AURORA_OR_DEVEDITION),
+        (VersionType.NIGHTLY, VersionType.BETA),
+        (VersionType.NIGHTLY, VersionType.RELEASE_CANDIDATE),
+        (VersionType.NIGHTLY, VersionType.RELEASE),
+        (VersionType.NIGHTLY, VersionType.ESR),
+        (VersionType.AURORA_OR_DEVEDITION, VersionType.BETA),
+        (VersionType.AURORA_OR_DEVEDITION, VersionType.RELEASE_CANDIDATE),
+        (VersionType.AURORA_OR_DEVEDITION, VersionType.RELEASE),
+        (VersionType.AURORA_OR_DEVEDITION, VersionType.ESR),
+        (VersionType.BETA, VersionType.RELEASE_CANDIDATE),
+        (VersionType.BETA, VersionType.RELEASE),
+        (VersionType.BETA, VersionType.ESR),
+        (VersionType.RELEASE_CANDIDATE, VersionType.RELEASE),
+        (VersionType.RELEASE_CANDIDATE, VersionType.ESR),
+        (VersionType.RELEASE, VersionType.ESR),
+    ),
+)
+def test_version_type_implements_lt_operator(previous_version, next_version):
+    assert previous_version < next_version
+
+
+@pytest.mark.parametrize(
+    "first, second",
+    (
+        (VersionType.NIGHTLY, VersionType.NIGHTLY),
+        (VersionType.AURORA_OR_DEVEDITION, VersionType.AURORA_OR_DEVEDITION),
+        (VersionType.BETA, VersionType.BETA),
+        (VersionType.RELEASE, VersionType.RELEASE),
+        (VersionType.RELEASE_CANDIDATE, VersionType.RELEASE_CANDIDATE),
+        (VersionType.ESR, VersionType.ESR),
+    ),
+)
 def test_version_type_implements_eq_operator(first, second):
     assert first == second
 
 
 def test_version_type_implements_remaining_comparision_operators():
     assert VersionType.NIGHTLY <= VersionType.NIGHTLY
     assert VersionType.NIGHTLY <= VersionType.BETA
```

### Comparing `mozilla_version-3.0.0/mozilla_version/version.py` & `mozilla-version-3.1.0/mozilla_version/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,65 @@
 """Defines common characteristics of a version at Mozilla."""
 
-import attr
 import re
-
+from contextlib import suppress
 from enum import Enum
 
+import attr
+
 from mozilla_version.errors import MissingFieldError, PatternNotMatchedError
 from mozilla_version.parser import (
-    get_value_matched_by_regex,
     does_regex_have_group,
+    get_value_matched_by_regex,
     positive_int,
     positive_int_or_none,
 )
 
 
 @attr.s(frozen=True, eq=False, hash=True)
 class BaseVersion:
     """Class that validates and handles general version numbers."""
 
     major_number = attr.ib(type=int, converter=positive_int)
     minor_number = attr.ib(type=int, converter=positive_int)
     patch_number = attr.ib(type=int, converter=positive_int_or_none, default=None)
 
-    _MANDATORY_NUMBERS = ('major_number', 'minor_number')
-    _OPTIONAL_NUMBERS = ('patch_number', )
+    _MANDATORY_NUMBERS = ("major_number", "minor_number")
+    _OPTIONAL_NUMBERS = ("patch_number",)
     _ALL_NUMBERS = _MANDATORY_NUMBERS + _OPTIONAL_NUMBERS
 
-    _VALID_ENOUGH_VERSION_PATTERN = re.compile(r"""
+    _VALID_ENOUGH_VERSION_PATTERN = re.compile(
+        r"""
         ^(?P<major_number>\d+)
         \.(?P<minor_number>\d+)
-        (\.(?P<patch_number>\d+))?$""", re.VERBOSE)
+        (\.(?P<patch_number>\d+))?$""",
+        re.VERBOSE,
+    )
 
     @classmethod
     def parse(cls, version_string, regex_groups=()):
         """Construct an object representing a valid version number."""
         regex_matches = cls._VALID_ENOUGH_VERSION_PATTERN.match(version_string)
 
         if regex_matches is None:
-            raise PatternNotMatchedError(version_string, (cls._VALID_ENOUGH_VERSION_PATTERN,))
+            raise PatternNotMatchedError(
+                version_string, (cls._VALID_ENOUGH_VERSION_PATTERN,)
+            )
 
         kwargs = {}
 
         for field in cls._MANDATORY_NUMBERS:
-            kwargs[field] = get_value_matched_by_regex(field, regex_matches, version_string)
+            kwargs[field] = get_value_matched_by_regex(
+                field, regex_matches, version_string
+            )
         for field in cls._OPTIONAL_NUMBERS:
-            try:
-                kwargs[field] = get_value_matched_by_regex(field, regex_matches, version_string)
-            except MissingFieldError:
-                pass
+            with suppress(MissingFieldError):
+                kwargs[field] = get_value_matched_by_regex(
+                    field, regex_matches, version_string
+                )
 
         for regex_group in regex_groups:
             kwargs[regex_group] = does_regex_have_group(regex_matches, regex_group)
 
         return cls(**kwargs)
 
     def __str__(self):
@@ -59,15 +67,15 @@
 
         Computes a new string based on the given attributes.
         """
         semvers = [str(self.major_number), str(self.minor_number)]
         if self.patch_number is not None:
             semvers.append(str(self.patch_number))
 
-        return '.'.join(semvers)
+        return ".".join(semvers)
 
     def __eq__(self, other):
         """Implement `==` operator."""
         return self._compare(other) == 0
 
     def __ne__(self, other):
         """Implement `!=` operator."""
@@ -99,45 +107,45 @@
 
         """
         if isinstance(other, str):
             other = BaseVersion.parse(other)
         elif not isinstance(other, BaseVersion):
             raise ValueError(f'Cannot compare "{other}", type not supported!')
 
-        for field in ('major_number', 'minor_number', 'patch_number'):
+        for field in ("major_number", "minor_number", "patch_number"):
             difference = self._substract_other_number_from_this_number(other, field)
             if difference != 0:
                 return difference
 
         return 0
 
     def _substract_other_number_from_this_number(self, other, field):
-        # BaseVersion sets unmatched numbers to None. E.g.: "32.0" sets the patch_number to None.
-        # Because of this behavior, `getattr(self, 'patch_number')` returns None too. That's why
-        # we can't call `getattr(self, field, 0)` directly, it will return None for all unmatched
-        # numbers
+        # BaseVersion sets unmatched numbers to None. E.g.: "32.0" sets the patch_number
+        # to None. Because of this behavior, `getattr(self, 'patch_number')` returns
+        # None too. That's why we can't call `getattr(self, field, 0)` directly, it will
+        # return None for all unmatched numbers
         this_number = getattr(self, field, None)
         this_number = 0 if this_number is None else this_number
         other_number = getattr(other, field, None)
         other_number = 0 if other_number is None else other_number
 
         return this_number - other_number
 
     def bump(self, field):
         """Bump the number defined `field`.
 
         Returns:
-            A new BaseVersion with the right field bumped and the following ones set to 0,
-            if they exist or if they need to be set.
+            A new BaseVersion with the right field bumped and the following ones set to
+            0, if they exist or if they need to be set.
 
             For instance:
              * 32.0 is bumped to 33.0, because the patch number does not exist
              * 32.0.1 is bumped to 33.0.0, because the patch number exists
-             * 32.0 is bumped to 32.1.0, because patch number must be defined if the minor number
-               is not 0.
+             * 32.0 is bumped to 32.1.0, because patch number must be defined if the
+               minor number is not 0.
 
         """
         try:
             return self.__class__(**self._create_bump_kwargs(field))
         except (ValueError, PatternNotMatchedError) as e:
             raise ValueError(
                 f'Cannot bump "{field}". New version number is not valid. Cause: {e}'
@@ -151,41 +159,39 @@
         has_requested_field_been_met = False
         should_set_optional_numbers = False
         for current_field in self._ALL_NUMBERS:
             current_number = getattr(self, current_field, None)
             if current_field == field:
                 has_requested_field_been_met = True
                 new_number = 1 if current_number is None else current_number + 1
-                if new_number == 1 and current_field == 'minor_number':
+                if new_number == 1 and current_field == "minor_number":
                     should_set_optional_numbers = True
                 kwargs[current_field] = new_number
             else:
-                if (
-                    has_requested_field_been_met and
-                    (
-                        current_field not in self._OPTIONAL_NUMBERS or
-                        should_set_optional_numbers or
-                        current_number is not None
-                    )
+                if has_requested_field_been_met and (
+                    current_field not in self._OPTIONAL_NUMBERS
+                    or should_set_optional_numbers
+                    or current_number is not None
                 ):
                     new_number = 0
                 else:
                     new_number = current_number
                 kwargs[current_field] = new_number
 
         return kwargs
 
 
 class VersionType(Enum):
     """Enum that sorts types of versions (e.g.: nightly, beta, release, esr).
 
-    Supports comparison. `ESR` is considered higher than `RELEASE` (even if they technically have
-    the same codebase). For instance: 60.0.1 < 60.0.1esr but 61.0 > 60.0.1esr.
-    This choice has a practical use case: if you have a list of Release and ESR version, you can
-    easily extract one kind or the other thanks to the VersionType.
+    Supports comparison. `ESR` is considered higher than `RELEASE` (even if they
+    technically have the same codebase). For instance: 60.0.1 < 60.0.1esr but
+    61.0 > 60.0.1esr. This choice has a practical use case: if you have a list of
+    Release and ESR version, you can easily extract one kind or the other thanks to the
+    VersionType.
 
     Examples:
         .. code-block:: python
 
             assert VersionType.NIGHTLY == VersionType.NIGHTLY
             assert VersionType.ESR > VersionType.RELEASE
 
@@ -248,47 +254,51 @@
         error_messages = self._get_all_error_messages_for_attributes()
         if error_messages:
             raise PatternNotMatchedError(self, patterns=error_messages)
 
     def _get_all_error_messages_for_attributes(self):
         return [
             pattern_message
-            for condition, pattern_message in ((
-                self.is_major and self.is_stability,
-                'Version cannot be both a major and a stability one',
-            ), (
-                self.is_major and self.is_development,
-                'Version cannot be both a major and a development one',
-            ), (
-                self.is_stability and self.is_development,
-                'Version cannot be both a stability and a development one',
-            ))
+            for condition, pattern_message in (
+                (
+                    self.is_major and self.is_stability,
+                    "Version cannot be both a major and a stability one",
+                ),
+                (
+                    self.is_major and self.is_development,
+                    "Version cannot be both a major and a development one",
+                ),
+                (
+                    self.is_stability and self.is_development,
+                    "Version cannot be both a stability and a development one",
+                ),
+            )
             if condition
         ]
 
     @property
     def is_major(self):
         """Return `True` if `ShipItVersion` is considered to be a major version.
 
         It's usually the .0 release but some exceptions may occur.
         """
-        return all((
-            not self.is_development,
-            self.minor_number == 0,
-            self.patch_number is None
-        ))
+        return all(
+            (not self.is_development, self.minor_number == 0, self.patch_number is None)
+        )
 
     @property
     def is_stability(self):
         """Return `True` if `ShipItVersion` is a version that fixed a major one."""
-        return all((
-            not self.is_development,
-            not self.is_major,
-            self.minor_number != 0 or self.patch_number != 0,
-        ))
+        return all(
+            (
+                not self.is_development,
+                not self.is_major,
+                self.minor_number != 0 or self.patch_number != 0,
+            )
+        )
 
     @property
     def is_development(self):
         """Return `True` if `ShipItVersion` was known to require further development.
 
         It's usually a beta or before the rapid release scheme, a release candidate.
         """
```

### Comparing `mozilla_version-3.0.0/requirements/docs.txt` & `mozilla-version-3.1.0/requirements/docs.txt`

 * *Files 3% similar despite different names*

```diff
@@ -109,35 +109,35 @@
     --hash=sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519 \
     --hash=sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561
     # via requests
 docutils==0.20.1 \
     --hash=sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6 \
     --hash=sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b
     # via
-    #   -r requirements/docs.in
+    #   -r docs.in
     #   m2r2
     #   sphinx
 idna==3.7 \
     --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
     --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 imagesize==1.4.1 \
     --hash=sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b \
     --hash=sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a
     # via sphinx
-jinja2==3.1.3 \
-    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
-    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
+jinja2==3.1.4 \
+    --hash=sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369 \
+    --hash=sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d
     # via
     #   readthedocs-sphinx-ext
     #   sphinx
 m2r2==0.3.3.post2 \
     --hash=sha256:86157721eb6eabcd54d4eea7195890cc58fa6188b8d0abea633383cfbb5e11e3 \
     --hash=sha256:e62bcb0e74b3ce19cda0737a0556b04cf4a43b785072fcef474558f2c1482ca8
-    # via -r requirements/docs.in
+    # via -r docs.in
 markupsafe==2.1.5 \
     --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
     --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
     --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
     --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
     --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
     --hash=sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f \
@@ -209,29 +209,29 @@
 pygments==2.17.2 \
     --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
     --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
     # via sphinx
 readthedocs-sphinx-ext==2.2.5 \
     --hash=sha256:ee5fd5b99db9f0c180b2396cbce528aa36671951b9526bb0272dbfce5517bd27 \
     --hash=sha256:f8c56184ea011c972dd45a90122568587cc85b0127bc9cf064d17c68bc809daa
-    # via -r requirements/docs.in
+    # via -r docs.in
 requests==2.31.0 \
     --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
     --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
     #   readthedocs-sphinx-ext
     #   sphinx
 snowballstemmer==2.2.0 \
     --hash=sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1 \
     --hash=sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a
     # via sphinx
-sphinx==7.3.6 \
-    --hash=sha256:d6c09acd42094fcd96a9299c1b32b2dafe82d667fdd6e532e5978443ad074c2a \
-    --hash=sha256:fc9f3d13fed5c9a0e677d368090e209899ce5d0081eb552b657e2923e57517f0
-    # via -r requirements/docs.in
+sphinx==7.3.7 \
+    --hash=sha256:413f75440be4cacf328f580b4274ada4565fb2187d696a84970c23f77b64d8c3 \
+    --hash=sha256:a4a7db75ed37531c05002d56ed6948d4c42f473a36f46e1382b0bd76ca9627bc
+    # via -r docs.in
 sphinxcontrib-applehelp==1.0.8 \
     --hash=sha256:c40a4f96f3776c4393d933412053962fac2b84f4c99a7982ba42e09576a70619 \
     --hash=sha256:cb61eb0ec1b61f349e5cc36b2028e9e7ca765be05e49641c97241274753067b4
     # via sphinx
 sphinxcontrib-devhelp==1.0.6 \
     --hash=sha256:6485d09629944511c893fa11355bda18b742b83a2b181f9a009f7e500595c90f \
     --hash=sha256:9893fd3f90506bc4b97bdb977ceb8fbd823989f4316b28c3841ec128544372d3
```

### Comparing `mozilla_version-3.0.0/requirements/test.txt` & `mozilla-version-3.1.0/requirements/test.txt`

 * *Files 2% similar despite different names*

```diff
@@ -154,17 +154,17 @@
     --hash=sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e \
     --hash=sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2 \
     --hash=sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48 \
     --hash=sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4
     # via
     #   -r requirements/test.in
     #   pytest-cov
-exceptiongroup==1.2.0 \
-    --hash=sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14 \
-    --hash=sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68
+exceptiongroup==1.2.1 \
+    --hash=sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad \
+    --hash=sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16
     # via pytest
 flake8==7.0.0 \
     --hash=sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132 \
     --hash=sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3
     # via
     #   -r requirements/test.in
     #   flake8-docstrings
```

