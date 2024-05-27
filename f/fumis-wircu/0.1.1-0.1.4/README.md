# Comparing `tmp/fumis_wircu-0.1.1.tar.gz` & `tmp/fumis_wircu-0.1.4.tar.gz`

## Comparing `fumis_wircu-0.1.1.tar` & `fumis_wircu-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/.editorconfig
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/.flake8
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/.gitattributes
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/.isort.cfg
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/.yamllint
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/MANIFEST.in
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/Makefile
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/mypi.ini
--rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/pylintrc
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/requirements.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/requirements_dev.txt
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/requirements_test.txt
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/tox.ini
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/examples/control.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/fumis_wircu/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/fumis_wircu/__version__.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/fumis_wircu/const.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/fumis_wircu/exceptions.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/fumis_wircu/fumis.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/fumis_wircu/models.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/tests/test_actions.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/tests/test_formula.py
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/tests/test_info.py
--rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/tests/test_request.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/tests/fixtures/info.json
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/README.md
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/hatch_build.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 fumis_wircu-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/.editorconfig
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/.flake8
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/.gitattributes
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/.isort.cfg
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/.yamllint
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/Makefile
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/mypi.ini
+-rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/pylintrc
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/requirements.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/requirements_dev.txt
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/requirements_test.txt
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/tox.ini
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/examples/control.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/fumis_wircu/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/fumis_wircu/__version__.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/fumis_wircu/const.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/fumis_wircu/exceptions.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/fumis_wircu/fumis.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/fumis_wircu/models.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/tests/test_actions.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/tests/test_formula.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/tests/test_info.py
+-rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/tests/test_request.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/tests/fixtures/info.json
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/README.md
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/hatch_build.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 fumis_wircu-0.1.4/PKG-INFO
```

### Comparing `fumis_wircu-0.1.1/.pre-commit-config.yaml` & `fumis_wircu-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/.yamllint` & `fumis_wircu-0.1.4/.yamllint`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/CODE_OF_CONDUCT.md` & `fumis_wircu-0.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/CONTRIBUTING.md` & `fumis_wircu-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/Makefile` & `fumis_wircu-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/mypi.ini` & `fumis_wircu-0.1.4/mypi.ini`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/pylintrc` & `fumis_wircu-0.1.4/pylintrc`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/tox.ini` & `fumis_wircu-0.1.4/tox.ini`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/.github/workflows/ci.yml` & `fumis_wircu-0.1.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/fumis_wircu/fumis.py` & `fumis_wircu-0.1.4/fumis_wircu/fumis.py`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/fumis_wircu/models.py` & `fumis_wircu-0.1.4/fumis_wircu/models.py`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/tests/test_actions.py` & `fumis_wircu-0.1.4/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/tests/test_info.py` & `fumis_wircu-0.1.4/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/tests/test_request.py` & `fumis_wircu-0.1.4/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/tests/fixtures/info.json` & `fumis_wircu-0.1.4/tests/fixtures/info.json`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/.gitignore` & `fumis_wircu-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/LICENSE.md` & `fumis_wircu-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/README.md` & `fumis_wircu-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/hatch_build.py` & `fumis_wircu-0.1.4/hatch_build.py`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/pyproject.toml` & `fumis_wircu-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fumis_wircu-0.1.1/PKG-INFO` & `fumis_wircu-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fumis_wircu
-Version: 0.1.1
+Version: 0.1.4
 Summary: Asynchronous Python client for the Fumis WiRCU API.
 Project-URL: Homepage, https://github.com/aaronmunsters/fumis_wircu
 Project-URL: Issues, https://github.com/aaronmunsters/fumis_wircu/issues
 Author: Aäron Munsters
 Author-email: Franck Nijhof <frenck@frenck.dev>
 Maintainer: Aäron Munsters
 License-Expression: MIT
```

