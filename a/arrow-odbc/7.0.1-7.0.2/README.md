# Comparing `tmp/arrow_odbc-7.0.1.tar.gz` & `tmp/arrow_odbc-7.0.2.tar.gz`

## Comparing `arrow_odbc-7.0.1.tar` & `arrow_odbc-7.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 arrow_odbc-7.0.1/Cargo.toml
--rw-r--r--   0      501       20      136 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/.gitattributes
--rw-r--r--   0      501       20      213 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/.github/dependabot.yml
--rw-r--r--   0      501       20     1762 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/.github/workflows/test.yml
--rw-r--r--   0      501       20     2654 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/.github/workflows/wheel.yml
--rw-r--r--   0      501       20      286 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/.gitignore
--rw-r--r--   0      501       20      841 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/.readthedocs.yaml
--rw-r--r--   0      501       20    12114 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/Changelog.md
--rw-r--r--   0      501       20     1954 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/Contributing.md
--rw-r--r--   0      501       20     1069 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/LICENSE
--rw-r--r--   0      501       20     8040 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/README.md
--rw-r--r--   0      501       20       14 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/cbindgen.toml
--rw-r--r--   0      501       20      623 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/conftest.py
--rw-r--r--   0      501       20      638 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/Makefile
--rw-r--r--   0      501       20      804 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/make.bat
--rw-r--r--   0      501       20       16 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/requirements.txt
--rw-r--r--   0      501       20      155 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/source/arrow_odbc.rst
--rw-r--r--   0      501       20     1965 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/source/conf.py
--rw-r--r--   0      501       20      458 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/source/index.rst
--rw-r--r--   0      501       20       67 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/source/modules.rst
--rw-r--r--   0      501       20      348 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/docker-compose.yml
--rw-r--r--   0      501       20      564 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/manylinux/Dockerfile
--rw-r--r--   0      501       20      121 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/manylinux/Readme.md
--rw-r--r--   0      501       20      148 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/manylinux/WHEEL
--rw-r--r--   0      501       20     1256 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/manylinux/build_wheel.sh
--rw-r--r--   0      501       20      446 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/__init__.py
--rw-r--r--   0      501       20     1885 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/connect.py
--rw-r--r--   0      501       20      672 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/error.py
--rw-r--r--   0      501       20      788 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/log.py
--rw-r--r--   0      501       20      578 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/pool.py
--rw-r--r--   0      501       20    25240 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/reader.py
--rw-r--r--   0      501       20     9625 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/writer.py
--rw-r--r--   0      501       20     2322 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/error.rs
--rw-r--r--   0      501       20     3434 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/lib.rs
--rw-r--r--   0      501       20      655 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/logging.rs
--rw-r--r--   0      501       20     1239 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/parameter.rs
--rw-r--r--   0      501       20      421 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/pool.rs
--rw-r--r--   0      501       20     8757 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/reader/arrow_odbc_reader.rs
--rw-r--r--   0      501       20    12865 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/reader.rs
--rw-r--r--   0      501       20     3545 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/writer.rs
--rw-r--r--   0      501       20   274432 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/temp_db.duckdb
--rw-r--r--   0      501       20        0 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/tests/__init__.py
--rw-r--r--   0      501       20     4115 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/tests/iris.csv
--rw-r--r--   0      501       20     2413 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/tests/iris.parquet
--rw-r--r--   0      501       20    29032 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/tests/test_arrow_odbc.py
--rw-r--r--   0      501       20    42700 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/Cargo.lock
--rw-r--r--   0      501       20      825 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/pyproject.toml
--rw-r--r--   0        0        0     8652 1970-01-01 00:00:00.000000 arrow_odbc-7.0.1/PKG-INFO
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 arrow_odbc-7.0.2/Cargo.toml
+-rw-r--r--   0      501       20      136 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/.gitattributes
+-rw-r--r--   0      501       20      213 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/.github/dependabot.yml
+-rw-r--r--   0      501       20     1762 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/.github/workflows/test.yml
+-rw-r--r--   0      501       20     2657 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/.github/workflows/wheel.yml
+-rw-r--r--   0      501       20      286 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/.gitignore
+-rw-r--r--   0      501       20      841 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/.readthedocs.yaml
+-rw-r--r--   0      501       20    12116 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/Changelog.md
+-rw-r--r--   0      501       20     1954 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/Contributing.md
+-rw-r--r--   0      501       20     1069 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/LICENSE
+-rw-r--r--   0      501       20     8040 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/README.md
+-rw-r--r--   0      501       20       14 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/cbindgen.toml
+-rw-r--r--   0      501       20      623 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/conftest.py
+-rw-r--r--   0      501       20      638 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/doc/Makefile
+-rw-r--r--   0      501       20      804 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/doc/make.bat
+-rw-r--r--   0      501       20       16 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/doc/requirements.txt
+-rw-r--r--   0      501       20      155 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/doc/source/arrow_odbc.rst
+-rw-r--r--   0      501       20     1965 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/doc/source/conf.py
+-rw-r--r--   0      501       20      458 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/doc/source/index.rst
+-rw-r--r--   0      501       20       67 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/doc/source/modules.rst
+-rw-r--r--   0      501       20      348 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/docker-compose.yml
+-rw-r--r--   0      501       20      564 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/manylinux/Dockerfile
+-rw-r--r--   0      501       20      121 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/manylinux/Readme.md
+-rw-r--r--   0      501       20      148 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/manylinux/WHEEL
+-rw-r--r--   0      501       20     1256 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/manylinux/build_wheel.sh
+-rw-r--r--   0      501       20      446 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/python/arrow_odbc/__init__.py
+-rw-r--r--   0      501       20     1885 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/python/arrow_odbc/connect.py
+-rw-r--r--   0      501       20      672 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/python/arrow_odbc/error.py
+-rw-r--r--   0      501       20      788 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/python/arrow_odbc/log.py
+-rw-r--r--   0      501       20      578 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/python/arrow_odbc/pool.py
+-rw-r--r--   0      501       20    25240 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/python/arrow_odbc/reader.py
+-rw-r--r--   0      501       20     9625 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/python/arrow_odbc/writer.py
+-rw-r--r--   0      501       20     2322 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/src/error.rs
+-rw-r--r--   0      501       20     3434 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/src/lib.rs
+-rw-r--r--   0      501       20      655 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/src/logging.rs
+-rw-r--r--   0      501       20     1239 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/src/parameter.rs
+-rw-r--r--   0      501       20      421 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/src/pool.rs
+-rw-r--r--   0      501       20     8757 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/src/reader/arrow_odbc_reader.rs
+-rw-r--r--   0      501       20    12865 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/src/reader.rs
+-rw-r--r--   0      501       20     3545 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/src/writer.rs
+-rw-r--r--   0      501       20   274432 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/temp_db.duckdb
+-rw-r--r--   0      501       20        0 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/tests/__init__.py
+-rw-r--r--   0      501       20     4115 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/tests/iris.csv
+-rw-r--r--   0      501       20     2413 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/tests/iris.parquet
+-rw-r--r--   0      501       20    29032 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/tests/test_arrow_odbc.py
+-rw-r--r--   0      501       20    42700 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/Cargo.lock
+-rw-r--r--   0      501       20      825 2024-05-27 05:54:15.000000 arrow_odbc-7.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8652 1970-01-01 00:00:00.000000 arrow_odbc-7.0.2/PKG-INFO
```

### Comparing `arrow_odbc-7.0.1/Cargo.toml` & `arrow_odbc-7.0.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/.github/workflows/test.yml` & `arrow_odbc-7.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/.github/workflows/wheel.yml` & `arrow_odbc-7.0.2/.github/workflows/wheel.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,35 +12,31 @@
   push:
     # Sequence of patterns matched against refs/tags
     tags:
       - 'v*' # Push events to matching v*, i.e. v1.0, v20.15.10
 
 jobs:
   windows-wheel:
-
     runs-on: windows-latest
-
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Publish package
       run: |
         python -m pip install --upgrade pip
         python -m pip install build
         python -m build
         pip install twine
         twine upload --skip-existing -u __token__ -p "${{ secrets.PYPI_API_TOKEN }}" dist/*
-
-  osx_13_x86:
-
+        
+  macos-x86-wheel:
     runs-on: macos_x86_wheel
-
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Publish package
@@ -48,49 +44,43 @@
         python -m pip install --upgrade pip
         python -m pip install build
         python -m build
         pip install twine
         twine upload --skip-existing -u __token__ -p "${{ secrets.PYPI_API_TOKEN }}" dist/*
 
   manylinux-wheel:
-
     runs-on: ubuntu-latest
-
     steps:
     - uses: actions/checkout@v4
     - name: Build Manylinux wheel
       run: |
         docker build -t cargodock ./manylinux
         docker run --rm -v ${PWD}:/io cargodock bash /io/manylinux/build_wheel.sh
         pip install twine
         twine upload --skip-existing -u __token__ -p "${{ secrets.PYPI_API_TOKEN }}" dist/*
 
 
   macos-wheel-m1:
-
     runs-on: flyci-macos-14-m1
-
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install latests rust toolchain
       uses: actions-rs/toolchain@v1
       with:
         toolchain: stable
         default: true
         override: true
-
     - name: Install Unix ODBC
       run: |
         brew install unixodbc
         sudo ln -s /opt/homebrew/lib ~/lib
-
     - name: Publish package
       run: |
         python -m pip install --upgrade pip
         python -m pip install build
         python -m build
         pip install twine
         twine upload --skip-existing -u __token__ -p "${{ secrets.PYPI_API_TOKEN }}" dist/*
```

### Comparing `arrow_odbc-7.0.1/.readthedocs.yaml` & `arrow_odbc-7.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/Changelog.md` & `arrow_odbc-7.0.2/Changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Changelog
 
-## 7.0.1
+## 7.0.1-2
 
 - Build wheel for MacOS 13 x86
 
 ## 7.0.0
 
 - unsigned TinyInt is now mapped to `UInt8`.
```

### Comparing `arrow_odbc-7.0.1/Contributing.md` & `arrow_odbc-7.0.2/Contributing.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/LICENSE` & `arrow_odbc-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/README.md` & `arrow_odbc-7.0.2/README.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/conftest.py` & `arrow_odbc-7.0.2/conftest.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/doc/Makefile` & `arrow_odbc-7.0.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/doc/make.bat` & `arrow_odbc-7.0.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/doc/source/conf.py` & `arrow_odbc-7.0.2/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "arrow-odbc"
 copyright = "2021, Markus Klein"
 author = "Markus Klein"
 
 # The full version, including alpha/beta/rc tags
-release = "7.0.1"
+release = "7.0.2"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `arrow_odbc-7.0.1/manylinux/Dockerfile` & `arrow_odbc-7.0.2/manylinux/Dockerfile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/manylinux/build_wheel.sh` & `arrow_odbc-7.0.2/manylinux/build_wheel.sh`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/python/arrow_odbc/connect.py` & `arrow_odbc-7.0.2/python/arrow_odbc/connect.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/python/arrow_odbc/error.py` & `arrow_odbc-7.0.2/python/arrow_odbc/error.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/python/arrow_odbc/log.py` & `arrow_odbc-7.0.2/python/arrow_odbc/log.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/python/arrow_odbc/pool.py` & `arrow_odbc-7.0.2/python/arrow_odbc/pool.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/python/arrow_odbc/reader.py` & `arrow_odbc-7.0.2/python/arrow_odbc/reader.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/python/arrow_odbc/writer.py` & `arrow_odbc-7.0.2/python/arrow_odbc/writer.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/src/error.rs` & `arrow_odbc-7.0.2/src/error.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/src/lib.rs` & `arrow_odbc-7.0.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/src/logging.rs` & `arrow_odbc-7.0.2/src/logging.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/src/parameter.rs` & `arrow_odbc-7.0.2/src/parameter.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/src/reader/arrow_odbc_reader.rs` & `arrow_odbc-7.0.2/src/reader/arrow_odbc_reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/src/reader.rs` & `arrow_odbc-7.0.2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/src/writer.rs` & `arrow_odbc-7.0.2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/temp_db.duckdb` & `arrow_odbc-7.0.2/temp_db.duckdb`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/tests/iris.csv` & `arrow_odbc-7.0.2/tests/iris.csv`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/tests/iris.parquet` & `arrow_odbc-7.0.2/tests/iris.parquet`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/tests/test_arrow_odbc.py` & `arrow_odbc-7.0.2/tests/test_arrow_odbc.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/Cargo.lock` & `arrow_odbc-7.0.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.1/pyproject.toml` & `arrow_odbc-7.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "maturin"
 
 [project]
 name = "arrow-odbc"
 authors = [{name = "Markus Klein"}]
 description="Read the data of an ODBC data source as sequence of Apache Arrow record batches."
 readme = "README.md"
-version = "7.0.1"
+version = "7.0.2"
 dependencies = ["cffi", "pyarrow >= 8.0.0"]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = ["pytest < 8.0.0", "pyodbc", "duckdb"]
```

### Comparing `arrow_odbc-7.0.1/PKG-INFO` & `arrow_odbc-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arrow-odbc
-Version: 7.0.1
+Version: 7.0.2
 Requires-Dist: cffi
 Requires-Dist: pyarrow >=8.0.0
 Requires-Dist: pytest <8.0.0 ; extra == 'test'
 Requires-Dist: pyodbc ; extra == 'test'
 Requires-Dist: duckdb ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
```

