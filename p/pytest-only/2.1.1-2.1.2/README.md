# Comparing `tmp/pytest_only-2.1.1.tar.gz` & `tmp/pytest_only-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_only-2.1.1.tar", max compression
+gzip compressed data, was "pytest_only-2.1.2.tar", max compression
```

## Comparing `pytest_only-2.1.1.tar` & `pytest_only-2.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3909 2022-06-14 07:29:34.538995 pytest_only-2.1.1/README.rst
--rw-r--r--   0        0        0     1198 2024-03-09 18:01:01.039328 pytest_only-2.1.1/pyproject.toml
--rw-r--r--   0        0        0       54 2022-05-29 08:02:31.761250 pytest_only-2.1.1/pytest_only/__init__.py
--rw-r--r--   0        0        0      560 2022-05-29 21:56:51.065510 pytest_only-2.1.1/pytest_only/compat.py
--rw-r--r--   0        0        0        0 2022-06-14 07:17:21.860122 pytest_only-2.1.1/pytest_only/ext/__init__.py
--rw-r--r--   0        0        0     4246 2024-03-09 17:57:10.150594 pytest_only-2.1.1/pytest_only/ext/flake8.py
--rw-r--r--   0        0        0     2932 2022-06-14 07:17:21.860122 pytest_only-2.1.1/pytest_only/ext/pylint.py
--rw-r--r--   0        0        0      895 2022-05-29 08:02:31.761250 pytest_only-2.1.1/pytest_only/plugin.py
--rw-r--r--   0        0        0      166 2022-05-29 08:50:19.330070 pytest_only-2.1.1/pytest_only/version.py
--rw-r--r--   0        0        0     4967 1970-01-01 00:00:00.000000 pytest_only-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3909 2022-06-14 07:29:34.538995 pytest_only-2.1.2/README.rst
+-rw-r--r--   0        0        0     1116 2024-05-27 17:03:55.928782 pytest_only-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0       54 2022-05-29 08:02:31.761250 pytest_only-2.1.2/pytest_only/__init__.py
+-rw-r--r--   0        0        0      560 2022-05-29 21:56:51.065510 pytest_only-2.1.2/pytest_only/compat.py
+-rw-r--r--   0        0        0        0 2022-06-14 07:17:21.860122 pytest_only-2.1.2/pytest_only/ext/__init__.py
+-rw-r--r--   0        0        0     4246 2024-03-09 17:57:10.150594 pytest_only-2.1.2/pytest_only/ext/flake8.py
+-rw-r--r--   0        0        0     2932 2022-06-14 07:17:21.860122 pytest_only-2.1.2/pytest_only/ext/pylint.py
+-rw-r--r--   0        0        0      895 2022-05-29 08:02:31.761250 pytest_only-2.1.2/pytest_only/plugin.py
+-rw-r--r--   0        0        0      166 2022-05-29 08:50:19.330070 pytest_only-2.1.2/pytest_only/version.py
+-rw-r--r--   0        0        0     4857 1970-01-01 00:00:00.000000 pytest_only-2.1.2/PKG-INFO
```

### Comparing `pytest_only-2.1.1/README.rst` & `pytest_only-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_only-2.1.1/pyproject.toml` & `pytest_only-2.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'pytest-only'
-version = "2.1.1"
+version = "2.1.2"
 description = 'Use @pytest.mark.only to run a single test'
 authors = ['Zach Kanzler <they4kman@gmail.com>']
 license = 'MIT'
 
 readme = 'README.rst'
 
 repository = 'https://github.com/theY4Kman/pytest-only'
@@ -16,23 +16,20 @@
     'Programming Language :: Python',
     'Framework :: Pytest',
     'License :: OSI Approved :: MIT License',
     'Topic :: Software Development :: Testing',
 ]
 
 [tool.poetry.dependencies]
-python = '>=3.7.2,<4'
-pytest = [
-    {version = '<7.1', python = '<= 3.6'},
-    {version = '>=7.1', python = '^3.7'},
-]
+python = '^3.8'
+pytest = '>=3.6.0,<9'
 
 [tool.poetry.group.dev.dependencies]
 flake8 = [
-    {version = '5.0.4', python = '>=3.7,<3.8.1'},
+    {version = '5.0.4', python = '>=3.8,<3.8.1'},
     {version = '^7.0.0', python = '>=3.8.1'},
 ]
 pylint = "^2.13.9"
 pytest-common-subject = "^1.0.6"
 pytest-pylint = "^0.21.0"
 tox = '^3.25.0'
```

### Comparing `pytest_only-2.1.1/pytest_only/compat.py` & `pytest_only-2.1.2/pytest_only/compat.py`

 * *Files identical despite different names*

### Comparing `pytest_only-2.1.1/pytest_only/ext/flake8.py` & `pytest_only-2.1.2/pytest_only/ext/flake8.py`

 * *Files identical despite different names*

### Comparing `pytest_only-2.1.1/pytest_only/ext/pylint.py` & `pytest_only-2.1.2/pytest_only/ext/pylint.py`

 * *Files identical despite different names*

### Comparing `pytest_only-2.1.1/pytest_only/plugin.py` & `pytest_only-2.1.2/pytest_only/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_only-2.1.1/PKG-INFO` & `pytest_only-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: pytest-only
-Version: 2.1.1
+Version: 2.1.2
 Summary: Use @pytest.mark.only to run a single test
 Home-page: https://github.com/theY4Kman/pytest-only
 License: MIT
 Keywords: pytest
 Author: Zach Kanzler
 Author-email: they4kman@gmail.com
-Requires-Python: >=3.7.2,<4
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest (<7.1) ; python_full_version <= "3.6.0"
-Requires-Dist: pytest (>=7.1) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: pytest (>=3.6.0,<9)
 Project-URL: Repository, https://github.com/theY4Kman/pytest-only
 Description-Content-Type: text/x-rst
 
 pytest-only
 ===========
 
 Only run tests marked with ``@pytest.mark.only``. If none are marked, all tests run as usual.
```

