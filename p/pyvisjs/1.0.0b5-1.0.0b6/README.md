# Comparing `tmp/pyvisjs-1.0.0b5.tar.gz` & `tmp/pyvisjs-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisjs-1.0.0b5.tar", last modified: Thu May 23 17:56:09 2024, max compression
+gzip compressed data, was "pyvisjs-1.0.0b6.tar", last modified: Mon May 27 12:16:40 2024, max compression
```

## Comparing `pyvisjs-1.0.0b5.tar` & `pyvisjs-1.0.0b6.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.179188 pyvisjs-1.0.0b5/
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1975 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     5120 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4040 2024-05-23 17:56:09.178188 pyvisjs-1.0.0b5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.169187 pyvisjs-1.0.0b5/docs/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/basic-example.md
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/edges.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.170187 pyvisjs-1.0.0b5/docs/img/
--rw-rw-rw-   0 root         (0) root         (0)      910 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/img/favicon-32x32.png
--rw-rw-rw-   0 root         (0) root         (0)    15406 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/img/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/index.md
--rw-rw-rw-   0 root         (0) root         (0)      419 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/installation.md
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/network.md
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/nodes.md
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/options.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.170187 pyvisjs-1.0.0b5/docs_overrides/
--rw-rw-rw-   0 root         (0) root         (0)     5058 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs_overrides/dandelion.html
--rw-rw-rw-   0 root         (0) root         (0)    32009 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs_overrides/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.171187 pyvisjs-1.0.0b5/examples/
--rw-rw-rw-   0 root         (0) root         (0)      718 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/examples/basic-example.py
--rw-rw-rw-   0 root         (0) root         (0)     2665 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/examples/repo.py
--rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/folder_structure.txt
--rw-rw-rw-   0 root         (0) root         (0)     1466 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/mkdocs.yml
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.173187 pyvisjs-1.0.0b5/pyvisjs/
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2146 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/edge.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/network.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/node.py
--rw-rw-rw-   0 root         (0) root         (0)    13511 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.176187 pyvisjs-1.0.0b5/pyvisjs/templates/
--rw-rw-rw-   0 root         (0) root         (0)      966 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/basic.html
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/bs-container.html
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/create_network.js
--rw-rw-rw-   0 root         (0) root         (0)      926 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/draw_title.js
--rw-rw-rw-   0 root         (0) root         (0)     7777 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/functions.js
--rw-rw-rw-   0 root         (0) root         (0)      605 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/init_tomSelect.js
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/select-edge-filter.html
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/tom-select.html
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.178188 pyvisjs-1.0.0b5/pyvisjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4040 2024-05-23 17:56:09.000000 pyvisjs-1.0.0b5/pyvisjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1166 2024-05-23 17:56:09.000000 pyvisjs-1.0.0b5/pyvisjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 17:56:09.000000 pyvisjs-1.0.0b5/pyvisjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-23 17:56:09.000000 pyvisjs-1.0.0b5/pyvisjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-23 17:56:09.000000 pyvisjs-1.0.0b5/pyvisjs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 17:56:09.179188 pyvisjs-1.0.0b5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.177188 pyvisjs-1.0.0b5/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/test_base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/test_edge.py
--rw-rw-rw-   0 root         (0) root         (0)    12201 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/test_network.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/test_options.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 12:16:40.641105 pyvisjs-1.0.0b6/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5120 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4032 2024-05-27 12:16:40.641105 pyvisjs-1.0.0b6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 12:16:40.632105 pyvisjs-1.0.0b6/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     5236 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs/basic-example.md
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs/edges.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 12:16:40.632105 pyvisjs-1.0.0b6/docs/img/
+-rw-rw-rw-   0 root         (0) root         (0)      910 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs/img/favicon-32x32.png
+-rw-rw-rw-   0 root         (0) root         (0)    15406 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs/img/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     4136 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs/index.md
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs/installation.md
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs/network.md
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs/nodes.md
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs/options.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 12:16:40.634105 pyvisjs-1.0.0b6/docs_overrides/
+-rw-rw-rw-   0 root         (0) root         (0)     5058 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs_overrides/dandelion.html
+-rw-rw-rw-   0 root         (0) root         (0)    32505 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/docs_overrides/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 12:16:40.634105 pyvisjs-1.0.0b6/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      718 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/examples/basic-example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2572 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/examples/repo.py
+-rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/folder_structure.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 12:16:40.635105 pyvisjs-1.0.0b6/pyvisjs/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2146 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     9743 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/network.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/node.py
+-rw-rw-rw-   0 root         (0) root         (0)    16256 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 12:16:40.638105 pyvisjs-1.0.0b6/pyvisjs/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/templates/basic.html
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/templates/bs-container.html
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/templates/create_network.js
+-rw-rw-rw-   0 root         (0) root         (0)      926 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/templates/draw_title.js
+-rw-rw-rw-   0 root         (0) root         (0)     7777 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/templates/functions.js
+-rw-rw-rw-   0 root         (0) root         (0)      605 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/templates/init_tomSelect.js
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/templates/select-edge-filter.html
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/templates/tom-select.html
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/pyvisjs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 12:16:40.640105 pyvisjs-1.0.0b6/pyvisjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4032 2024-05-27 12:16:40.000000 pyvisjs-1.0.0b6/pyvisjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-27 12:16:40.000000 pyvisjs-1.0.0b6/pyvisjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 12:16:40.000000 pyvisjs-1.0.0b6/pyvisjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-27 12:16:40.000000 pyvisjs-1.0.0b6/pyvisjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-27 12:16:40.000000 pyvisjs-1.0.0b6/pyvisjs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 12:16:40.641105 pyvisjs-1.0.0b6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 12:16:40.640105 pyvisjs-1.0.0b6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 12:16:24.000000 pyvisjs-1.0.0b6/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/tests/test_base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/tests/test_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)    15759 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/tests/test_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/tests/test_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-27 12:16:23.000000 pyvisjs-1.0.0b6/tests/test_utils.py
```

### Comparing `pyvisjs-1.0.0b5/.gitignore` & `pyvisjs-1.0.0b6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/.gitlab-ci.yml` & `pyvisjs-1.0.0b6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/CONTRIBUTING.md` & `pyvisjs-1.0.0b6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/LICENSE` & `pyvisjs-1.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/PKG-INFO` & `pyvisjs-1.0.0b6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,21 +36,20 @@
 Requires-Dist: Jinja2
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: all
 Requires-Dist: pyvisjs[test]; extra == "all"
 
 [![pipeline status](https://gitlab.com/22kittens/pyvisjs/badges/main/pipeline.svg)](https://gitlab.com/22kittens/pyvisjs/-/commits/main)
-[![Latest Release](https://gitlab.com/22kittens/pyvisjs/-/badges/release.svg)](https://gitlab.com/22kittens/pyvisjs/-/releases)
 [![PyPI - Version](https://img.shields.io/pypi/v/pyvisjs)](https://pypi.org/project/pyvisjs)
 [![Documentation](https://img.shields.io/badge/ref-Documentation-blue)](https://22kittens.gitlab.io/pyvisjs/)
 
 
 
-# ![logo](docs/img/favicon-32x32.png) - pyvisjs
+# ![logo](https://gitlab.com/uploads/-/system/project/avatar/56819743/favicon-32x32.png) - pyvisjs
 Python wrapper for vis.js Network
 
 > :warning: **Beta version disclaimer** Please note that this package is in a **beta** version and backwards-incompatible changes might be introduced in future releases.
 
 
 pyvisjs is a Python package designed to provide seamless interaction with [vis.js](https://visjs.org) network visualizations, allowing users to manipulate and visualize network data using Python.
 
@@ -87,16 +86,16 @@
 net.show("example.html")
 ```
 
 For more examples and detailed usage, please refer to the [documentation](https://22kittens.gitlab.io/pyvisjs).
 
 ## Contributing
 
-Contributions are welcome! If you have suggestions, feature requests, or find any bugs, please open an issue or submit a pull request. Make sure to follow the [contribution guidelines](CONTRIBUTING.md).
+Contributions are welcome! If you have suggestions, feature requests, or find any bugs, please open an issue or submit a pull request. Make sure to follow the [contribution guidelines](https://22kittens.gitlab.io/pyvisjs/CONTRIBUTING).
 
 ## Acknowledgments
 
 This project is inspired by the [pyvis](https://github.com/WestHealth/pyvis) Python package and the [visNetwork](https://github.com/datastorm-open/visNetwork) R-language package.
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](https://22kittens.gitlab.io/pyvisjs/LICENSE).
```

### Comparing `pyvisjs-1.0.0b5/README.md` & `pyvisjs-1.0.0b6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [![pipeline status](https://gitlab.com/22kittens/pyvisjs/badges/main/pipeline.svg)](https://gitlab.com/22kittens/pyvisjs/-/commits/main)
-[![Latest Release](https://gitlab.com/22kittens/pyvisjs/-/badges/release.svg)](https://gitlab.com/22kittens/pyvisjs/-/releases)
 [![PyPI - Version](https://img.shields.io/pypi/v/pyvisjs)](https://pypi.org/project/pyvisjs)
 [![Documentation](https://img.shields.io/badge/ref-Documentation-blue)](https://22kittens.gitlab.io/pyvisjs/)
 
 
 
-# ![logo](docs/img/favicon-32x32.png) - pyvisjs
+# ![logo](https://gitlab.com/uploads/-/system/project/avatar/56819743/favicon-32x32.png) - pyvisjs
 Python wrapper for vis.js Network
 
 > :warning: **Beta version disclaimer** Please note that this package is in a **beta** version and backwards-incompatible changes might be introduced in future releases.
 
 
 pyvisjs is a Python package designed to provide seamless interaction with [vis.js](https://visjs.org) network visualizations, allowing users to manipulate and visualize network data using Python.
 
@@ -46,16 +45,16 @@
 net.show("example.html")
 ```
 
 For more examples and detailed usage, please refer to the [documentation](https://22kittens.gitlab.io/pyvisjs).
 
 ## Contributing
 
-Contributions are welcome! If you have suggestions, feature requests, or find any bugs, please open an issue or submit a pull request. Make sure to follow the [contribution guidelines](CONTRIBUTING.md).
+Contributions are welcome! If you have suggestions, feature requests, or find any bugs, please open an issue or submit a pull request. Make sure to follow the [contribution guidelines](https://22kittens.gitlab.io/pyvisjs/CONTRIBUTING).
 
 ## Acknowledgments
 
 This project is inspired by the [pyvis](https://github.com/WestHealth/pyvis) Python package and the [visNetwork](https://github.com/datastorm-open/visNetwork) R-language package.
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](https://22kittens.gitlab.io/pyvisjs/LICENSE).
```

### Comparing `pyvisjs-1.0.0b5/docs/img/favicon-32x32.png` & `pyvisjs-1.0.0b6/docs/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/docs/img/favicon.ico` & `pyvisjs-1.0.0b6/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/docs_overrides/dandelion.html` & `pyvisjs-1.0.0b6/docs_overrides/dandelion.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/docs_overrides/index.html` & `pyvisjs-1.0.0b6/docs_overrides/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
 </div>
 
 <script type="text/javascript">
     
     
 const data = create_network();
 data.network.has_hidden_nodes = false;
+data.network.zoom_animation_played = false;
 
 // sorry for this dirty trick
 el2m3nt = document.getElementById("__palette_1");
 el2m3nt.parentNode.removeChild(el2m3nt);
 
 el2m3nt = document.getElementsByClassName("vis-button vis-up")[0];
 el2m3nt.parentNode.removeChild(el2m3nt);
@@ -155,20 +156,35 @@
 el2m3nt.parentNode.removeChild(el2m3nt);
 el2m3nt = document.getElementsByClassName("vis-button vis-right")[0];
 el2m3nt.parentNode.removeChild(el2m3nt);
 el2m3nt = document.getElementsByClassName("vis-button vis-zoomExtends")[0];
 el2m3nt.parentNode.removeChild(el2m3nt);
 
 
-//data.network.redraw();
+data.network.once("afterDrawing", 
+    function (ctx) {
+        if (data.network.zoom_animation_played === false) {
+            data.network.Zoom(1.55, 3000)
+            data.network.zoom_animation_played = true
+        }
+    }
+);
 
 
 // all jinja injections should happen here because it allows to mock this function and test all the rest in isolation
 function create_network() {
 
+    vis.Network.prototype.Zoom = function (scale, duration) {
+        const animationOptions = {
+            scale: this.getScale() + scale,
+            animation: { duration: duration }
+        };
+        this.view.moveTo(animationOptions);
+    };
+    
     // create an array with nodes
     const ds_nodes = new vis.DataSet([{"color": "orange", "file_ext": "", "file_type": "dir", "font": {"color": "black"}, "id": ".", "label": "pyvisjs\nadd\npackage\ndocumentation", "shape": "circle"}, {"color": "#4eba3f", "file_ext": "", "file_type": "dir", "font": {"color": "black"}, "id": ".\\docs", "label": "docs", "shape": "circle"}, {"color": "#4eba3f", "file_ext": "", "file_type": "dir", "font": {"color": "black"}, "id": ".\\docs_overrides", "label": "docs_overrides", "shape": "circle"}, {"color": "#4eba3f", "file_ext": "", "file_type": "dir", "font": {"color": "black"}, "id": ".\\examples", "label": "examples", "shape": "circle"}, {"color": "#4eba3f", "file_ext": "", "file_type": "dir", "font": {"color": "black"}, "id": ".\\pyvisjs", "label": "pyvisjs", "shape": "circle"}, {"color": "#4eba3f", "file_ext": "", "file_type": "dir", "font": {"color": "black"}, "id": ".\\tests", "label": "tests", "shape": "circle"}, {"file_ext": "", "file_type": "file", "font": {"color": "black"}, "id": ".\\.gitignore", "label": ".gitignore", "shape": "box"}, {"file_ext": ".yml", "file_type": "file", "font": {"color": "black"}, "id": ".\\.gitlab-ci.yml", "label": ".gitlab-ci.yml", "shape": "box"}, {"color": "#F02B4B", "file_ext": ".md", "file_type": "file", "font": {"color": "black"}, "id": ".\\CONTRIBUTING.md", "label": "CONTRIBUTING.md", "shape": "box"}, {"color": "#8f2d56", "file_ext": ".html", "file_type": "file", "font": {"color": "white"}, "id": ".\\default.html", "label": "default.html", "shape": "box"}, {"color": "#DF7DEC", "file_ext": ".txt", "file_type": "file", "font": {"color": "black"}, "id": ".\\folder_structure.txt", "label": "folder_structure.txt", "shape": "box"}, {"file_ext": "", "file_type": "file", "font": {"color": "black"}, "id": ".\\LICENSE", "label": "LICENSE", "shape": "box"}, {"file_ext": ".yml", "file_type": "file", "font": {"color": "black"}, "id": ".\\mkdocs.yml", "label": "mkdocs.yml", "shape": "box"}, {"file_ext": ".toml", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyproject.toml", "label": "pyproject.toml", "shape": "box"}, {"color": "#F02B4B", "file_ext": ".md", "file_type": "file", "font": {"color": "black"}, "id": ".\\README.md", "label": "README.md", "shape": "box"}, {"color": "#DF7DEC", "file_ext": ".txt", "file_type": "file", "font": {"color": "black"}, "id": ".\\requirements-doc.txt", "label": "requirements-doc.txt", "shape": "box"}, {"color": "#DF7DEC", "file_ext": ".txt", "file_type": "file", "font": {"color": "black"}, "id": ".\\requirements.txt", "label": "requirements.txt", "shape": "box"}, {"color": "#4eba3f", "file_ext": "", "file_type": "dir", "font": {"color": "black"}, "id": ".\\docs\\img", "label": "img", "shape": "circle"}, {"color": "#F02B4B", "file_ext": ".md", "file_type": "file", "font": {"color": "black"}, "id": ".\\docs\\edges.md", "label": "edges.md", "shape": "box"}, {"color": "#F02B4B", "file_ext": ".md", "file_type": "file", "font": {"color": "black"}, "id": ".\\docs\\examples.md", "label": "examples.md", "shape": "box"}, {"color": "#F02B4B", "file_ext": ".md", "file_type": "file", "font": {"color": "black"}, "id": ".\\docs\\index.md", "label": "index.md", "shape": "box"}, {"file_ext": ".png", "file_type": "file", "font": {"color": "black"}, "id": ".\\docs\\img\\favicon-32x32.png", "label": "favicon-32x32.png", "shape": "box"}, {"file_ext": ".ico", "file_type": "file", "font": {"color": "black"}, "id": ".\\docs\\img\\favicon.ico", "label": "favicon.ico", "shape": "box"}, {"color": "#8f2d56", "file_ext": ".html", "file_type": "file", "font": {"color": "white"}, "id": ".\\docs_overrides\\home.html", "label": "home.html", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\examples\\bluor.py", "label": "bluor.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\examples\\readme.py", "label": "readme.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\examples\\repo.py", "label": "repo.py", "shape": "box"}, {"color": "#4eba3f", "file_ext": "", "file_type": "dir", "font": {"color": "black"}, "id": ".\\pyvisjs\\templates", "label": "templates", "shape": "circle"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyvisjs\\base_dictable.py", "label": "base_dictable.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyvisjs\\edge.py", "label": "edge.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyvisjs\\network.py", "label": "network.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyvisjs\\node.py", "label": "node.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyvisjs\\options.py", "label": "options.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyvisjs\\utils.py", "label": "utils.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyvisjs\\_version.py", "label": "_version.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyvisjs\\__init__.py", "label": "__init__.py", "shape": "box"}, {"color": "#8f2d56", "file_ext": ".html", "file_type": "file", "font": {"color": "white"}, "id": ".\\pyvisjs\\templates\\base.html", "label": "base.html", "shape": "box"}, {"color": "#8f2d56", "file_ext": ".html", "file_type": "file", "font": {"color": "white"}, "id": ".\\pyvisjs\\templates\\basic.html", "label": "basic.html", "shape": "box"}, {"color": "#8f2d56", "file_ext": ".html", "file_type": "file", "font": {"color": "white"}, "id": ".\\pyvisjs\\templates\\bs-container.html", "label": "bs-container.html", "shape": "box"}, {"color": "#da7422", "file_ext": ".js", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyvisjs\\templates\\create_network.js", "label": "create_network.js", "shape": "box"}, {"color": "#da7422", "file_ext": ".js", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyvisjs\\templates\\draw_title.js", "label": "draw_title.js", "shape": "box"}, {"color": "#da7422", "file_ext": ".js", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyvisjs\\templates\\functions.js", "label": "functions.js", "shape": "box"}, {"color": "#da7422", "file_ext": ".js", "file_type": "file", "font": {"color": "black"}, "id": ".\\pyvisjs\\templates\\init_tomSelect.js", "label": "init_tomSelect.js", "shape": "box"}, {"color": "#8f2d56", "file_ext": ".html", "file_type": "file", "font": {"color": "white"}, "id": ".\\pyvisjs\\templates\\select-edge-filter.html", "label": "select-edge-filter.html", "shape": "box"}, {"color": "#8f2d56", "file_ext": ".html", "file_type": "file", "font": {"color": "white"}, "id": ".\\pyvisjs\\templates\\tom-select.html", "label": "tom-select.html", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\tests\\test_base_dictable.py", "label": "test_base_dictable.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\tests\\test_edge.py", "label": "test_edge.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\tests\\test_network.py", "label": "test_network.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\tests\\test_node.py", "label": "test_node.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\tests\\test_options.py", "label": "test_options.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\tests\\test_utils.py", "label": "test_utils.py", "shape": "box"}, {"color": "#54bede", "file_ext": ".py", "file_type": "file", "font": {"color": "black"}, "id": ".\\tests\\__init__.py", "label": "__init__.py", "shape": "box"}]);
 
     // create an array with edges
     const ds_edges = new vis.DataSet([{"from": ".", "label": "dir:1", "to": ".\\docs"}, {"from": ".", "label": "dir:2", "to": ".\\docs_overrides"}, {"from": ".", "label": "dir:3", "to": ".\\examples"}, {"from": ".", "label": "dir:4", "to": ".\\pyvisjs"}, {"from": ".", "label": "dir:6", "to": ".\\tests"}, {"from": ".", "label": "file:0", "to": ".\\.gitignore"}, {"from": ".", "label": "file:1", "to": ".\\.gitlab-ci.yml"}, {"from": ".", "label": "file:2", "to": ".\\CONTRIBUTING.md"}, {"from": ".", "label": "file:3", "to": ".\\default.html"}, {"from": ".", "label": "file:4", "to": ".\\folder_structure.txt"}, {"from": ".", "label": "file:5", "to": ".\\LICENSE"}, {"from": ".", "label": "file:6", "to": ".\\mkdocs.yml"}, {"from": ".", "label": "file:7", "to": ".\\pyproject.toml"}, {"from": ".", "label": "file:8", "to": ".\\README.md"}, {"from": ".", "label": "file:9", "to": ".\\requirements-doc.txt"}, {"from": ".", "label": "file:10", "to": ".\\requirements.txt"}, {"from": ".\\docs", "label": "dir:0", "to": ".\\docs\\img"}, {"from": ".\\docs", "label": "file:0", "to": ".\\docs\\edges.md"}, {"from": ".\\docs", "label": "file:1", "to": ".\\docs\\examples.md"}, {"from": ".\\docs", "label": "file:2", "to": ".\\docs\\index.md"}, {"from": ".\\docs\\img", "label": "file:0", "to": ".\\docs\\img\\favicon-32x32.png"}, {"from": ".\\docs\\img", "label": "file:1", "to": ".\\docs\\img\\favicon.ico"}, {"from": ".\\docs_overrides", "label": "file:0", "to": ".\\docs_overrides\\home.html"}, {"from": ".\\examples", "label": "file:0", "to": ".\\examples\\bluor.py"}, {"from": ".\\examples", "label": "file:1", "to": ".\\examples\\readme.py"}, {"from": ".\\examples", "label": "file:2", "to": ".\\examples\\repo.py"}, {"from": ".\\pyvisjs", "label": "dir:0", "to": ".\\pyvisjs\\templates"}, {"from": ".\\pyvisjs", "label": "file:0", "to": ".\\pyvisjs\\base_dictable.py"}, {"from": ".\\pyvisjs", "label": "file:1", "to": ".\\pyvisjs\\edge.py"}, {"from": ".\\pyvisjs", "label": "file:2", "to": ".\\pyvisjs\\network.py"}, {"from": ".\\pyvisjs", "label": "file:3", "to": ".\\pyvisjs\\node.py"}, {"from": ".\\pyvisjs", "label": "file:4", "to": ".\\pyvisjs\\options.py"}, {"from": ".\\pyvisjs", "label": "file:5", "to": ".\\pyvisjs\\utils.py"}, {"from": ".\\pyvisjs", "label": "file:6", "to": ".\\pyvisjs\\_version.py"}, {"from": ".\\pyvisjs", "label": "file:7", "to": ".\\pyvisjs\\__init__.py"}, {"from": ".\\pyvisjs\\templates", "label": "file:0", "to": ".\\pyvisjs\\templates\\base.html"}, {"from": ".\\pyvisjs\\templates", "label": "file:1", "to": ".\\pyvisjs\\templates\\basic.html"}, {"from": ".\\pyvisjs\\templates", "label": "file:2", "to": ".\\pyvisjs\\templates\\bs-container.html"}, {"from": ".\\pyvisjs\\templates", "label": "file:3", "to": ".\\pyvisjs\\templates\\create_network.js"}, {"from": ".\\pyvisjs\\templates", "label": "file:4", "to": ".\\pyvisjs\\templates\\draw_title.js"}, {"from": ".\\pyvisjs\\templates", "label": "file:5", "to": ".\\pyvisjs\\templates\\functions.js"}, {"from": ".\\pyvisjs\\templates", "label": "file:6", "to": ".\\pyvisjs\\templates\\init_tomSelect.js"}, {"from": ".\\pyvisjs\\templates", "label": "file:7", "to": ".\\pyvisjs\\templates\\select-edge-filter.html"}, {"from": ".\\pyvisjs\\templates", "label": "file:8", "to": ".\\pyvisjs\\templates\\tom-select.html"}, {"from": ".\\tests", "label": "file:0", "to": ".\\tests\\test_base_dictable.py"}, {"from": ".\\tests", "label": "file:1", "to": ".\\tests\\test_edge.py"}, {"from": ".\\tests", "label": "file:2", "to": ".\\tests\\test_network.py"}, {"from": ".\\tests", "label": "file:3", "to": ".\\tests\\test_node.py"}, {"from": ".\\tests", "label": "file:4", "to": ".\\tests\\test_options.py"}, {"from": ".\\tests", "label": "file:5", "to": ".\\tests\\test_utils.py"}, {"from": ".\\tests", "label": "file:6", "to": ".\\tests\\__init__.py"}]);
 
     // create a network
@@ -197,25 +213,24 @@
             "file_type": ["dir", "file"],
             "label": [".gitignore", ".gitlab-ci.yml", ".pytest_cache", "CACHEDIR.TAG", "CONTRIBUTING.md", "LICENSE", "README.md", "__init__.py", "_version.py", "base.html", "base_dictable.py", "basic.html", "bluor.py", "bs-container.html", "cache", "create_network.js", "default.html", "docs", "docs_overrides", "draw_title.js", "edge.py", "edges.md", "examples", "examples.md", "favicon-32x32.png", "favicon.ico", "folder_structure.txt", "functions.js", "home copy.html", "home.html", "img", "index.md", "init_tomSelect.js", "mkdocs.yml", "network.py", "node.py", "nodeids", "options.py", "pyproject.toml", "pyvisjs", "pyvisjs\nadd\npackage\ndocumentation", "readme.py", "repo.py", "requirements-doc.txt", "requirements.txt", "select-edge-filter.html", "stepwise", "templates", "test_base_dictable.py", "test_edge.py", "test_network.py", "test_node.py", "test_options.py", "test_utils.py", "tests", "tom-select.html", "utils.py", "v"]
         }, 
         "title": "pyvisjs code repo visualisation",
         "dropdown_auto_close": true,
     };
 
-
     return {
         network: new vis.Network(container, data, options),
         nodes: ds_nodes.get({ returnType: "Object" }),
         edges: ds_edges.get({ returnType: "Object" }),
         ds_nodes: ds_nodes,
         pyvisjs: pyvisjs,
     }
 }
     
-    const eventHandler = function(name) {
+const eventHandler = function(name) {
     return function() {
         const list_of_selected_values = arguments[0];
         dict = convert_field_value_list_to_dict(list_of_selected_values);
         hide_nodes_by_edge_attribute_values_intersect(dict);
         if (data.pyvisjs.dropdown_auto_close === true) tom_select.close();
     };
 };
@@ -226,15 +241,16 @@
     //create: true,
     //onItemAdd:function(){
     //    this.setTextboxValue('');
     //    this.refreshOptions();
     //},
     plugins: ['remove_button'],
 });
-    if (data.pyvisjs.title !== null) {
+
+if (data.pyvisjs.title !== null) {
     data.network.on("beforeDrawing", function (ctx) {
         const central_focus = data.network.getViewPosition();
         const scale = data.network.getScale();
 
         div = document.getElementById("visjsnet").getElementsByClassName("vis-network")[0];
         const height = div.clientHeight;
         const width = div.clientWidth;
```

### Comparing `pyvisjs-1.0.0b5/examples/basic-example.py` & `pyvisjs-1.0.0b6/examples/basic-example.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/examples/repo.py` & `pyvisjs-1.0.0b6/examples/repo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 from pyvisjs import Network, Options
 import os
 from pathlib import Path
 
 
 options = Options("800px", "1300px")
 options.edges.set(arrows="to")
+options.pyvisjs \
+    .set(title="pyvisjs code repo visualisation") \
+    .set_filtering(
+        enable_highlighting=True,
+        node_filtering=["file_type", "file_ext", "label"],
+        dropdown_auto_close=True,
+    )
 
 net = Network(options=options)
 
 for path, subdirs, files in os.walk("."):
     if ".venv" not in path \
         and "__pycache__" not in path \
         and "cachedir.tag" not in path \
+        and ".pytest_cache" not in path \
+        and ".git" not in path \
+        and "node_modules" not in path \
         and "egg-info" not in path:
         curr_dir = (Path(os.getcwd()).stem).replace("-", "\n")
         net.add_node(
             node_id = path, 
             label = curr_dir, 
             shape = "circle",
             color = "orange",
             font = {"color": "black"},
             file_type = "dir",
             file_ext = "",
         )
 
         for name in subdirs:
-            if name not in [".venv", "__pycache__", "pyvisjs.egg-info", "cachedir.tag"]:
-                full_name = os.path.join(path, name)
-                net.add_node(
-                    node_id = full_name, 
-                    label = name, 
-                    shape = "circle",
-                    color = "#4eba3f",
-                    font = {"color": "black"},
-                    file_type = "dir",
-                    file_ext = "",
-                )            
-                net.add_edge(path, full_name, label=f"dir:{subdirs.index(name)}")
+            full_name = os.path.join(path, name)
+            net.add_node(
+                node_id = full_name, 
+                label = name, 
+                shape = "circle",
+                color = "#4eba3f",
+                font = {"color": "black"},
+                file_type = "dir",
+                file_ext = "",
+            )            
+            net.add_edge(path, full_name, label=f"dir:{subdirs.index(name)}")
 
         for name in files:
             full_name = os.path.join(path, name)
             ext = Path(name).suffix
 
             if ext == ".py":
                 (color, font_color) = ("#54bede", "black")
@@ -63,14 +72,8 @@
                 file_type = "file",
                 file_ext = ext,
                 font = {"color": font_color},
             )            
             net.add_edge(path, full_name, label=f"file:{files.index(name)}")
 
 
-net.render_tom_template(
-                    title="pyvisjs code repo visualisation",
-                    open_in_browser=True,
-                    enable_highlighting=True,
-                    node_filtering=["file_type", "file_ext", "label"],
-                    dropdown_auto_close=True,
-                    )
+net.show()
```

### Comparing `pyvisjs-1.0.0b5/folder_structure.txt` & `pyvisjs-1.0.0b6/folder_structure.txt`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/mkdocs.yml` & `pyvisjs-1.0.0b6/mkdocs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -47,19 +47,19 @@
 
 markdown_extensions:
   - pymdownx.highlight:
       linenums: true
   - pymdownx.superfences
 
 nav:
-  - "Getting started": index.md
+  - "Getting Started": index.md
   - "Documentation":
     - "Network": network.md
     - "Edges": edges.md
     - "Nodes": nodes.md
     - "Options": options.md
   - "Examples":
     - "Installation": installation.md
     - "Basic example": basic-example.md
-#  - "About":
-#    - "Contributing"
-#    - "License"
+  - "About":
+    - "Contributing": CONTRIBUTING.md
+    - "License": LICENSE.md
```

### Comparing `pyvisjs-1.0.0b5/pyproject.toml` & `pyvisjs-1.0.0b6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/pyvisjs/base_dictable.py` & `pyvisjs-1.0.0b6/pyvisjs/base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/pyvisjs/edge.py` & `pyvisjs-1.0.0b6/pyvisjs/edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/pyvisjs/network.py` & `pyvisjs-1.0.0b6/pyvisjs/network.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,17 +50,15 @@
 
         if edges:
             default_data.update({
                 "edges": edges,
             })
 
         if options:
-            default_data.update({
-                "options": options,
-            })
+            default_data["options"] = options
 
         self._data = default_data
 
     def __repr__(self):
         return f"Network(\'{self.name}\')"
     
     def add_node(self, node_id:str, label=None, color=None, shape="dot", size=None, cid=None, **kwargs):
@@ -110,47 +108,54 @@
 
         if not [edge.start for edge in self.edges if edge.start == str(from_id) and edge.end == str(to_id)]:
             self.edges.append(Edge(from_id, to_id, **kwargs))
 
     def to_dict(self):
         return super().to_dict()["_data"]
 
-    def show(self, file_name):
-        self.render_default_template(open_in_browser=True, output_filename=file_name)
+    def show(self, file_name:str=None):
+        if file_name:
+            self.render(open_in_browser=True, output_filename=file_name)
+        else:
+            self.render(open_in_browser=True)
 
-    def _render(self, template_filename:str, open_in_browser=False, save_to_output=False, output_filename="default.html", pyvisjs_options:Dict=None):
+    def render(self, open_in_browser=False, save_to_output=False, output_filename="default.html"):
         network_dict = self.to_dict()
+        pyvisjs_options = None
+        filtering_enabled = False
+
+        if self.options:
+            pyvisjs_options = self.options.pyvisjs.to_dict(nodes=self.nodes, edges=self.edges)
+            filtering_enabled = pyvisjs_options["filtering_enabled"]
+        
+        template_filename = "tom-select.html" if filtering_enabled else "basic.html"
 
         html_output = self.env \
             .get_template(template_filename) \
             .render(
-                width=network_dict["options"].get("width", "100%"),
-                height=network_dict["options"].get("height", "100%"),
                 data=network_dict,
                 pyvisjs=pyvisjs_options or {},
             )
 
         if save_to_output or open_in_browser:
             file_path = save_file(output_filename, html_output)
 
         if open_in_browser:
             open_file(file_path)
 
         return html_output
     
-    def render_default_template(self, open_in_browser=False, save_to_output=False, output_filename="default.html"):
-        return self._render(
-            template_filename="basic.html",
+    def __render_default_template(self, open_in_browser=False, save_to_output=False, output_filename="default.html"):
+        return self.render(
             open_in_browser=open_in_browser,
             save_to_output=save_to_output,
             output_filename=output_filename)
     
 
-    def render_tom_template(self, title:str=None, open_in_browser=False, save_to_output=False, output_filename="default.html", 
-    enable_highlighting=False, edge_filtering=None, node_filtering=None, dropdown_auto_close:bool=True) -> str:
+    def __render_tom_template(self, open_in_browser=False, save_to_output=False, output_filename="default.html") -> str:
         """This method uses jinja to inject prepared data to `'templates\\tom-select.html'` \n
         (for more info about the injected data see Notes section below).
         
         Parameters
         ----------
         open_in_browser: bool, default=False
             Resolved template will be saved as the `output_filename` and opened with `os.startfile`
@@ -203,50 +208,15 @@
         >>>         "node_filtering_lookup": node_filtering_lookup,
         >>>         "title": title,
         >>>         "dropdown_auto_close": dropdown_auto_close,
         >>>     },
         >>> )
 
         you can find more details about `edge_filtering_lookup` and `node_filtering_lookup` structure here `tests\\test_network.py\\test_network_render_template_edge_filtering_list`
-        """
-
-        edge_filtering_lookup: Dict = None
-        node_filtering_lookup: Dict = None
-
-        # edges
-        if not edge_filtering is None:
-            if not isinstance(edge_filtering, list):
-                edge_filtering = [str(edge_filtering)]
-
-            edge_filtering_lookup = {}
-            for field_name in edge_filtering:
-                tp_field_name = Edge.convert_to_template_attribute(field_name)
-                unique_values = list(set([str(getattr(edge, field_name)) for edge in self.edges if hasattr(edge, field_name)]))
-                unique_values.sort()
-                edge_filtering_lookup[tp_field_name] = unique_values
-
-        # nodes
-        if not node_filtering is None:
-            if not isinstance(node_filtering, list):
-                node_filtering = [str(node_filtering)]
-
-            node_filtering_lookup = {}
-            for field_name in node_filtering:
-                unique_values = list(set([str(getattr(node, field_name)) for node in self.nodes if hasattr(node, field_name)]))
-                unique_values.sort()
-                node_filtering_lookup[field_name] = unique_values             
-        
-        pyvisjs_options = {
-                    "enable_highlighting": enable_highlighting,
-                    "edge_filtering_lookup": edge_filtering_lookup,
-                    "node_filtering_lookup": node_filtering_lookup,
-                    "title": title,
-                    "dropdown_auto_close": dropdown_auto_close,
-                };
+        """          
+        
          
-        return self._render(
-            template_filename="tom-select.html",
+        return self.render(
             open_in_browser=open_in_browser,
             save_to_output=save_to_output,
-            output_filename=output_filename,
-            pyvisjs_options=pyvisjs_options)
+            output_filename=output_filename)
```

### Comparing `pyvisjs-1.0.0b5/pyvisjs/node.py` & `pyvisjs-1.0.0b6/pyvisjs/node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/pyvisjs/templates/base.html` & `pyvisjs-1.0.0b6/pyvisjs/templates/base.html`

 * *Files 27% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     {%- endblock %}
     <style type="text/css">
       {% block head_style -%}
       body {
         font-family: 'JetBrains Mono';font-size: 22px;
       }
       #visjsnet {
-          width: {{width}};
-          height: {{height}};
+          width: {{ data["options"]["width"]|default ('100%') }};
+          height: {{ data["options"]["height"]|default ('100%') }};
           border: 1px solid lightgray;
       }
       {%- endblock %}
     </style>
   {%- endblock %}
   </head>
   <body>
```

### Comparing `pyvisjs-1.0.0b5/pyvisjs/templates/bs-container.html` & `pyvisjs-1.0.0b6/pyvisjs/templates/bs-container.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/pyvisjs/templates/create_network.js` & `pyvisjs-1.0.0b6/pyvisjs/templates/create_network.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,24 @@
 const data = create_network();
 data.network.has_hidden_nodes = false;
 //if (data.pyvisjs.enable_highlighting === true) data.network.on("click", hide_not_selected_nodes);
 
 // all jinja injections should happen here because it allows to mock this function and test all the rest in isolation
 function create_network() {
 
+    vis.Network.prototype.Zoom = function(scale) {
+        const animationOptions = {
+            scale: this.getScale() + scale,
+            animation: {
+                duration: 300
+            }
+        };
+        this.view.moveTo(animationOptions);
+    };
+
     // create an array with nodes
     const ds_nodes = new vis.DataSet({
         {
             data["nodes"] | tojson
         }
     });
 
@@ -42,11 +52,11 @@
         network: new vis.Network(container, data, options),
         nodes: ds_nodes.get({
             returnType: "Object"
         }),
         edges: ds_edges.get({
             returnType: "Object"
         }),
-        ds_nodes: ds_nodes,
+        ds_nodes: ds_nodes, // this is needed to make changes to the nodes model through ds_nodes.update()
         pyvisjs: pyvisjs,
     }
 }
```

### Comparing `pyvisjs-1.0.0b5/pyvisjs/templates/draw_title.js` & `pyvisjs-1.0.0b6/pyvisjs/templates/draw_title.js`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/pyvisjs/templates/functions.js` & `pyvisjs-1.0.0b6/pyvisjs/templates/functions.js`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/pyvisjs/templates/init_tomSelect.js` & `pyvisjs-1.0.0b6/pyvisjs/templates/init_tomSelect.js`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/pyvisjs/templates/select-edge-filter.html` & `pyvisjs-1.0.0b6/pyvisjs/templates/select-edge-filter.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/pyvisjs/templates/tom-select.html` & `pyvisjs-1.0.0b6/pyvisjs/templates/tom-select.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/pyvisjs/utils.py` & `pyvisjs-1.0.0b6/pyvisjs/utils.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/pyvisjs.egg-info/PKG-INFO` & `pyvisjs-1.0.0b6/pyvisjs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,21 +36,20 @@
 Requires-Dist: Jinja2
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: all
 Requires-Dist: pyvisjs[test]; extra == "all"
 
 [![pipeline status](https://gitlab.com/22kittens/pyvisjs/badges/main/pipeline.svg)](https://gitlab.com/22kittens/pyvisjs/-/commits/main)
-[![Latest Release](https://gitlab.com/22kittens/pyvisjs/-/badges/release.svg)](https://gitlab.com/22kittens/pyvisjs/-/releases)
 [![PyPI - Version](https://img.shields.io/pypi/v/pyvisjs)](https://pypi.org/project/pyvisjs)
 [![Documentation](https://img.shields.io/badge/ref-Documentation-blue)](https://22kittens.gitlab.io/pyvisjs/)
 
 
 
-# ![logo](docs/img/favicon-32x32.png) - pyvisjs
+# ![logo](https://gitlab.com/uploads/-/system/project/avatar/56819743/favicon-32x32.png) - pyvisjs
 Python wrapper for vis.js Network
 
 > :warning: **Beta version disclaimer** Please note that this package is in a **beta** version and backwards-incompatible changes might be introduced in future releases.
 
 
 pyvisjs is a Python package designed to provide seamless interaction with [vis.js](https://visjs.org) network visualizations, allowing users to manipulate and visualize network data using Python.
 
@@ -87,16 +86,16 @@
 net.show("example.html")
 ```
 
 For more examples and detailed usage, please refer to the [documentation](https://22kittens.gitlab.io/pyvisjs).
 
 ## Contributing
 
-Contributions are welcome! If you have suggestions, feature requests, or find any bugs, please open an issue or submit a pull request. Make sure to follow the [contribution guidelines](CONTRIBUTING.md).
+Contributions are welcome! If you have suggestions, feature requests, or find any bugs, please open an issue or submit a pull request. Make sure to follow the [contribution guidelines](https://22kittens.gitlab.io/pyvisjs/CONTRIBUTING).
 
 ## Acknowledgments
 
 This project is inspired by the [pyvis](https://github.com/WestHealth/pyvis) Python package and the [visNetwork](https://github.com/datastorm-open/visNetwork) R-language package.
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](https://22kittens.gitlab.io/pyvisjs/LICENSE).
```

### Comparing `pyvisjs-1.0.0b5/pyvisjs.egg-info/SOURCES.txt` & `pyvisjs-1.0.0b6/pyvisjs.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 LICENSE
 README.md
 folder_structure.txt
 mkdocs.yml
 pyproject.toml
 requirements-doc.txt
 requirements.txt
+docs/CONTRIBUTING.md
+docs/LICENSE.md
 docs/basic-example.md
 docs/edges.md
 docs/index.md
 docs/installation.md
 docs/network.md
 docs/nodes.md
 docs/options.md
```

### Comparing `pyvisjs-1.0.0b5/tests/test_base_dictable.py` & `pyvisjs-1.0.0b6/tests/test_base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/tests/test_edge.py` & `pyvisjs-1.0.0b6/tests/test_edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/tests/test_network.py` & `pyvisjs-1.0.0b6/tests/test_network.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 import pytest
 from unittest.mock import patch
 from pyvisjs import Network, Node, Edge, Options
 
-def test_network_init():
+# Network
+# ├── __init__ (name, nodes, edges, options)
+# ├── _initialize_data
+# ├── get_options
+# ├── set_options
+# ├── get_nodes
+# ├── get_edges
+# ├── add_node
+# ├── add_edge
+# ├── show
+# ├── render
+# └── to_dict
+
+def test_network_init_default_params():
     # init
     DEFAULT_DICT = {
         "nodes": [],
         "edges": [],
         "options": {}
     }
     # mock
@@ -14,81 +27,157 @@
 
     # call
     n = Network("Network2")
     
     # assert
     assert n.name == "Network2"
     assert n.env is not None
+    assert n._data == DEFAULT_DICT # result of calling _initialize_data
+    assert n.attr_filter_func # from the base class
     assert n.to_dict() == DEFAULT_DICT
 
 def test_network_init_with_data():
     # init
+    TITLE = "My network"
+    PHYSICS_ENABLED = False
     NETWORK_DICT = {
         "nodes": [
             { "id": "1", "label": "node 1", "shape": "dot" },
             { "id": "2", "label": "node 2", "shape": "dot" },
             { "id": "3", "label": "node 3", "shape": "dot" },
         ],
         "edges": [
             { "from": "1", "to": "2" },
             { "from": "2", "to": "3" },
             { "from": "3", "to": "4" }
         ],
-        "options": {}
+        "options": {
+            "physics": {
+                "enabled": PHYSICS_ENABLED
+            }
+        }
     }
     # mock
 
 
     # call
     nd1 = Node(1, "node 1")
     nd2 = Node(2, "node 2")
     nd3 = Node(3, "node 3")
 
     eg1 = Edge(1, 2)
     eg2 = Edge(2, 3)
     eg3 = Edge(3, 4)
 
     opt = Options()
+    opt.pyvisjs.set(title=TITLE)
+    opt.physics.set(enabled=PHYSICS_ENABLED)
 
     n = Network("Network2", [nd1, nd2, nd3], [eg1, eg2, eg3], opt)
     
     # assert
     assert n.name == "Network2"
     assert n.env is not None
     assert n.to_dict() == NETWORK_DICT
 
-def test_network_read_write_properties():
+def test_network_initialize_data():
+    # init
+    DEFAULT_DICT = {
+        "nodes": [],
+        "edges": [],
+        "options": {}
+    }
+
+    NODES = [Node(1), Node(2)]
+    EDGES = [Edge(1, 2)]
+    OPT = Options("100%", "100%")
+
+    INITIALIZED_DICT = {
+        "nodes": NODES,
+        "edges": EDGES,
+        "options": OPT
+    }
+    # mock
+
+    # call
+    n = Network("Network2")
+    n_data_before_init = n._data
+    n._initialize_data(NODES, EDGES, OPT) 
+
+    # assert
+    assert n_data_before_init == DEFAULT_DICT
+    assert n._data == INITIALIZED_DICT
+
+def test_network_get_options_default():
+    # init
+
+    # mock
+
+    # call
+    n = Network("Network2")
+     
+    # assert
+    assert n.options == None
+
+def test_network_get_options():
+    # init
+    TITLE = "Network title"
+    PHYSICS_ENABLED = True
+    # mock
+
+    # call
+    opt = Options()
+    opt.pyvisjs.set(title=TITLE)
+    opt.physics.set(enabled=PHYSICS_ENABLED)
+    n = Network("Network2", options=opt)
+     
+    # assert
+    assert n.options.pyvisjs.title == TITLE
+    assert n.options.physics.enabled == PHYSICS_ENABLED
+
+def test_network_set_options():
+    # init
+    ZOOM_VIEW = True
+    DRAG_NODES = False
+    # mock
+
+    # call
+    n = Network("Network2")
+    n_default_options = n.options
+    n.options = Options().set_interaction(dragNodes=DRAG_NODES, zoomView=ZOOM_VIEW)
+
+    # assert
+    assert n_default_options == None
+    assert n.options.interaction["dragNodes"] == DRAG_NODES
+    assert n.options.interaction["zoomView"] == ZOOM_VIEW
+
+def test_network_get_nodes_and_edges():
     # init
 
     # mock
 
     # call
     nd1 = Node(1, "node 1")
     nd2 = Node(2, "node 2")
     nd3 = Node(3, "node 3")
 
     eg1 = Edge(1, 2)
     eg2 = Edge(2, 3)
     eg3 = Edge(3, 4)
 
-    opt = Options()
-
     n = Network("Network2", [nd1, nd2], [eg1])
-    n.options = opt
     n.nodes.append(nd3)
     n.edges.append(eg2)
     n.edges.append(eg3)
 
     # assert
-    assert n.options == opt
     assert n.nodes == [nd1, nd2, nd3]
     assert n.edges == [eg1, eg2, eg3]
 
-
-def test_network_add_nodes():
+def test_network_add_node():
     # init
 
     # mock
 
     # call
     n = Network("Network1")
     n.add_node(1)
@@ -100,15 +189,15 @@
     assert len(n.nodes) == 3
     assert n.nodes[0].id == "1"
     assert n.nodes[0].label == "1"
     assert n.nodes[1].id == "2"
     assert n.nodes[1].label == "name2"
     assert n.nodes[2].category == "high"
 
-def test_network_add_edges():
+def test_network_add_edge():
     # init
 
     # mock
 
     # call
     n = Network("Network1")
     n.add_node(1)
@@ -127,274 +216,336 @@
     assert n.edges[0].end == "2"
     assert n.edges[1].start == "2"
     assert n.edges[1].end == "3"
     assert n.edges[1].country == "LV"
 
 def test_network_to_dict():
     # init
+    TITLE = "Title1"
+    PHYSICS_ENABLED = True
+
     NETWORK_DICT = {
         "nodes": [
             { "id": "1", "label": "1", "shape": "dot" },
             { "id": "2", "label": "name2", "shape": "dot" },
             { "id": "3", "label": "3", "shape": "dot" },
         ],
         "edges": [
             { "from": "1", "to": "2" },
             { "from": "2", "to": "3" }
         ],
-        "options": {}
+        "options": {
+            "physics": {
+                "enabled": PHYSICS_ENABLED
+            }
+        }
     }
 
     # mock
 
     # call
-    n = Network("Network1")
+    opt = Options()
+    opt.pyvisjs.set(title=TITLE) # pyvisjs key is not going to options.to_dict()
+    opt.physics.set(enabled=PHYSICS_ENABLED) 
+
+    n = Network("Network1", options=opt)
     n.add_node(1)
     n.add_node(2, "name2")
     n.add_edge(1, 2) # both nodes exist
     n.add_edge(2, 3) # one node missing
     n.add_edge(2, 3) # duplicate edge
     
     # assert
     assert n.to_dict() == NETWORK_DICT
 
 @patch('pyvisjs.network.Environment')
-def test_network_render_tom_template_passing_render_default_params(mock_Environment):
+def test_network_render_default_params(mock_Environment):
     # init
-    WIDTH="100%"
-    HEIGHT="100%"
-    DATA={"nodes": [], "edges": [], "options": {}}
-    PYVISJS={
-        "enable_highlighting": False,
-        "edge_filtering_lookup": None,
-        "node_filtering_lookup": None,
-        "title": None,
-        "dropdown_auto_close": True,
-    }
+    DATA = {"nodes": [], "edges": [], "options": {}}
+    PYVISJS = {}
+    TEMPLATE_FILENAME = "basic.html"
     
     # mock
-    mock_render = mock_Environment.return_value.get_template.return_value.render
+    mock_get_template = mock_Environment.return_value.get_template
+    mock_render = mock_get_template.return_value.render
 
     # call
     network = Network("Test Network")
-    html_output = network.render_tom_template() # <--------------------
+    html_output = network.render() # <--------------------
 
     # assert
-    mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
+    mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
+    mock_render.assert_called_once_with(data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.Environment')
-def test_network_render_tom_template_passing_render_params(mock_Environment):
+def test_network_render_pyvisjs_options_only(mock_Environment):
     # init
-    WIDTH="100%"
-    HEIGHT="100%"
     DATA={"nodes": [], "edges": [], "options": {}}
+    TITLE="network title"
     TEMPLATE_FILENAME="tom-select.html"
     ENABLE_HIGHLIGHTING=True
     EDGE_FILTERING="edge_field" # str(!) not list
     NODE_FILTERING=["field1", "field2"] # list
     DROPDOWN_AUTO_CLOSE=False,
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
         "edge_filtering_lookup": {"edge_field": []},
         "node_filtering_lookup": {"field1": [], "field2": []},
-        "title": None,
+        "title": TITLE,
         "dropdown_auto_close": DROPDOWN_AUTO_CLOSE,
+        'filtering_enabled': True,
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
-    network = Network("Test Network")
-    html_output = network.render_tom_template( # <--------------------
-        enable_highlighting=ENABLE_HIGHLIGHTING, 
-        edge_filtering=EDGE_FILTERING, 
+    options = Options()
+    options.pyvisjs.set(title=TITLE).set_filtering(
+        enable_highlighting=ENABLE_HIGHLIGHTING,
+        edge_filtering=EDGE_FILTERING,
         node_filtering=NODE_FILTERING,
-        dropdown_auto_close=DROPDOWN_AUTO_CLOSE)
+        dropdown_auto_close=DROPDOWN_AUTO_CLOSE
+    )
+    network = Network("Test Network", options=options)
+    network.render() # <--------------------
+
+    # assert
+    mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
+    mock_render.assert_called_once_with(data=DATA, pyvisjs=PYVISJS)
+
+@patch('pyvisjs.network.Environment')
+def test_network_render_pyvisjs_options_only_no_filtering(mock_Environment):
+    # init
+    DATA={"nodes": [], "edges": [], "options": {}}
+    TITLE="network title"
+    TEMPLATE_FILENAME="basic.html"
+    PYVISJS={
+        "title": TITLE,
+        'filtering_enabled': False,
+    }
+    
+    # mock
+    mock_get_template = mock_Environment.return_value.get_template
+    mock_render = mock_get_template.return_value.render
+
+    # call
+    options = Options()
+    options.pyvisjs.set(title=TITLE)
+    network = Network("Test Network", options=options)
+    network.render() # <--------------------
 
     # assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
-    mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
+    mock_render.assert_called_once_with(data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.Environment')
-def test_network_render_tom_template_edge_filtering_list(mock_Environment):
+def test_network_render_edge_filtering_list(mock_Environment):
     # init
-    WIDTH="100%"
-    HEIGHT="100%"
     DATA={
         'nodes': [
             {'id': '1', 'label': '1', 'shape': 'dot'}, 
             {'id': '2', 'label': '2', 'shape': 'dot'}, 
             {'id': '3', 'label': '3', 'shape': 'dot'}], 
         'edges': [
             {'to': '2', 'field1': 'AM', 'from': '1'}, 
             {'to': '3', 'field1': 'AM', 'from': '1'}, 
             {'to': '3', 'field1': 'JL', 'from': '2'}], 
         'options': {}
     }
     TEMPLATE_FILENAME="tom-select.html"
     ENABLE_HIGHLIGHTING=True
+    DROPDOWN_AUTOCLOSE=True
     EDGE_FILTERING=["field1", "field2"]
     NODE_FILTERING=["label", "shape"]
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
         "edge_filtering_lookup": {"field1": ["AM", "JL"], "field2": []},
         "node_filtering_lookup": {"label": ["1", "2", "3"], "shape": ["dot"]},
-        "title": None,
-        "dropdown_auto_close": True,
+        "filtering_enabled": True,
+        "dropdown_auto_close": DROPDOWN_AUTOCLOSE,
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
-    net = Network("Network1")
+    options = Options()
+    options.pyvisjs.set_filtering(
+        enable_highlighting=ENABLE_HIGHLIGHTING, 
+        edge_filtering=EDGE_FILTERING,
+        node_filtering=NODE_FILTERING,
+        dropdown_auto_close=DROPDOWN_AUTOCLOSE,
+    )
+    net = Network("Network1", options=options)
     net.add_edge(1, 2, field1="AM")
     net.add_edge(1, 3, field1="AM")
     net.add_edge(2, 3, field1="JL")
-    html_output = net.render_tom_template( # <--------------------
-        enable_highlighting=ENABLE_HIGHLIGHTING, 
-        edge_filtering=EDGE_FILTERING,
-        node_filtering=NODE_FILTERING) 
+    net.render() # <--------------------
+
 
     # assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
-    mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
+    mock_render.assert_called_once_with(data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.Environment')
 def test_network_render_tom_template_edge_filtering_int(mock_Environment):
     # init
-    WIDTH="100%"
-    HEIGHT="100%"
     DATA={"nodes": [], "edges": [], "options": {}}
     TEMPLATE_FILENAME="tom-select.html"
     ENABLE_HIGHLIGHTING=True
     EDGE_FILTERING=34
     NODE_FILTERING=22
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
         "edge_filtering_lookup": {"34": []},
         "node_filtering_lookup": {"22": []},
-        "title": None,
-        "dropdown_auto_close": True,
+        "filtering_enabled": True,
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
-    net = Network("Network1")
-    html_output = net.render_tom_template(# <--------------------
+    options = Options()
+    options.pyvisjs.set_filtering(
         enable_highlighting=ENABLE_HIGHLIGHTING, 
         edge_filtering=EDGE_FILTERING,
-        node_filtering=NODE_FILTERING) 
+        node_filtering=NODE_FILTERING
+    )
+    net = Network("Network1", options=options)
+
+    net.render()# <--------------------
+ 
 
     # assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
-    mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
+    mock_render.assert_called_once_with(data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
-def test_network_render_default_template_with_all_default_values(mock_Environment, mock_save_file, mock_open_file):
+def test_network_render_default_template_and_return_value(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
     DEFAULT_TEMPLATE_FILENAME = "basic.html"
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
     mock_render.return_value = RENDER_RESULT
 
     # call
     network = Network("Test Network")
-    html_output = network.render_default_template() # <--------------------
+    html_output = network.render() # <--------------------
 
     # assert
     mock_get_template.assert_called_once_with(DEFAULT_TEMPLATE_FILENAME)
     mock_save_file.assert_not_called()
     mock_open_file.assert_not_called()
     assert html_output == RENDER_RESULT
 
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
 def test_network_render_template_with_open_in_browser(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
-    TEMPLATE_FILENAME = "some-template-name.html"
+    TEMPLATE_FILENAME = "basic.html"
     DEFAULT_OUTPUT_FILENAME = "default.html"
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
     mock_render.return_value = RENDER_RESULT
     mock_save_file.return_value = DEFAULT_OUTPUT_FILENAME
 
     # call
     network = Network("Test Network")
-    html_output = network._render(TEMPLATE_FILENAME, open_in_browser=True) # <--------------------
+    html_output = network.render(open_in_browser=True) # <--------------------
 
     #assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_save_file.assert_called_once_with(DEFAULT_OUTPUT_FILENAME, RENDER_RESULT)
     mock_open_file.assert_called_once_with(DEFAULT_OUTPUT_FILENAME)
     assert html_output == RENDER_RESULT
 
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
 def test_network_render_template_with_save_to_output(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
-    TEMPLATE_FILENAME = "template-1.html"
+    TEMPLATE_FILENAME = "basic.html"
     DEFAULT_OUTPUT_FILENAME = "default.html"
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
     mock_render.return_value = RENDER_RESULT
 
     # call
     network = Network("Test Network")
-    html_output = network._render(TEMPLATE_FILENAME, save_to_output=True) # <--------------------
+    html_output = network.render(save_to_output=True) # <--------------------
 
     #assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_save_file.assert_called_once_with(DEFAULT_OUTPUT_FILENAME, RENDER_RESULT)
     mock_open_file.assert_not_called()
     assert html_output == RENDER_RESULT
 
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
 def test_network_render_template_with_open_and_save_no_defaults(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
-    TEMPLATE_FILENAME = "custom_template.html"
+    TEMPLATE_FILENAME = "basic.html"
     CUSTOM_OUTPUT_FILENAME = "custom_output.html"
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
     mock_render.return_value = RENDER_RESULT
     mock_save_file.return_value = CUSTOM_OUTPUT_FILENAME
 
     # call
     network = Network("Test Network")
-    html_output = network._render( # <--------------------
-        TEMPLATE_FILENAME,
+    html_output = network.render( # <--------------------
         open_in_browser=True, 
         save_to_output=True, 
         output_filename=CUSTOM_OUTPUT_FILENAME)
 
     #assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_save_file.assert_called_once_with(CUSTOM_OUTPUT_FILENAME, RENDER_RESULT)
     mock_open_file.assert_called_once_with(CUSTOM_OUTPUT_FILENAME)
-    assert html_output == RENDER_RESULT
+    assert html_output == RENDER_RESULT
+
+@patch('pyvisjs.network.Network.render')
+def test_network_show_default_params(mock_render):
+    # init
+    # mock
+    # call
+    net = Network("Network")
+    net.show()
+
+    # assert
+    mock_render.assert_called_once_with(open_in_browser=True)
+
+@patch('pyvisjs.network.Network.render')
+def test_network_show(mock_render):
+    # init
+    FILE_NAME = "output1.html"
+    # mock
+    # call
+    net = Network("Network")
+    net.show(FILE_NAME)
+
+    # assert
+    mock_render.assert_called_once_with(open_in_browser=True, output_filename=FILE_NAME)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyvisjs-1.0.0b5/tests/test_node.py` & `pyvisjs-1.0.0b6/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/tests/test_options.py` & `pyvisjs-1.0.0b6/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b5/tests/test_utils.py` & `pyvisjs-1.0.0b6/tests/test_utils.py`

 * *Files identical despite different names*

