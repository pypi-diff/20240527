# Comparing `tmp/bats_core_pkg-0.1.2.tar.gz` & `tmp/bats_core_pkg-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bats_core_pkg-0.1.2.tar", max compression
+gzip compressed data, was "bats_core_pkg-0.1.3.tar", max compression
```

## Comparing `bats_core_pkg-0.1.2.tar` & `bats_core_pkg-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1247 2022-12-23 16:10:57.981463 bats_core_pkg-0.1.2/LICENSE.md
--rw-r--r--   0        0        0       77 2022-12-23 16:35:38.179226 bats_core_pkg-0.1.2/README.md
--rw-r--r--   0        0        0      325 2022-12-23 16:59:19.687580 bats_core_pkg-0.1.2/bats_core_pkg/__init__.py
--rw-r--r--   0        0        0      219 2022-10-19 21:37:47.000000 bats_core_pkg-0.1.2/bats_core_pkg/dist/AUTHORS
--rw-r--r--   0        0        0     2535 2022-10-19 21:37:47.000000 bats_core_pkg-0.1.2/bats_core_pkg/dist/LICENSE.md
--rwxr-xr-x   0        0        0     1671 2022-12-23 16:28:14.679291 bats_core_pkg-0.1.2/bats_core_pkg/dist/bin/bats
--rwxr-xr-x   0        0        0     6706 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/common.bash
--rwxr-xr-x   0        0        0     5822 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/formatter.bash
--rwxr-xr-x   0        0        0      777 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/preprocessing.bash
--rwxr-xr-x   0        0        0     3612 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/semaphore.bash
--rwxr-xr-x   0        0        0    10512 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/test_functions.bash
--rwxr-xr-x   0        0        0    13933 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/tracing.bash
--rwxr-xr-x   0        0        0     1019 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/validator.bash
--rwxr-xr-x   0        0        0     1891 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/warnings.bash
--rwxr-xr-x   0        0        0    13572 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats
--rwxr-xr-x   0        0        0    11248 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-exec-file
--rwxr-xr-x   0        0        0    13107 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-exec-suite
--rwxr-xr-x   0        0        0    10318 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-exec-test
--rwxr-xr-x   0        0        0       45 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-format-cat
--rwxr-xr-x   0        0        0     6140 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-format-junit
--rwxr-xr-x   0        0        0     6498 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-format-pretty
--rwxr-xr-x   0        0        0     1256 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-format-tap
--rwxr-xr-x   0        0        0     2115 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-format-tap13
--rwxr-xr-x   0        0        0     3751 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-preprocess
--rw-r--r--   0        0        0      780 2022-12-23 16:59:46.303589 bats_core_pkg-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 bats_core_pkg-0.1.2/setup.py
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 bats_core_pkg-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1247 2022-12-23 16:10:57.981463 bats_core_pkg-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0       77 2022-12-23 16:35:38.179226 bats_core_pkg-0.1.3/README.md
+-rw-r--r--   0        0        0      325 2022-12-23 16:59:19.687580 bats_core_pkg-0.1.3/bats_core_pkg/__init__.py
+-rw-r--r--   0        0        0      219 2022-10-19 21:37:47.000000 bats_core_pkg-0.1.3/bats_core_pkg/dist/AUTHORS
+-rw-r--r--   0        0        0     2535 2022-10-19 21:37:47.000000 bats_core_pkg-0.1.3/bats_core_pkg/dist/LICENSE.md
+-rwxr-xr-x   0        0        0     1671 2022-12-23 16:28:14.679291 bats_core_pkg-0.1.3/bats_core_pkg/dist/bin/bats
+-rwxr-xr-x   0        0        0     6706 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/common.bash
+-rwxr-xr-x   0        0        0     5822 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/formatter.bash
+-rwxr-xr-x   0        0        0      777 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/preprocessing.bash
+-rwxr-xr-x   0        0        0     3612 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/semaphore.bash
+-rwxr-xr-x   0        0        0    10512 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/test_functions.bash
+-rwxr-xr-x   0        0        0    13933 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/tracing.bash
+-rwxr-xr-x   0        0        0     1019 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/validator.bash
+-rwxr-xr-x   0        0        0     1891 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/warnings.bash
+-rwxr-xr-x   0        0        0    13572 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats
+-rwxr-xr-x   0        0        0    11248 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-exec-file
+-rwxr-xr-x   0        0        0    13107 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-exec-suite
+-rwxr-xr-x   0        0        0    10318 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-exec-test
+-rwxr-xr-x   0        0        0       45 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-format-cat
+-rwxr-xr-x   0        0        0     6140 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-format-junit
+-rwxr-xr-x   0        0        0     6498 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-format-pretty
+-rwxr-xr-x   0        0        0     1256 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-format-tap
+-rwxr-xr-x   0        0        0     2115 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-format-tap13
+-rwxr-xr-x   0        0        0     3751 2022-12-23 16:28:14.683291 bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-preprocess
+-rw-r--r--   0        0        0      779 2022-12-23 17:06:02.611719 bats_core_pkg-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 bats_core_pkg-0.1.3/setup.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 bats_core_pkg-0.1.3/PKG-INFO
```

### Comparing `bats_core_pkg-0.1.2/LICENSE.md` & `bats_core_pkg-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/LICENSE.md` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/bin/bats` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/bin/bats`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/common.bash` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/common.bash`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/formatter.bash` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/formatter.bash`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/preprocessing.bash` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/preprocessing.bash`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/semaphore.bash` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/semaphore.bash`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/test_functions.bash` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/test_functions.bash`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/tracing.bash` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/tracing.bash`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/validator.bash` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/validator.bash`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/lib/bats-core/warnings.bash` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/lib/bats-core/warnings.bash`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-exec-file` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-exec-file`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-exec-suite` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-exec-suite`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-exec-test` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-exec-test`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-format-junit` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-format-junit`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-format-pretty` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-format-pretty`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-format-tap` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-format-tap`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-format-tap13` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-format-tap13`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/bats_core_pkg/dist/libexec/bats-core/bats-preprocess` & `bats_core_pkg-0.1.3/bats_core_pkg/dist/libexec/bats-core/bats-preprocess`

 * *Files identical despite different names*

### Comparing `bats_core_pkg-0.1.2/pyproject.toml` & `bats_core_pkg-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bats-core-pkg"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python wrapper on tops of bats-core"
 authors = ["David Caro <dcaro@wikimedia.org>"]
 homepage = "https://github.com/david-caro/bats-core-pkg"
 repository = "https://github.com/david-caro/bats-core-pkg"
 license = "MIT"
 classifiers = [
     "Topic :: Software Development :: Build Tools",
@@ -18,13 +18,13 @@
     "bats_core_pkg/dist/*",
 ]
 
 [tool.poetry.scripts]
 bats_core_pkg = 'bats_core_pkg:main'
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.7"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bats_core_pkg-0.1.2/setup.py` & `bats_core_pkg-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,23 @@
                    'dist/libexec/bats-core/*']}
 
 entry_points = \
 {'console_scripts': ['bats_core_pkg = bats_core_pkg:main']}
 
 setup_kwargs = {
     'name': 'bats-core-pkg',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Python wrapper on tops of bats-core',
     'long_description': '# bats-core-pkg\nSimple wrapper to bats-core to be able to pull it from pypi.\n',
     'author': 'David Caro',
     'author_email': 'dcaro@wikimedia.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/david-caro/bats-core-pkg',
     'packages': packages,
     'package_data': package_data,
     'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `bats_core_pkg-0.1.2/PKG-INFO` & `bats_core_pkg-0.1.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: bats-core-pkg
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrapper on tops of bats-core
 Home-page: https://github.com/david-caro/bats-core-pkg
 License: MIT
 Author: David Caro
 Author-email: dcaro@wikimedia.org
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/david-caro/bats-core-pkg
 Description-Content-Type: text/markdown
```

