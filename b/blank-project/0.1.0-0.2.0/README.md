# Comparing `tmp/blank_project-0.1.0.tar.gz` & `tmp/blank_project-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "blank_project-0.2.0.tar", last modified: Mon May 27 04:19:59 2024, max compression
```

## Comparing `blank_project-0.1.0.tar` & `blank_project-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,16 @@
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 blank_project-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 blank_project-0.1.0/Makefile
--rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 blank_project-0.1.0/init.sh
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 blank_project-0.1.0/blank_project/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 blank_project-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 blank_project-0.1.0/tests/test_package_version.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 blank_project-0.1.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 blank_project-0.1.0/LICENSE
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 blank_project-0.1.0/README.md
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 blank_project-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 blank_project-0.1.0/PKG-INFO
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-27 04:19:59.716996 blank_project-0.2.0/
+-rw-r--r--   0 peter      (501) staff       (20)     1087 2024-05-18 03:06:00.000000 blank_project-0.2.0/LICENSE
+-rw-r--r--   0 peter      (501) staff       (20)     4363 2024-05-27 04:19:59.716342 blank_project-0.2.0/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)     2668 2024-05-27 04:18:41.000000 blank_project-0.2.0/README.md
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-27 04:19:59.710851 blank_project-0.2.0/blank_project/
+-rw-r--r--   0 peter      (501) staff       (20)      136 2024-05-27 04:18:41.000000 blank_project-0.2.0/blank_project/__init__.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-27 04:19:59.713962 blank_project-0.2.0/blank_project.egg-info/
+-rw-r--r--   0 peter      (501) staff       (20)     4363 2024-05-27 04:19:59.000000 blank_project-0.2.0/blank_project.egg-info/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)      272 2024-05-27 04:19:59.000000 blank_project-0.2.0/blank_project.egg-info/SOURCES.txt
+-rw-r--r--   0 peter      (501) staff       (20)        1 2024-05-27 04:19:59.000000 blank_project-0.2.0/blank_project.egg-info/dependency_links.txt
+-rw-r--r--   0 peter      (501) staff       (20)      131 2024-05-27 04:19:59.000000 blank_project-0.2.0/blank_project.egg-info/requires.txt
+-rw-r--r--   0 peter      (501) staff       (20)       14 2024-05-27 04:19:59.000000 blank_project-0.2.0/blank_project.egg-info/top_level.txt
+-rw-r--r--   0 peter      (501) staff       (20)     2143 2024-05-27 04:18:41.000000 blank_project-0.2.0/pyproject.toml
+-rw-r--r--   0 peter      (501) staff       (20)       38 2024-05-27 04:19:59.717125 blank_project-0.2.0/setup.cfg
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-27 04:19:59.713376 blank_project-0.2.0/tests/
+-rw-r--r--   0 peter      (501) staff       (20)      169 2024-05-27 04:18:41.000000 blank_project-0.2.0/tests/test_package_version.py
```

### Comparing `blank_project-0.1.0/LICENSE` & `blank_project-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blank_project-0.1.0/README.md` & `blank_project-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # blank-project
 
-<!-- ![Build Status](https://github.com/<username>/<reponame>/actions/workflows/ci.yaml/badge.svg?branch=master) -->
-<!-- ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/<reponame>) -->
-<!-- ![PyPI Version](https://img.shields.io/pypi/v/<reponame>) -->
-<!-- [![Code Coverage](https://codecov.io/gh/<username>/<reponame>/graph/badge.svg?token=<token>)](https://codecov.io/gh/<username>/<reponame>) -->
-<!-- [![Maintainability](https://api.codeclimate.com/v1/badges/<id>/maintainability)](https://codeclimate.com/github/<username>/<reponame>/maintainability) -->
+![Build Status](https://github.com/p3t3rbr0/py3-blank-project/actions/workflows/ci.yaml/badge.svg?branch=master)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/blank-project)
+![PyPI Version](https://img.shields.io/pypi/v/blank-project)
+[![Code Coverage](https://codecov.io/github/p3t3rbr0/py3-blank-project/graph/badge.svg?token=CYSG54XRPR)](https://codecov.io/github/p3t3rbr0/py3-blank-project)
+[![Maintainability](https://api.codeclimate.com/v1/badges/b0a123a1539122f6a119/maintainability)](https://codeclimate.com/github/p3t3rbr0/py3-blank-project/maintainability)
 
 A dummy package for quickly starting typical Python projects.
 
 Features:
 
 * Basic `.gitignore`;
 * GitHub actions for builds and checks;
 * Acceptable directory structure at once;
 * Regular automation based on a `Makefile`;
-* Templates for basic python badges into `README.md`.
+* Templates for basic Python badges into `README.md`.
 * Single point of project specification - `pyproject.toml`;
 * Acceptable settings for: `black`, `isort`, `flake8`, `mypy`, `pydocstyle` and `coverage`;
 
 ## Usage
 
 1. Clone repo:
 
@@ -45,32 +45,34 @@
 $ rm -f init.sh
 ```
 
 5. Change `authors`, `description`, `keywords` and `classifiers` into **pyproject.toml**.
 
 6. Change `README.md`, `CHANGELOG.md` and `LICENSE` files.
 
-A new blank python project is ready, create gh-repo and go forward!
+7. Change "dunders" (`author`, `version` and `license`) in `<package>.__init__.py`.
+
+A new blank Python project is ready, create gh-repo and go forward!
 
 ## Available make commands
 
 ### Dependencies
 
 - `make deps-dev` - Install only development dependencies.
 - `make deps-build` - Install only build system dependencies.
 - `make deps` - Install all dependencies.
 
 ### Distributing
 
 - `make build-sdist` - Build a source distrib.
-- `make build-wheel` - Build a pure python wheel distrib.
+- `make build-wheel` - Build a pure Python wheel distrib.
 - `make build` - Build both distribs (source and wheel).
 - `make upload` - Upload built packages to PyPI.
 
 ### Development
 
-- `make cleanup` - Clean up python temporary files and caches.
+- `make cleanup` - Clean up Python temporary files and caches.
 - `make format` - Fromat the code (by black and isort).
 - `make lint` - Check code style, docstring style and types (by flake8, pydocstyle and mypy).
 - `make tests` - Run tests with coverage measure (output to terminal).
 - `make tests-cov-json` - Run tests with coverage measure (output to json [coverage.json]).
 - `make tests-cov-html` - Run tests with coverage measure (output to html [coverage_report/]).
```

### Comparing `blank_project-0.1.0/pyproject.toml` & `blank_project-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 [build-system]
-requires = ["hatchling==1.24.2"]
-build-backend = "hatchling.build"
+requires = ["setuptools==70.0.0"]
+build-backend = "setuptools.build_meta"
 
-[tool.hatch.version]
-path = "blank_project/__init__.py"
+[tool.setuptools]
+packages = ["blank_project"]
+
+[tool.setuptools.dynamic]
+version = {attr = "blank_project.__version__"}
+
+[tool.setuptools.package-data]
+blank_project = ["py.typed"]
 
 [project]
 name = "blank-project"
 dynamic = ["version"]
 authors = [
   {name = "Peter Bro", email = "p3t3rbr0@gmail.com"},
 ]
 description = "A dummy package for quickly starting typical Python projects."
 keywords = ["utility", "dummy package"]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -44,22 +50,14 @@
     "mypy==1.10.0",
     "isort==5.13.2",
     "flake8==7.0.0",
     "black==24.4.2",
     "pydocstyle==6.3.0",
 ]
 
-[tool.hatch.build.targets.wheel]
-include = ["*.py"]
-exclude = ["venv", "tests", ".*", "coverage*"]
-
-[tool.hatch.build.targets.sdist]
-ignore-vcs = true
-exclude = ["venv", ".*", "coverage*"]
-
 [tool.mypy]
 exclude = ["tests"]
 ignore_missing_imports = true
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
```

### Comparing `blank_project-0.1.0/PKG-INFO` & `blank_project-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: blank-project
-Version: 0.1.0
+Version: 0.2.0
 Summary: A dummy package for quickly starting typical Python projects.
+Author-email: Peter Bro <p3t3rbr0@gmail.com>
 Project-URL: Homepage, https://github.com/p3t3rbr0/py3-blank-project
 Project-URL: Documentation, https://github.com/p3t3rbr0/py3-blank-project/blob/master/README.md
 Project-URL: Repository, https://github.com/p3t3rbr0/py3-blank-project.git
 Project-URL: Issues, https://github.com/p3t3rbr0/py3-blank-project/issues
 Project-URL: Changelog, https://github.com/p3t3rbr0/py3-blank-project/blob/master/CHANGELOG.md
-Author-email: Peter Bro <p3t3rbr0@gmail.com>
-License-File: LICENSE
-Keywords: dummy package,utility
-Classifier: Development Status :: 1 - Planning
+Keywords: utility,dummy package
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
 Provides-Extra: build
-Requires-Dist: build==1.2.1; extra == 'build'
-Requires-Dist: twine==5.0.0; extra == 'build'
+Requires-Dist: build==1.2.1; extra == "build"
+Requires-Dist: twine==5.0.0; extra == "build"
 Provides-Extra: dev
-Requires-Dist: black==24.4.2; extra == 'dev'
-Requires-Dist: coverage==7.5.1; extra == 'dev'
-Requires-Dist: flake8==7.0.0; extra == 'dev'
-Requires-Dist: isort==5.13.2; extra == 'dev'
-Requires-Dist: mypy==1.10.0; extra == 'dev'
-Requires-Dist: pydocstyle==6.3.0; extra == 'dev'
-Description-Content-Type: text/markdown
+Requires-Dist: coverage==7.5.1; extra == "dev"
+Requires-Dist: mypy==1.10.0; extra == "dev"
+Requires-Dist: isort==5.13.2; extra == "dev"
+Requires-Dist: flake8==7.0.0; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
+Requires-Dist: pydocstyle==6.3.0; extra == "dev"
 
 # blank-project
 
-<!-- ![Build Status](https://github.com/<username>/<reponame>/actions/workflows/ci.yaml/badge.svg?branch=master) -->
-<!-- ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/<reponame>) -->
-<!-- ![PyPI Version](https://img.shields.io/pypi/v/<reponame>) -->
-<!-- [![Code Coverage](https://codecov.io/gh/<username>/<reponame>/graph/badge.svg?token=<token>)](https://codecov.io/gh/<username>/<reponame>) -->
-<!-- [![Maintainability](https://api.codeclimate.com/v1/badges/<id>/maintainability)](https://codeclimate.com/github/<username>/<reponame>/maintainability) -->
+![Build Status](https://github.com/p3t3rbr0/py3-blank-project/actions/workflows/ci.yaml/badge.svg?branch=master)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/blank-project)
+![PyPI Version](https://img.shields.io/pypi/v/blank-project)
+[![Code Coverage](https://codecov.io/github/p3t3rbr0/py3-blank-project/graph/badge.svg?token=CYSG54XRPR)](https://codecov.io/github/p3t3rbr0/py3-blank-project)
+[![Maintainability](https://api.codeclimate.com/v1/badges/b0a123a1539122f6a119/maintainability)](https://codeclimate.com/github/p3t3rbr0/py3-blank-project/maintainability)
 
 A dummy package for quickly starting typical Python projects.
 
 Features:
 
 * Basic `.gitignore`;
 * GitHub actions for builds and checks;
 * Acceptable directory structure at once;
 * Regular automation based on a `Makefile`;
-* Templates for basic python badges into `README.md`.
+* Templates for basic Python badges into `README.md`.
 * Single point of project specification - `pyproject.toml`;
 * Acceptable settings for: `black`, `isort`, `flake8`, `mypy`, `pydocstyle` and `coverage`;
 
 ## Usage
 
 1. Clone repo:
 
@@ -82,32 +82,34 @@
 $ rm -f init.sh
 ```
 
 5. Change `authors`, `description`, `keywords` and `classifiers` into **pyproject.toml**.
 
 6. Change `README.md`, `CHANGELOG.md` and `LICENSE` files.
 
-A new blank python project is ready, create gh-repo and go forward!
+7. Change "dunders" (`author`, `version` and `license`) in `<package>.__init__.py`.
+
+A new blank Python project is ready, create gh-repo and go forward!
 
 ## Available make commands
 
 ### Dependencies
 
 - `make deps-dev` - Install only development dependencies.
 - `make deps-build` - Install only build system dependencies.
 - `make deps` - Install all dependencies.
 
 ### Distributing
 
 - `make build-sdist` - Build a source distrib.
-- `make build-wheel` - Build a pure python wheel distrib.
+- `make build-wheel` - Build a pure Python wheel distrib.
 - `make build` - Build both distribs (source and wheel).
 - `make upload` - Upload built packages to PyPI.
 
 ### Development
 
-- `make cleanup` - Clean up python temporary files and caches.
+- `make cleanup` - Clean up Python temporary files and caches.
 - `make format` - Fromat the code (by black and isort).
 - `make lint` - Check code style, docstring style and types (by flake8, pydocstyle and mypy).
 - `make tests` - Run tests with coverage measure (output to terminal).
 - `make tests-cov-json` - Run tests with coverage measure (output to json [coverage.json]).
 - `make tests-cov-html` - Run tests with coverage measure (output to html [coverage_report/]).
```

