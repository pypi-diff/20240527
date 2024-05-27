# Comparing `tmp/multiregex-2.0.2.tar.gz` & `tmp/multiregex-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiregex-2.0.2.tar", last modified: Thu May 23 16:12:15 2024, max compression
+gzip compressed data, was "multiregex-2.0.3.tar", last modified: Mon May 27 15:01:10 2024, max compression
```

## Comparing `multiregex-2.0.2.tar` & `multiregex-2.0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.212339 multiregex-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-23 16:12:09.000000 multiregex-2.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/ISSUE_TEMPLATE/issue-template.md
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-23 16:12:09.000000 multiregex-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-23 16:12:09.000000 multiregex-2.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-23 16:12:09.000000 multiregex-2.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-23 16:12:09.000000 multiregex-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-23 16:12:15.212339 multiregex-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-23 16:12:09.000000 multiregex-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-23 16:12:09.000000 multiregex-2.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-23 16:12:09.000000 multiregex-2.0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-23 16:12:09.000000 multiregex-2.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-23 16:12:09.000000 multiregex-2.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-23 16:12:09.000000 multiregex-2.0.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/multiregex/
--rw-r--r--   0 runner    (1001) docker     (127)    12776 2024-05-23 16:12:09.000000 multiregex-2.0.2/multiregex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:09.000000 multiregex-2.0.2/multiregex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/multiregex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-23 16:12:15.000000 multiregex-2.0.2/multiregex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-23 16:12:15.000000 multiregex-2.0.2/multiregex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:12:15.000000 multiregex-2.0.2/multiregex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 16:12:15.000000 multiregex-2.0.2/multiregex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 16:12:15.000000 multiregex-2.0.2/multiregex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)   171516 2024-05-23 16:12:09.000000 multiregex-2.0.2/pixi.lock
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-23 16:12:09.000000 multiregex-2.0.2/pixi.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-23 16:12:09.000000 multiregex-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 16:12:15.212339 multiregex-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-23 16:12:09.000000 multiregex-2.0.2/stubs/ahocorasick.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-23 16:12:09.000000 multiregex-2.0.2/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26689 2024-05-23 16:12:09.000000 multiregex-2.0.2/test_utils/cpython_test_re.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-23 16:12:09.000000 multiregex-2.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-23 16:12:09.000000 multiregex-2.0.2/tests/test_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-23 16:12:09.000000 multiregex-2.0.2/tests/test_cpython_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-23 16:12:09.000000 multiregex-2.0.2/tests/test_multiregex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:01:10.583390 multiregex-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-27 15:01:05.000000 multiregex-2.0.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:01:10.579390 multiregex-2.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 15:01:05.000000 multiregex-2.0.3/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:01:10.579390 multiregex-2.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 15:01:05.000000 multiregex-2.0.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 15:01:05.000000 multiregex-2.0.3/.github/ISSUE_TEMPLATE/issue-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-27 15:01:05.000000 multiregex-2.0.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-27 15:01:05.000000 multiregex-2.0.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:01:10.579390 multiregex-2.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-27 15:01:05.000000 multiregex-2.0.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-27 15:01:05.000000 multiregex-2.0.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-27 15:01:05.000000 multiregex-2.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-27 15:01:05.000000 multiregex-2.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-27 15:01:05.000000 multiregex-2.0.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-27 15:01:05.000000 multiregex-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-27 15:01:10.583390 multiregex-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-27 15:01:05.000000 multiregex-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:01:10.583390 multiregex-2.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-27 15:01:05.000000 multiregex-2.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-27 15:01:05.000000 multiregex-2.0.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-27 15:01:05.000000 multiregex-2.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-27 15:01:05.000000 multiregex-2.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-27 15:01:05.000000 multiregex-2.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:01:10.583390 multiregex-2.0.3/multiregex/
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-05-27 15:01:05.000000 multiregex-2.0.3/multiregex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:01:05.000000 multiregex-2.0.3/multiregex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:01:10.583390 multiregex-2.0.3/multiregex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-27 15:01:10.000000 multiregex-2.0.3/multiregex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 15:01:10.000000 multiregex-2.0.3/multiregex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:01:10.000000 multiregex-2.0.3/multiregex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 15:01:10.000000 multiregex-2.0.3/multiregex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 15:01:10.000000 multiregex-2.0.3/multiregex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171516 2024-05-27 15:01:05.000000 multiregex-2.0.3/pixi.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-27 15:01:05.000000 multiregex-2.0.3/pixi.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-27 15:01:05.000000 multiregex-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:01:10.583390 multiregex-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:01:10.583390 multiregex-2.0.3/stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-27 15:01:05.000000 multiregex-2.0.3/stubs/ahocorasick.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:01:10.583390 multiregex-2.0.3/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-27 15:01:05.000000 multiregex-2.0.3/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26689 2024-05-27 15:01:05.000000 multiregex-2.0.3/test_utils/cpython_test_re.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:01:10.583390 multiregex-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-27 15:01:05.000000 multiregex-2.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-27 15:01:05.000000 multiregex-2.0.3/tests/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-27 15:01:05.000000 multiregex-2.0.3/tests/test_cpython_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-27 15:01:05.000000 multiregex-2.0.3/tests/test_multiregex.py
```

### Comparing `multiregex-2.0.2/.github/workflows/build.yml` & `multiregex-2.0.3/.github/workflows/build.yml`

 * *Files 12% similar despite different names*

```diff
@@ -36,9 +36,13 @@
       id-token: write
     environment: pypi
     steps:
       - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
+      - name: Publish package on TestPyPi
+        uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450
+        with:
+          repository-url: https://test.pypi.org/legacy/
       - name: Publish package on PyPi
         uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450
```

### Comparing `multiregex-2.0.2/.github/workflows/ci.yml` & `multiregex-2.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/.gitignore` & `multiregex-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/.pre-commit-config.yaml` & `multiregex-2.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/CHANGELOG.rst` & `multiregex-2.0.3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/LICENSE` & `multiregex-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/PKG-INFO` & `multiregex-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiregex
-Version: 2.0.2
+Version: 2.0.3
 Summary: Quickly match many regexes against a string. Provides 2-10x speedups over naïve regex matching.
 Author-email: "QuantCo, Inc." <noreply@quantco.com>, Jonas Haag <jonas@lophus.org>
 Maintainer-email: Bela Stoyan <bela.stoyan@quantco.com>
 Project-URL: Home, https://github.com/quantco/multiregex
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `multiregex-2.0.2/README.md` & `multiregex-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/docs/Makefile` & `multiregex-2.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/docs/conf.py` & `multiregex-2.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/docs/make.bat` & `multiregex-2.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/multiregex/__init__.py` & `multiregex-2.0.3/multiregex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 `RegexMatcher.generate_prematchers`.  You must provide a handcrafted list of
 prematchers for regexes that this fails for.  You may also override the
 automatically generated prematchers.
 """
 
 import collections
 import functools
-import importlib
+import importlib.metadata
 import re
 import warnings
 
 try:
     sre_constants = re._constants  # type: ignore
     sre_parse = re._parser  # type: ignore
 except AttributeError:
```

### Comparing `multiregex-2.0.2/multiregex.egg-info/PKG-INFO` & `multiregex-2.0.3/multiregex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiregex
-Version: 2.0.2
+Version: 2.0.3
 Summary: Quickly match many regexes against a string. Provides 2-10x speedups over naïve regex matching.
 Author-email: "QuantCo, Inc." <noreply@quantco.com>, Jonas Haag <jonas@lophus.org>
 Maintainer-email: Bela Stoyan <bela.stoyan@quantco.com>
 Project-URL: Home, https://github.com/quantco/multiregex
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `multiregex-2.0.2/multiregex.egg-info/SOURCES.txt` & `multiregex-2.0.3/multiregex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/pixi.lock` & `multiregex-2.0.3/pixi.lock`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/pixi.toml` & `multiregex-2.0.3/pixi.toml`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/pyproject.toml` & `multiregex-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/test_utils/cpython_test_re.py` & `multiregex-2.0.3/test_utils/cpython_test_re.py`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/tests/test_bench.py` & `multiregex-2.0.3/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/tests/test_cpython_tests.py` & `multiregex-2.0.3/tests/test_cpython_tests.py`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.2/tests/test_multiregex.py` & `multiregex-2.0.3/tests/test_multiregex.py`

 * *Files identical despite different names*

