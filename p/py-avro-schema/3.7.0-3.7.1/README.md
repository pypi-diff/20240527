# Comparing `tmp/py_avro_schema-3.7.0.tar.gz` & `tmp/py_avro_schema-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_avro_schema-3.7.0.tar", last modified: Thu May 23 12:00:48 2024, max compression
+gzip compressed data, was "py_avro_schema-3.7.1.tar", last modified: Mon May 27 13:33:09 2024, max compression
```

## Comparing `py_avro_schema-3.7.0.tar` & `py_avro_schema-3.7.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.128196 py_avro_schema-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.120196 py_avro_schema-3.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.120196 py_avro_schema-3.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15052 2024-05-23 12:00:48.128196 py_avro_schema-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.124196 py_avro_schema-3.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/docs/py_avro_schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 12:00:48.128196 py_avro_schema-3.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.120196 py_avro_schema-3.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.124196 py_avro_schema-3.7.0/src/py_avro_schema/
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/src/py_avro_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/src/py_avro_schema/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/src/py_avro_schema/_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/src/py_avro_schema/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/src/py_avro_schema/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.124196 py_avro_schema-3.7.0/src/py_avro_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15052 2024-05-23 12:00:48.000000 py_avro_schema-3.7.0/src/py_avro_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-23 12:00:48.000000 py_avro_schema-3.7.0/src/py_avro_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:00:48.000000 py_avro_schema-3.7.0/src/py_avro_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-23 12:00:48.000000 py_avro_schema-3.7.0/src/py_avro_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 12:00:48.000000 py_avro_schema-3.7.0/src/py_avro_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.124196 py_avro_schema-3.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_avro_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    21362 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_logicals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_plain_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    16924 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:09.227857 py_avro_schema-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:09.215857 py_avro_schema-3.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:09.219857 py_avro_schema-3.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15052 2024-05-27 13:33:09.223857 py_avro_schema-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:09.219857 py_avro_schema-3.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/docs/py_avro_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:33:09.227857 py_avro_schema-3.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:09.215857 py_avro_schema-3.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:09.219857 py_avro_schema-3.7.1/src/py_avro_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/src/py_avro_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/src/py_avro_schema/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/src/py_avro_schema/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/src/py_avro_schema/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/src/py_avro_schema/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:09.223857 py_avro_schema-3.7.1/src/py_avro_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15052 2024-05-27 13:33:09.000000 py_avro_schema-3.7.1/src/py_avro_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-27 13:33:09.000000 py_avro_schema-3.7.1/src/py_avro_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:33:09.000000 py_avro_schema-3.7.1/src/py_avro_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 13:33:09.000000 py_avro_schema-3.7.1/src/py_avro_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 13:33:09.000000 py_avro_schema-3.7.1/src/py_avro_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:09.223857 py_avro_schema-3.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/tests/test_avro_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21362 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/tests/test_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/tests/test_logicals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/tests/test_plain_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16924 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-27 13:33:03.000000 py_avro_schema-3.7.1/tox.ini
```

### Comparing `py_avro_schema-3.7.0/.flake8` & `py_avro_schema-3.7.1/.flake8`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/.github/workflows/release-package.yml` & `py_avro_schema-3.7.1/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/.github/workflows/test-package.yml` & `py_avro_schema-3.7.1/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/.gitignore` & `py_avro_schema-3.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/.pre-commit-config.yaml` & `py_avro_schema-3.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/LICENSE` & `py_avro_schema-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/LICENSE_HEADER.txt` & `py_avro_schema-3.7.1/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/PKG-INFO` & `py_avro_schema-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-avro-schema
-Version: 3.7.0
+Version: 3.7.1
 Summary: Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py_avro_schema-3.7.0/README.md` & `py_avro_schema-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/docs/conf.py` & `py_avro_schema-3.7.1/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "sphinx_rtd_theme",
 ]
 
 html_theme = "sphinx_rtd_theme"
 
+add_module_names = False
+
 autosectionlabel_prefix_document = True
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
 }
 
 # List of patterns, relative to source directory, that match files and
```

### Comparing `py_avro_schema-3.7.0/docs/index.rst` & `py_avro_schema-3.7.1/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 py-avro-schema
 ==============
 
 Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 
 .. toctree::
-   :maxdepth: 2
+   :maxdepth: 1
    :caption: Contents
 
    tutorial
    types
    modules
```

### Comparing `py_avro_schema-3.7.0/docs/tutorial.rst` & `py_avro_schema-3.7.1/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/docs/types.rst` & `py_avro_schema-3.7.1/docs/types.rst`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/pyproject.toml` & `py_avro_schema-3.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/src/py_avro_schema/__init__.py` & `py_avro_schema-3.7.1/src/py_avro_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/src/py_avro_schema/_schemas.py` & `py_avro_schema-3.7.1/src/py_avro_schema/_schemas.py`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/src/py_avro_schema/_testing.py` & `py_avro_schema-3.7.1/src/py_avro_schema/_testing.py`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/src/py_avro_schema/_typing.py` & `py_avro_schema-3.7.1/src/py_avro_schema/_typing.py`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/src/py_avro_schema.egg-info/PKG-INFO` & `py_avro_schema-3.7.1/src/py_avro_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-avro-schema
-Version: 3.7.0
+Version: 3.7.1
 Summary: Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py_avro_schema-3.7.0/src/py_avro_schema.egg-info/SOURCES.txt` & `py_avro_schema-3.7.1/src/py_avro_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/tests/test_avro_schema.py` & `py_avro_schema-3.7.1/tests/test_avro_schema.py`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/tests/test_dataclass.py` & `py_avro_schema-3.7.1/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/tests/test_logicals.py` & `py_avro_schema-3.7.1/tests/test_logicals.py`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/tests/test_plain_class.py` & `py_avro_schema-3.7.1/tests/test_plain_class.py`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/tests/test_primitives.py` & `py_avro_schema-3.7.1/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/tests/test_pydantic.py` & `py_avro_schema-3.7.1/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/tests/test_typing.py` & `py_avro_schema-3.7.1/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `py_avro_schema-3.7.0/tox.ini` & `py_avro_schema-3.7.1/tox.ini`

 * *Files identical despite different names*

