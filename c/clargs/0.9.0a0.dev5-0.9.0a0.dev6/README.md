# Comparing `tmp/clargs-0.9.0a0.dev5.tar.gz` & `tmp/clargs-0.9.0a0.dev6.tar.gz`

## Comparing `clargs-0.9.0a0.dev5.tar` & `clargs-0.9.0a0.dev6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/.github/workflows/run-tests-and-build.yml
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/examples/0_basic.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/examples/1_flags.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/examples/2_show_defaults.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/examples/3_list.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/examples/4_parse_groups.py
--rw-r--r--   0        0        0    20371 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/examples/5_logging.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/examples/6_validation.py
--rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/examples/__generate_example_output__.sh
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/src/clargs/__about__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/src/clargs/__init__.py
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/src/clargs/aap_from_data.py
--rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/src/clargs/clargs.py
--rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/src/clargs/docsparser.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/src/clargs/helper_types.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/tests/__init__.py
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/tests/test_docsparser.py
--rw-r--r--   0        0        0    26301 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/tests/test_simple.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/tests/test_validation.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/LICENSE.txt
--rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/README.md
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/pyproject.toml
--rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev5/PKG-INFO
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/.github/workflows/run-tests-and-build.yml
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/examples/0_basic.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/examples/1_flags.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/examples/2_show_defaults.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/examples/3_list.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/examples/4_parse_groups.py
+-rw-r--r--   0        0        0    20371 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/examples/5_logging.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/examples/6_validation.py
+-rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/examples/__generate_example_output__.sh
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/src/clargs/__about__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/src/clargs/__init__.py
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/src/clargs/aap_from_data.py
+-rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/src/clargs/clargs.py
+-rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/src/clargs/docsparser.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/src/clargs/helper_types.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/tests/__init__.py
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/tests/test_docsparser.py
+-rw-r--r--   0        0        0    26301 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/tests/test_simple.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/tests/test_validation.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/LICENSE.txt
+-rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/README.md
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev6/PKG-INFO
```

### Comparing `clargs-0.9.0a0.dev5/.github/workflows/publish.yaml` & `clargs-0.9.0a0.dev6/.github/workflows/publish.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Upload to PyPI
+name: Upload to PyPI and Tag
 
 on:
   push:
     branches:
       - "hatch"
     paths:
       - 'src/clargs/__about__.py'
@@ -11,27 +11,38 @@
 
 jobs:
   test-and-build:
     uses: ./.github/workflows/run-tests-and-build.yml
 
   upload:
     needs: test-and-build
-    name: Upload release to PyPI
+    name: Publish release to PyPI
     runs-on: ubuntu-latest
     environment:
       name: pypi
       url: https://pypi.org/p/clargs
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
-    - uses: actions/checkout@v4
     - uses: actions/download-artifact@v4
       with:
         name: distribution-package
         path: dist
     - name: Publish package distributions to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
+  tag:
+    needs: upload
+    name: Create a release tag in git
+    runs-on: ubuntu-latest
+    permissions:
+      contents: write
+    steps:
+    - uses: actions/checkout@v4
+    - uses: actions/download-artifact@v4
+      with:
+        name: distribution-package
+        path: dist
     - name: Tag version and push
       run:  |
-          VERSION="PACKAGE/v$(ls -1 dist/*.whl | head | cut -f2 -d-)"
+          VERSION="RELEASE/v$(ls -1 dist/*.whl | head | cut -f2 -d-)"
           git tag "${VERSION}"
           git push --tags
```

### Comparing `clargs-0.9.0a0.dev5/.github/workflows/run-tests-and-build.yml` & `clargs-0.9.0a0.dev6/.github/workflows/run-tests-and-build.yml`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/examples/0_basic.py` & `clargs-0.9.0a0.dev6/examples/0_basic.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/examples/1_flags.py` & `clargs-0.9.0a0.dev6/examples/1_flags.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/examples/2_show_defaults.py` & `clargs-0.9.0a0.dev6/examples/2_show_defaults.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/examples/3_list.py` & `clargs-0.9.0a0.dev6/examples/3_list.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/examples/4_parse_groups.py` & `clargs-0.9.0a0.dev6/examples/4_parse_groups.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/examples/5_logging.py` & `clargs-0.9.0a0.dev6/examples/5_logging.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/examples/6_validation.py` & `clargs-0.9.0a0.dev6/examples/6_validation.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/examples/__generate_example_output__.sh` & `clargs-0.9.0a0.dev6/examples/__generate_example_output__.sh`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/src/clargs/__init__.py` & `clargs-0.9.0a0.dev6/src/clargs/__init__.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/src/clargs/aap_from_data.py` & `clargs-0.9.0a0.dev6/src/clargs/aap_from_data.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/src/clargs/clargs.py` & `clargs-0.9.0a0.dev6/src/clargs/clargs.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/src/clargs/docsparser.py` & `clargs-0.9.0a0.dev6/src/clargs/docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/src/clargs/helper_types.py` & `clargs-0.9.0a0.dev6/src/clargs/helper_types.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/tests/test_docsparser.py` & `clargs-0.9.0a0.dev6/tests/test_docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/tests/test_simple.py` & `clargs-0.9.0a0.dev6/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/tests/test_validation.py` & `clargs-0.9.0a0.dev6/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/LICENSE.txt` & `clargs-0.9.0a0.dev6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/README.md` & `clargs-0.9.0a0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/pyproject.toml` & `clargs-0.9.0a0.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0a0.dev5/PKG-INFO` & `clargs-0.9.0a0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: clargs
-Version: 0.9.0a0.dev5
+Version: 0.9.0a0.dev6
 Summary: Easily generate commandline apps from your functions, based on type hints
 Project-URL: Documentation, https://github.com/reinhrst/clargs#readme
 Project-URL: Issues, https://github.com/reinhrst/clargs/issues
 Project-URL: Source, https://github.com/reinhrst/clargs
 Author-email: Claude <pypi@claude.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

