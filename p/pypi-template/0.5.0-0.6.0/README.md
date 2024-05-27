# Comparing `tmp/pypi-template-0.5.0.tar.gz` & `tmp/pypi-template-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi-template-0.5.0.tar", last modified: Sun Jan 21 16:30:53 2024, max compression
+gzip compressed data, was "pypi-template-0.6.0.tar", last modified: Mon May 27 14:44:44 2024, max compression
```

## Comparing `pypi-template-0.5.0.tar` & `pypi-template-0.6.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.901455 pypi-template-0.5.0/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.895851 pypi-template-0.5.0/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     1078 2024-01-20 14:03:02.000000 pypi-template-0.5.0/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1062 2024-01-20 14:03:02.000000 pypi-template-0.5.0/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)      121 2022-05-28 13:55:05.000000 pypi-template-0.5.0/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     2096 2024-01-21 16:30:53.901260 pypi-template-0.5.0/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.896270 pypi-template-0.5.0/pypi_template/
--rw-r--r--   0 xtof       (501) staff       (20)    13283 2024-01-20 14:06:01.000000 pypi-template-0.5.0/pypi_template/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      201 2022-08-08 19:55:13.000000 pypi-template-0.5.0/pypi_template/__main__.py
--rw-r--r--   0 xtof       (501) staff       (20)      828 2023-09-17 11:55:29.000000 pypi-template-0.5.0/pypi_template/module.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.898279 pypi-template-0.5.0/pypi_template/templates/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.898504 pypi-template-0.5.0/pypi_template/templates/(dot)github/
--rw-r--r--   0 xtof       (501) staff       (20)      221 2022-05-28 13:55:05.000000 pypi-template-0.5.0/pypi_template/templates/(dot)github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-05-28 13:55:05.000000 pypi-template-0.5.0/pypi_template/templates/(dot)github/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.898696 pypi-template-0.5.0/pypi_template/templates/(dot)github/workflows/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-05-28 13:55:05.000000 pypi-template-0.5.0/pypi_template/templates/(dot)github/workflows/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1194 2024-01-21 16:10:56.000000 pypi-template-0.5.0/pypi_template/templates/(dot)github/workflows/test.yaml
--rw-r--r--   0 xtof       (501) staff       (20)       69 2022-05-28 13:55:05.000000 pypi-template-0.5.0/pypi_template/templates/(dot)gitignore
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.898925 pypi-template-0.5.0/pypi_template/templates/(package_module_name)/
--rw-r--r--   0 xtof       (501) staff       (20)      115 2022-08-09 19:45:24.000000 pypi-template-0.5.0/pypi_template/templates/(package_module_name)/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      832 2022-08-09 19:46:55.000000 pypi-template-0.5.0/pypi_template/templates/(package_module_name)/module.py
--rw-r--r--   0 xtof       (501) staff       (20)      109 2023-10-31 17:42:14.000000 pypi-template-0.5.0/pypi_template/templates/.gitignore
--rw-r--r--   0 xtof       (501) staff       (20)      570 2024-01-21 16:15:05.000000 pypi-template-0.5.0/pypi_template/templates/.readthedocs.yaml
--rw-r--r--   0 xtof       (501) staff       (20)     1199 2023-09-17 12:16:14.000000 pypi-template-0.5.0/pypi_template/templates/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)       77 2022-05-28 13:55:05.000000 pypi-template-0.5.0/pypi_template/templates/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     3008 2024-01-21 16:04:45.000000 pypi-template-0.5.0/pypi_template/templates/Makefile
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-09 19:47:19.000000 pypi-template-0.5.0/pypi_template/templates/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.899307 pypi-template-0.5.0/pypi_template/templates/base/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-05-28 13:55:05.000000 pypi-template-0.5.0/pypi_template/templates/base/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    33749 2023-09-17 15:36:03.000000 pypi-template-0.5.0/pypi_template/templates/base/classifiers.txt
--rw-r--r--   0 xtof       (501) staff       (20)      988 2023-09-16 14:25:50.000000 pypi-template-0.5.0/pypi_template/templates/base/index.md
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.900335 pypi-template-0.5.0/pypi_template/templates/docs/
--rw-r--r--   0 xtof       (501) staff       (20)      634 2023-09-16 12:45:14.000000 pypi-template-0.5.0/pypi_template/templates/docs/Makefile
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-09 20:01:14.000000 pypi-template-0.5.0/pypi_template/templates/docs/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.900562 pypi-template-0.5.0/pypi_template/templates/docs/_static/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-05-28 13:55:05.000000 pypi-template-0.5.0/pypi_template/templates/docs/_static/.gitignore
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-09 20:01:17.000000 pypi-template-0.5.0/pypi_template/templates/docs/_static/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      117 2023-09-16 14:10:56.000000 pypi-template-0.5.0/pypi_template/templates/docs/code.md
--rw-r--r--   0 xtof       (501) staff       (20)     1222 2023-09-16 16:47:17.000000 pypi-template-0.5.0/pypi_template/templates/docs/conf.py
--rw-r--r--   0 xtof       (501) staff       (20)      739 2022-08-09 20:17:25.000000 pypi-template-0.5.0/pypi_template/templates/docs/contributing.md
--rw-r--r--   0 xtof       (501) staff       (20)      102 2023-09-16 14:18:27.000000 pypi-template-0.5.0/pypi_template/templates/docs/getting-started.md
--rw-r--r--   0 xtof       (501) staff       (20)      174 2023-09-16 14:17:41.000000 pypi-template-0.5.0/pypi_template/templates/docs/index.md
--rw-r--r--   0 xtof       (501) staff       (20)      800 2023-09-16 12:45:14.000000 pypi-template-0.5.0/pypi_template/templates/docs/make.bat
--rw-r--r--   0 xtof       (501) staff       (20)       31 2022-05-28 13:55:05.000000 pypi-template-0.5.0/pypi_template/templates/docs/whats-in-the-box.md
--rw-r--r--   0 xtof       (501) staff       (20)      290 2024-01-17 10:20:48.000000 pypi-template-0.5.0/pypi_template/templates/requirements.docs.txt
--rw-r--r--   0 xtof       (501) staff       (20)       58 2024-01-20 09:36:58.000000 pypi-template-0.5.0/pypi_template/templates/requirements.txt
--rw-r--r--   0 xtof       (501) staff       (20)     1608 2023-09-17 12:32:03.000000 pypi-template-0.5.0/pypi_template/templates/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.900749 pypi-template-0.5.0/pypi_template/templates/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-05-28 13:55:05.000000 pypi-template-0.5.0/pypi_template/templates/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      300 2022-08-09 19:49:45.000000 pypi-template-0.5.0/pypi_template/templates/tests/test_example.py
--rw-r--r--   0 xtof       (501) staff       (20)      213 2024-01-21 16:06:12.000000 pypi-template-0.5.0/pypi_template/templates/tox.ini
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.901059 pypi-template-0.5.0/pypi_template.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     2096 2024-01-21 16:30:53.000000 pypi-template-0.5.0/pypi_template.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)     1798 2024-01-21 16:30:53.000000 pypi-template-0.5.0/pypi_template.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2024-01-21 16:30:53.000000 pypi-template-0.5.0/pypi_template.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       61 2024-01-21 16:30:53.000000 pypi-template-0.5.0/pypi_template.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       63 2024-01-21 16:30:53.000000 pypi-template-0.5.0/pypi_template.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       14 2024-01-21 16:30:53.000000 pypi-template-0.5.0/pypi_template.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       67 2023-09-16 11:48:37.000000 pypi-template-0.5.0/pyproject.toml
--rw-r--r--   0 xtof       (501) staff       (20)       38 2024-01-21 16:30:53.901494 pypi-template-0.5.0/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1888 2024-01-20 14:03:02.000000 pypi-template-0.5.0/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-01-21 16:30:53.900882 pypi-template-0.5.0/tests/
--rw-r--r--   0 xtof       (501) staff       (20)      147 2023-09-17 11:55:29.000000 pypi-template-0.5.0/tests/test_example.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.709087 pypi-template-0.6.0/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.702949 pypi-template-0.6.0/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     1078 2024-01-20 14:03:02.000000 pypi-template-0.6.0/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1062 2024-03-30 17:48:05.000000 pypi-template-0.6.0/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      121 2022-05-28 13:55:05.000000 pypi-template-0.6.0/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     2145 2024-05-27 14:44:44.708873 pypi-template-0.6.0/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.703382 pypi-template-0.6.0/pypi_template/
+-rw-r--r--   0 xtof       (501) staff       (20)    16009 2024-05-27 14:44:06.000000 pypi-template-0.6.0/pypi_template/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      201 2022-08-08 19:55:13.000000 pypi-template-0.6.0/pypi_template/__main__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      828 2023-09-17 11:55:29.000000 pypi-template-0.6.0/pypi_template/module.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.705453 pypi-template-0.6.0/pypi_template/templates/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.705691 pypi-template-0.6.0/pypi_template/templates/(dot)github/
+-rw-r--r--   0 xtof       (501) staff       (20)      221 2022-05-28 13:55:05.000000 pypi-template-0.6.0/pypi_template/templates/(dot)github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-05-28 13:55:05.000000 pypi-template-0.6.0/pypi_template/templates/(dot)github/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.705881 pypi-template-0.6.0/pypi_template/templates/(dot)github/workflows/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-05-28 13:55:05.000000 pypi-template-0.6.0/pypi_template/templates/(dot)github/workflows/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1192 2024-04-01 15:16:38.000000 pypi-template-0.6.0/pypi_template/templates/(dot)github/workflows/test.yaml
+-rw-r--r--   0 xtof       (501) staff       (20)       69 2022-05-28 13:55:05.000000 pypi-template-0.6.0/pypi_template/templates/(dot)gitignore
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.706120 pypi-template-0.6.0/pypi_template/templates/(package_module_name)/
+-rw-r--r--   0 xtof       (501) staff       (20)      115 2022-08-09 19:45:24.000000 pypi-template-0.6.0/pypi_template/templates/(package_module_name)/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      832 2022-08-09 19:46:55.000000 pypi-template-0.6.0/pypi_template/templates/(package_module_name)/module.py
+-rw-r--r--   0 xtof       (501) staff       (20)      115 2024-01-24 16:06:32.000000 pypi-template-0.6.0/pypi_template/templates/.gitignore
+-rw-r--r--   0 xtof       (501) staff       (20)      570 2024-01-21 16:15:05.000000 pypi-template-0.6.0/pypi_template/templates/.readthedocs.yaml
+-rw-r--r--   0 xtof       (501) staff       (20)     1199 2024-03-30 17:42:45.000000 pypi-template-0.6.0/pypi_template/templates/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       77 2022-05-28 13:55:05.000000 pypi-template-0.6.0/pypi_template/templates/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     3337 2024-04-07 13:47:28.000000 pypi-template-0.6.0/pypi_template/templates/Makefile
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-09 19:47:19.000000 pypi-template-0.6.0/pypi_template/templates/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.706522 pypi-template-0.6.0/pypi_template/templates/base/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-05-28 13:55:05.000000 pypi-template-0.6.0/pypi_template/templates/base/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    34534 2024-04-01 13:32:57.000000 pypi-template-0.6.0/pypi_template/templates/base/classifiers.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      988 2023-09-16 14:25:50.000000 pypi-template-0.6.0/pypi_template/templates/base/index.md
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.707538 pypi-template-0.6.0/pypi_template/templates/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)      634 2023-09-16 12:45:14.000000 pypi-template-0.6.0/pypi_template/templates/docs/Makefile
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-09 20:01:14.000000 pypi-template-0.6.0/pypi_template/templates/docs/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.707762 pypi-template-0.6.0/pypi_template/templates/docs/_static/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-05-28 13:55:05.000000 pypi-template-0.6.0/pypi_template/templates/docs/_static/.gitignore
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-09 20:01:17.000000 pypi-template-0.6.0/pypi_template/templates/docs/_static/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      117 2023-09-16 14:10:56.000000 pypi-template-0.6.0/pypi_template/templates/docs/code.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1222 2023-09-16 16:47:17.000000 pypi-template-0.6.0/pypi_template/templates/docs/conf.py
+-rw-r--r--   0 xtof       (501) staff       (20)      736 2024-04-09 05:56:58.000000 pypi-template-0.6.0/pypi_template/templates/docs/contributing.md
+-rw-r--r--   0 xtof       (501) staff       (20)      102 2023-09-16 14:18:27.000000 pypi-template-0.6.0/pypi_template/templates/docs/getting-started.md
+-rw-r--r--   0 xtof       (501) staff       (20)      174 2023-09-16 14:17:41.000000 pypi-template-0.6.0/pypi_template/templates/docs/index.md
+-rw-r--r--   0 xtof       (501) staff       (20)      800 2023-09-16 12:45:14.000000 pypi-template-0.6.0/pypi_template/templates/docs/make.bat
+-rw-r--r--   0 xtof       (501) staff       (20)       31 2022-05-28 13:55:05.000000 pypi-template-0.6.0/pypi_template/templates/docs/whats-in-the-box.md
+-rw-r--r--   0 xtof       (501) staff       (20)      290 2024-01-17 10:20:48.000000 pypi-template-0.6.0/pypi_template/templates/requirements.docs.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       58 2024-01-20 09:36:58.000000 pypi-template-0.6.0/pypi_template/templates/requirements.txt
+-rw-r--r--   0 xtof       (501) staff       (20)     1608 2023-09-17 12:32:03.000000 pypi-template-0.6.0/pypi_template/templates/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.707966 pypi-template-0.6.0/pypi_template/templates/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-05-28 13:55:05.000000 pypi-template-0.6.0/pypi_template/templates/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      300 2022-08-09 19:49:45.000000 pypi-template-0.6.0/pypi_template/templates/tests/test_example.py
+-rw-r--r--   0 xtof       (501) staff       (20)      173 2024-04-01 15:12:14.000000 pypi-template-0.6.0/pypi_template/templates/tox.ini
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.708583 pypi-template-0.6.0/pypi_template.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     2145 2024-05-27 14:44:44.000000 pypi-template-0.6.0/pypi_template.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)     1819 2024-05-27 14:44:44.000000 pypi-template-0.6.0/pypi_template.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2024-05-27 14:44:44.000000 pypi-template-0.6.0/pypi_template.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       61 2024-05-27 14:44:44.000000 pypi-template-0.6.0/pypi_template.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       82 2024-05-27 14:44:44.000000 pypi-template-0.6.0/pypi_template.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       14 2024-05-27 14:44:44.000000 pypi-template-0.6.0/pypi_template.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      246 2024-04-01 15:10:32.000000 pypi-template-0.6.0/pyproject.toml
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2024-05-27 14:44:44.709130 pypi-template-0.6.0/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1917 2024-04-01 13:04:17.000000 pypi-template-0.6.0/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-05-27 14:44:44.708284 pypi-template-0.6.0/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)      147 2023-09-17 11:55:29.000000 pypi-template-0.6.0/tests/test_example.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1236 2024-04-03 18:28:52.000000 pypi-template-0.6.0/tests/test_values.py
```

### Comparing `pypi-template-0.5.0/.github/README.md` & `pypi-template-0.6.0/.github/README.md`

 * *Files identical despite different names*

### Comparing `pypi-template-0.5.0/LICENSE.txt` & `pypi-template-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypi-template-0.5.0/PKG-INFO` & `pypi-template-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-template
-Version: 0.5.0
+Version: 0.6.0
 Summary: Template-based common/best practices for managing a Python package on PyPi
 Home-page: https://github.com/christophevg/pypi-template
 Author: Christophe VG
 License: MIT
 Keywords: python pypi package management template
 Classifier: Environment :: Console
 Classifier: Development Status :: 4 - Beta
@@ -21,14 +21,16 @@
 License-File: LICENSE.txt
 Requires-Dist: jinja2
 Requires-Dist: pyyaml
 Requires-Dist: prompt-toolkit
 Requires-Dist: colorama
 Requires-Dist: fire
 Requires-Dist: importlib-resources
+Requires-Dist: requests
+Requires-Dist: packaging
 
 # PyPi Template
 
 > Template-based common/best practices for managing a Python package on PyPi
 
 [![Latest Version on PyPI](https://img.shields.io/pypi/v/pypi-template.svg)](https://pypi.python.org/pypi/pypi-template/)
 [![Supported Implementations](https://img.shields.io/pypi/pyversions/pypi-template.svg)](https://pypi.python.org/pypi/pypi-template/)
```

### Comparing `pypi-template-0.5.0/pypi_template/__init__.py` & `pypi-template-0.6.0/pypi_template/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 import os
 import datetime
 
 import importlib_resources
 
 from jinja2 import Environment, PackageLoader, meta
 
+import json
 import yaml
 
 from prompt_toolkit.completion import FuzzyWordCompleter
 from prompt_toolkit import prompt
 from prompt_toolkit.styles import Style
 from colorama import init, Fore
 
 import subprocess
 
+import requests
+from packaging import version as packaging_version
+
 style = Style.from_dict({ "underlined": "underline" })
 init(autoreset=True)
 
 class PyPiTemplate():
 
   """
   manage a PyPi-published Python project using templates.
@@ -40,56 +44,74 @@
       % pypi-template apply          # e.g. after an upgrade of pypi-template
       % pypi-template edit requires  # to add an additional dependency
       % pypi-template yes edit all   # to edit any new variables
   """
   
   def __init__(self):
     # operational setup
-    self._started        = False
     self._be_verbose     = False
     self._show_debug     = False
     self._say_yes_to_all = False
+    self._as_json        = False
   
     # setup Jinja Template Engine
     self._environment = Environment(
       loader=PackageLoader("pypi_template", "templates")
     )
-    self._environment.keep_trailing_newline=True
+    self._environment.keep_trailing_newline = True
 
-    # substitution/template variables
+    # default, not exposed, system-style dynamic variables
     self._system_vars = {
       "now"                   : datetime.datetime.now().isoformat(),
       "current_year"          : str(datetime.datetime.now().year),
       "pypi_template_version" : __version__
     }
+    # substitution/template variables that are lists, not single values
     self._var_lists = {
       "classifiers"     : self._load_classifiers(),
       "requires"        : None,
       "console_scripts" : None,
       "scripts"         : None,
       "skip"            : None
     }
+    # key/value substitution/template variables
     self._template_vars  = {}
+
+    # system vars that are in the .pypi-template
+    self._system_template_vars = {
+      "version" : __version__
+    }
+
+    # all templates
     self._templates      = {}
+    
+    # tracking changes applied to _template_vars
     self._changes        = {}
+
+    # default default values
     self._default_values = {
       "readme"                    : ".github/README.md",
       "first_year_of_publication" : self._system_vars["current_year"],
     }
+    
+    # load personal default values, saved variables (from .pypi-template)
+    # and discover all templates and variables that have been used on them
     self._load_personal_default_values()
+    self._load_vars()
+    self._collect_templates()
     
-  # fire default output
-  
+  # fire default output - if there are unapplied changes, notify them when
+  # exiting - and thus losing them
   def __str__(self):
     if self._changes:
       return f"unapplied changes:\n{yaml.dump(self._changes)}"
     else:
       return ""
 
-  # operational setup
+  # operational setup commands
 
   def verbose(self):
     """
     Explain everything that is done. (chainable)
     """
     self._be_verbose = True
     return self
@@ -105,71 +127,76 @@
     """
     Accept all previous values for variables. Only not yet initialized variables
     need handling. (chainable)
     """
     self._say_yes_to_all = True
     return self
 
-  # commands
+  def json(self):
+    """
+    Format output as a JSON string
+    """
+    self._as_json = True
+    return self
 
+  # values
+
+  @property
   def version(self):
     """
     Output PyPiTemplate's version.
     """
-    return __version__
+    return self._out(__version__)
+
+  @property
+  def variables(self):
+    """
+    Return a list of all available template variables you can edit.
+    """
+    return self._out(
+      sorted(list(self._template_vars.keys()) + list(self._var_lists.keys()))
+    )
+
+  @property
+  def defaults(self):
+    """
+    Return a list of all default template variables values.
+    """
+    return self._out(self._default_values)
+
+  @property
+  def uninitialized(self):
+    """
+    Return a list of template variables that don't have a value yet.
+    """
+    return self._out([ key for key in self.variables if self[key] is None ])
+
+  # commands
 
   def path(self, p):
     """
     Set the path to the provided one. Defaults to the current working directory.
     (chainable)
     """
     os.chdir(p)
     return self
 
   def init(self):
     """
     Initialize a fresh project.
     """
-    self._start(notify_uninitialized=False)
     self.edit("all")
     self.apply()
     if self._going_to("👷‍♂️ performing post-init install (e.g. environments)"):
       subprocess.run(["make", "install"])
 
-  def variables(self):
-    """
-    Return a list of all available template variables you can edit.
-    """
-    self._start()
-    return list(self._template_vars.keys()) + list(self._var_lists.keys())
-
-  def defaults(self):
-    """
-    Return a list of all default template variables values.
-    """
-    self._start()
-    return self._default_values
-
-  def uninitialized(self):
-    """
-    Return a list of template variables that don't have a value yet.
-    """
-    self._start()
-    return [
-      key
-      for key in self.variables()
-      if key not in self._template_vars
-      or self._template_vars[key] is None
-    ]
-
   def edit(self, variable):
     """
     Edit a variable (or provide "all") and apply the change. (chainable)
     """
-    self._start()
     if variable == "all":
       self._collect_all_vars()
     else:
       self._collect_var(variable, force=True)
 
     return self
 
@@ -181,101 +208,111 @@
     self._append("skip", target)
     return self
 
   def apply(self):
     """
     Apply the currently registered configuration.
     """
-    self._start()
     self.save()
     self._render_files()
 
   def save(self):
     """
     Save the current set of variables to `.pypi-template` (chainable)
     """
     if self._changes:
       if self._going_to("💾 saving variables"):
         with open(".pypi-template", "w", encoding="utf-8") as outfile:
-          yaml.safe_dump(self._template_vars, outfile, default_flow_style=False)
-    self.changes = {}
+          yaml.safe_dump(
+            {**self._template_vars, **self._system_template_vars},
+            outfile, default_flow_style=False
+          )
+      self._changes = {}
+    return self
+
+  def status(self):
+    """
+    Perform a few sanity checks (chainable)
+    """
+    if all([
+      self._check_pypi_version(),
+      self._check_uninitialized_variables(),
+      self._check_config_version()
+    ]):
+      print("😎 everyhing is OK")
     return self
 
   # helper functions
   
-  def _being_verbose(self, msg):
-    if self._be_verbose or self._show_debug:
-      print(msg)
-      return True
-    return False
-  
-  def _debugging(self, msg):
-    if self._show_debug:
-      print(msg)
-      return True
-    return False
+  def _check_pypi_version(self):
+    # notify of newer version
+    response = requests.get("https://pypi.org/pypi/pypi-template/json")
+    latest_version = response.json()['info']['version']
+    if packaging_version.parse(self.version) < packaging_version.parse(latest_version):
+      print(f"🚨 a newer version of pypi-template ({latest_version}) is available")
+      print( "   👉 issue 'pip install -U pypi-template' to upgrade!")
+      return False
+    return True
 
-  def _going_to(self, msg):
-    prefix = ""
-    # leading whitespace + icon
-    while msg.startswith(" ") or msg[1] == " ":
-      prefix += msg[0]
-      msg = msg[1:]
-    if not self._debugging(f"{prefix}not really {msg}"):
-      self._being_verbose(f"{prefix}{msg}")
-      return True
-    return False
-  
-  def _load_classifiers(self):
-    return str(
-      self._load_resource("base", "classifiers.txt"), "utf-8"
-    ).split("\n")
+  def _check_uninitialized_variables(self):
+    # notify of uninitialized variables
+    if self.uninitialized:
+      plural = "s" if len(self.uninitialized) > 1 else ""
+      print(f"🚨 uninitialized template variable{plural}: {', '.join(self.uninitialized)}")
+      print( "   👉 issue 'yes edit all apply' to fix!")
+      return False
+    return True
 
-  def _load_resource(self, *args):
-    f = importlib_resources.files(__name__).joinpath("templates", *args)
-    return f.read_bytes()
+  def _check_config_version(self):
+    # notify if version in config isn't current
+    config_version = self._system_template_vars["version"]
+    if config_version != self.version:
+      print(f"🚨 pypi-template config version {config_version} != {self.version}")
+      print( "   👉 issue 'save' to update!")
+      return False
+    return True
 
-  def _list_resources(self, package="pypi_template.templates"):
-    excluded_ext = ".pyc"
-    excluded     = [
-      "__pycache__",
-      "pypi_template.templates.__init__.py",
-      "pypi_template.templates.(dot)github.__init__.py",
-      "pypi_template.templates.base.__init__.py",
-      "pypi_template.templates.docs._static.__init__.py"
-    ]
-    files = []
+  # template vars are items of self
 
-    for entry in importlib_resources.files(package).iterdir():
-      resource = entry.name
-      if resource.endswith(excluded_ext) or \
-         resource in excluded or \
-         f"{package}.{resource}" in excluded:
-        pass
-      elif importlib_resources.files(package).joinpath(resource).is_dir():
-        subfiles = self._list_resources(f"{package}.{resource}")
-        files += [ os.path.join(resource, f) for f in subfiles ]
-      else:
-        files.append(resource)
-    return files
+  def __getitem__(self, key):
+    try:
+      return self._template_vars[key]
+    except KeyError:
+      pass
+    return None
 
-  def _start(self, notify_uninitialized=True):
-    if not self._started:
-      self._load_vars()
-      self._collect_templates()
-      self._started = True
-      if self.uninitialized() and notify_uninitialized:
-        plural = "s" if len(self.uninitialized()) > 1 else ""
-        print(f"🚨 uninitialized template variable{plural}: {self.uninitialized()}")
+  def __setitem__(self, var, value):
+    current = self[var]
+    if value != current:
+      self._debugging(f"👉 recording change {current} -> {value}")
+      self._template_vars[var] = value
+      self._changes[var] = {
+        "old" : current,
+        "new" : value
+      }
+
+  def __delitem__(self, key):
+    del self._template_vars[key]
+
+  # variables helpers
 
   def _load_vars(self):
     try:
       with open(".pypi-template", encoding="utf-8") as fp:
         self._template_vars = yaml.safe_load(fp)
-    except Exception:
+      self._debugging("💾 loaded .pypy-template")
+      for key, value in self._template_vars.items():
+        self._debugging(f"  {key} = {value} {'⚙️' if key in self._system_template_vars else ''}")
+      # move the version to the system_template_vars
+      # since it isn't a real (template) var
+      for key in self._system_template_vars.keys():
+        self._system_template_vars[key] = self._template_vars.pop("version", None)
+    except FileNotFoundError:
+      pass
+    except KeyError:
       pass
 
   def _load_personal_default_values(self):
     try:
       with open(os.path.expanduser("~/.pypi-template"), encoding="utf-8") as fp:
         self._default_values.update(yaml.safe_load(fp))
     except Exception:
@@ -292,37 +329,22 @@
         if var not in self._template_vars and var not in self._system_vars:
           self._template_vars[var] = None
 
   def _collect_all_vars(self):
     for var in sorted(self._template_vars.keys()):
       self._collect_var(var)
 
-  def _update(self, var, value):
-    self._start()
-    try:
-      current = self._template_vars[var]
-    except KeyError:
-      current = None
-    if value != current:
-      self._debugging(f"👉 recording change {current} -> {value}")
-      self._template_vars[var] = value
-      self._changes[var] = {
-        "old" : current,
-        "new" : value
-      }
-
   def _append(self, var, value):
-    self._start()
     try:
       current = self._template_vars[var].copy()
     except KeyError:
       current = []
     if value not in current:
       self._debugging(f"appending {value} to {current}")
-      self._update(var, current + [value])
+      self[var] = current + [value]
 
   def _collect_var(self, var, force=False):
     try:
       current = self._template_vars[var]
       if not force and current is not None and self._say_yes_to_all:
         return
       if var in self._var_lists:
@@ -335,17 +357,17 @@
   def __collect_var_value(self, var, current):
     question = f"{var.replace('_', ' ').capitalize()}: "
     if current is None:
       if var in self._default_values:
         current = self._default_values[var]
       else:
         current = ""
-    self._update(var, prompt(
+    self[var] = prompt(
       [("class:underlined", question)], style=style, default=current
-    ))
+    )
 
   def __collect_var_selections(self, var, current=None):
     if not current:
       current = []
     if len(current) > 0:
       print(Fore.BLUE + f"Current {var.replace('_', ' ')}:")
       for selection in current:
@@ -365,15 +387,15 @@
           complete_while_typing=True
         )
       else:
         selection = prompt([("class:underlined", question)], style=style)
       if selection != "":
         if selection not in selections:
           selections.append(selection)
-    self._update(var, selections)
+    self[var] = selections
     
   def _changed_files(self):
     excluded = [ "base/index.md", "base/classifiers.txt" ]
     reported = []
     
     def _is_skipped_folder(folder):
       for path in self._template_vars["skip"]:
@@ -423,19 +445,86 @@
         if new_content == original_content:
           self._being_verbose(f"✅ {filename} has no changes")
           continue
         self._being_verbose(f"✍️  {filename} was changed")
         self._backup(filename)
       self._write_file(filename, new_content)
 
+  # filesystem helpers
+
   def _mkdir(self, directory):
     if self._going_to(f"📁 creating directory {directory}"):
       os.makedirs(directory)
 
   def _backup(self, filename):
     if self._going_to(f"   💾 backing up {filename}"):
       os.rename(filename, filename + ".backup")
 
   def _write_file(self, filename, new_content):
     if self._going_to(f"   💾 writing {filename}"):
       with open(filename, "w", encoding="utf-8") as outfile:
         outfile.write(new_content)
+
+  # output helpers
+  
+  def _out(self, data):
+    if self._as_json:
+      return json.dumps(data, indent=2, default=str)
+    return data
+
+  def _being_verbose(self, msg):
+    if self._be_verbose or self._show_debug:
+      print(msg)
+      return True
+    return False
+  
+  def _debugging(self, msg):
+    if self._show_debug:
+      print(msg)
+      return True
+    return False
+
+  def _going_to(self, msg):
+    prefix = ""
+    # leading whitespace + icon
+    while msg.startswith(" ") or msg[1] == " ":
+      prefix += msg[0]
+      msg = msg[1:]
+    if not self._debugging(f"{prefix}not really {msg}"):
+      self._being_verbose(f"{prefix}{msg}")
+      return True
+    return False
+  
+  # resources helpers
+  
+  def _load_classifiers(self):
+    return str(
+      self._load_resource("base", "classifiers.txt"), "utf-8"
+    ).split("\n")
+
+  def _load_resource(self, *args):
+    f = importlib_resources.files(__name__).joinpath("templates", *args)
+    return f.read_bytes()
+
+  def _list_resources(self, package="pypi_template.templates"):
+    excluded_ext = ".pyc"
+    excluded     = [
+      "__pycache__",
+      "pypi_template.templates.__init__.py",
+      "pypi_template.templates.(dot)github.__init__.py",
+      "pypi_template.templates.base.__init__.py",
+      "pypi_template.templates.docs._static.__init__.py"
+    ]
+    files = []
+
+    for entry in importlib_resources.files(package).iterdir():
+      resource = entry.name
+      if resource.endswith(excluded_ext) or \
+         resource in excluded or \
+         f"{package}.{resource}" in excluded:
+        pass
+      elif importlib_resources.files(package).joinpath(resource).is_dir():
+        subfiles = self._list_resources(f"{package}.{resource}")
+        files += [ os.path.join(resource, f) for f in subfiles ]
+      else:
+        files.append(resource)
+    return files
```

### Comparing `pypi-template-0.5.0/pypi_template/module.py` & `pypi-template-0.6.0/pypi_template/module.py`

 * *Files identical despite different names*

### Comparing `pypi-template-0.5.0/pypi_template/templates/(dot)github/workflows/test.yaml` & `pypi-template-0.6.0/pypi_template/templates/(dot)github/workflows/test.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python {% raw %}${{ matrix.python-version }}{% endraw %}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: {% raw %}${{ matrix.python-version }}{% endraw %}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install ruff pytest coverage
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
       - name: Lint with ruff
         run: |
           # stop the build if there are Python syntax errors or undefined names
-          ruff --output-format=github --select=E9,F63,F7,F82 --target-version=py38 .
+          ruff check --output-format=github --select=E9,F63,F7,F82 --target-version=py38 .
           # default set of ruff rules with GitHub Annotations
-          ruff --output-format=github --target-version=py38 .
+          ruff check --output-format=github --target-version=py38 .
       - name: Test with PyTest and generate coverage report
         run: |
-          coverage run -m --omit="*/.tox/*,*/distutils/*,tests/*" pytest
+          coverage run -m pytest
           coverage lcov
+          coverage report
       - name: Coveralls
         uses: coverallsapp/github-action@v2
```

### Comparing `pypi-template-0.5.0/pypi_template/templates/(package_module_name)/module.py` & `pypi-template-0.6.0/pypi_template/templates/(package_module_name)/module.py`

 * *Files identical despite different names*

### Comparing `pypi-template-0.5.0/pypi_template/templates/.readthedocs.yaml` & `pypi-template-0.6.0/pypi_template/templates/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pypi-template-0.5.0/pypi_template/templates/LICENSE.txt` & `pypi-template-0.6.0/pypi_template/templates/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypi-template-0.5.0/pypi_template/templates/Makefile` & `pypi-template-0.6.0/pypi_template/templates/Makefile`

 * *Files 23% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 
 # test envs
 
 PYTHON_VERSIONS ?= 3.8.12 3.9.18 3.10.13 3.11.5
 RUFF_PYTHON_VERSION ?= py38
 
 PROJECT=$(shell basename $(CURDIR))
-PACKAGE_NAME=`cat .pypi-template | grep "^package_module_name" | cut -d":" -f2`
+PACKAGE_NAME=`cat .pypi-template | grep "^package_module_name" | cut -d":" -f2 | xargs`
 
-RUN_CMD?=python -m $(PACKAGE_NAME)
+LOG_LEVEL?=ERROR
+SILENT?=yes
+
+RUN_CMD?=LOG_LEVEL=$(LOG_LEVEL) python -m $(PACKAGE_NAME)
 RUN_ARGS?=
 
 TEST_ENVS=$(addprefix $(PROJECT)-test-,$(PYTHON_VERSIONS))
 
 install: install-env-run install-env-docs install-env-test
 	@echo "👷‍♂️ $(BLUE)installing requirements in $(PROJECT)$(NC)"
 	pyenv local $(PROJECT)
@@ -45,15 +48,15 @@
 
 $(PROJECT)-test-%:
 	@echo "👷‍♂️ $(BLUE)creating virtual test environment $@$(NC)"
 	pyenv local --unset
 	-pyenv virtualenv $* $@ > /dev/null
 	pyenv local $@
 	pip install -U pip > /dev/null
-	pip install -U ruff tox > /dev/null
+	pip install -U ruff tox coverage > /dev/null
 
 uninstall: uninstall-envs
 
 uninstall-envs: uninstall-env-test uninstall-env-docs uninstall-env-run env clean-env
 
 uninstall-env-test: $(addprefix uninstall-env-test-,$(PYTHON_VERSIONS))
 
@@ -67,36 +70,44 @@
 
 upgrade:
 	@pip list --outdated | tail +3 | cut -d " " -f 1 | xargs -n1 pip install -U
 
 # env switching
 
 env-%:
-	pyenv local $(PROJECT)-$*
+	@echo "👷‍♂️ $(BLUE)activating $* environment$(NC)"
+	@pyenv local $(PROJECT)-$*
 
 env:
-	pyenv local $(PROJECT)
+	@echo "👷‍♂️ $(BLUE)activating project environment$(NC)"
+	@pyenv local $(PROJECT)
 
 env-test:
-	pyenv local $(TEST_ENVS)
+	@echo "👷‍♂️ $(BLUE)activating test environments$(NC)"
+	@pyenv local $(TEST_ENVS)
 	
 # functional targets
 
 run: env-run
-	$(RUN_CMD) $(RUN_ARGS)
+	@echo "👷‍♂️ $(BLUE)running$(GREEN) $(RUN_CMD) $(RUN_ARGS)$(NC)"
+	@$(RUN_CMD) $(RUN_ARGS)
 
 test: env-test lint
+ifeq ($(SILENT),yes)
+	tox -q
+else
 	tox
+endif
 
 coverage: test
 	coverage report
+	coverage lcov
 
 lint: env-test
-	ruff --select=E9,F63,F7,F82 --target-version=$(RUFF_PYTHON_VERSION) .
-	ruff --target-version=$(RUFF_PYTHON_VERSION) .
+	ruff check --target-version=$(RUFF_PYTHON_VERSION) .
 
 docs: env-docs
 	cd docs; make html
 	open docs/_build/html/index.html
 
 # packaging targets
```

### Comparing `pypi-template-0.5.0/pypi_template/templates/base/classifiers.txt` & `pypi-template-0.6.0/pypi_template/templates/base/classifiers.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 Environment :: GPU :: NVIDIA CUDA :: 11.5
 Environment :: GPU :: NVIDIA CUDA :: 11.6
 Environment :: GPU :: NVIDIA CUDA :: 11.7
 Environment :: GPU :: NVIDIA CUDA :: 11.8
 Environment :: GPU :: NVIDIA CUDA :: 12
 Environment :: GPU :: NVIDIA CUDA :: 12 :: 12.0
 Environment :: GPU :: NVIDIA CUDA :: 12 :: 12.1
+Environment :: GPU :: NVIDIA CUDA :: 12 :: 12.2
 Environment :: Handhelds/PDA's
 Environment :: MacOS X
 Environment :: MacOS X :: Aqua
 Environment :: MacOS X :: Carbon
 Environment :: MacOS X :: Cocoa
 Environment :: No Input/Output (Daemon)
 Environment :: OpenStack
@@ -114,14 +115,15 @@
 Framework :: Django :: 3.0
 Framework :: Django :: 3.1
 Framework :: Django :: 3.2
 Framework :: Django :: 4
 Framework :: Django :: 4.0
 Framework :: Django :: 4.1
 Framework :: Django :: 4.2
+Framework :: Django :: 5.0
 Framework :: Django CMS
 Framework :: Django CMS :: 3.4
 Framework :: Django CMS :: 3.5
 Framework :: Django CMS :: 3.6
 Framework :: Django CMS :: 3.7
 Framework :: Django CMS :: 3.8
 Framework :: Django CMS :: 3.9
@@ -146,25 +148,27 @@
 Framework :: Jupyter :: JupyterLab :: Extensions :: Mime Renderers
 Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Framework :: Jupyter :: JupyterLab :: Extensions :: Themes
 Framework :: Kedro
 Framework :: Lektor
 Framework :: Masonite
 Framework :: Matplotlib
+Framework :: MkDocs
 Framework :: Nengo
 Framework :: Odoo
 Framework :: Odoo :: 8.0
 Framework :: Odoo :: 9.0
 Framework :: Odoo :: 10.0
 Framework :: Odoo :: 11.0
 Framework :: Odoo :: 12.0
 Framework :: Odoo :: 13.0
 Framework :: Odoo :: 14.0
 Framework :: Odoo :: 15.0
 Framework :: Odoo :: 16.0
+Framework :: Odoo :: 17.0
 Framework :: Opps
 Framework :: Paste
 Framework :: Pelican
 Framework :: Pelican :: Plugins
 Framework :: Pelican :: Themes
 Framework :: Plone
 Framework :: Plone :: 3.2
@@ -179,28 +183,32 @@
 Framework :: Plone :: 5.3
 Framework :: Plone :: 6.0
 Framework :: Plone :: 6.1
 Framework :: Plone :: Addon
 Framework :: Plone :: Core
 Framework :: Plone :: Distribution
 Framework :: Plone :: Theme
+Framework :: PySimpleGUI
+Framework :: PySimpleGUI :: 4
+Framework :: PySimpleGUI :: 5
 Framework :: Pycsou
 Framework :: Pydantic
 Framework :: Pydantic :: 1
 Framework :: Pydantic :: 2
 Framework :: Pylons
 Framework :: Pyramid
 Framework :: Pytest
 Framework :: Review Board
 Framework :: Robot Framework
 Framework :: Robot Framework :: Library
 Framework :: Robot Framework :: Tool
 Framework :: Scrapy
 Framework :: Setuptools Plugin
 Framework :: Sphinx
+Framework :: Sphinx :: Domain
 Framework :: Sphinx :: Extension
 Framework :: Sphinx :: Theme
 Framework :: Trac
 Framework :: Trio
 Framework :: Tryton
 Framework :: TurboGears
 Framework :: TurboGears :: Applications
@@ -208,14 +216,15 @@
 Framework :: Twisted
 Framework :: Wagtail
 Framework :: Wagtail :: 1
 Framework :: Wagtail :: 2
 Framework :: Wagtail :: 3
 Framework :: Wagtail :: 4
 Framework :: Wagtail :: 5
+Framework :: Wagtail :: 6
 Framework :: ZODB
 Framework :: Zope
 Framework :: Zope2
 Framework :: Zope3
 Framework :: Zope :: 2
 Framework :: Zope :: 3
 Framework :: Zope :: 4
@@ -263,14 +272,15 @@
 License :: OSI Approved :: BSD License
 License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
 License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 License :: OSI Approved :: Common Development and Distribution License 1.0 (CDDL-1.0)
 License :: OSI Approved :: Common Public License
 License :: OSI Approved :: Eclipse Public License 1.0 (EPL-1.0)
 License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
+License :: OSI Approved :: Educational Community License, Version 2.0 (ECL-2.0)
 License :: OSI Approved :: Eiffel Forum License
 License :: OSI Approved :: European Union Public Licence 1.0 (EUPL 1.0)
 License :: OSI Approved :: European Union Public Licence 1.1 (EUPL 1.1)
 License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 License :: OSI Approved :: GNU Affero General Public License v3
 License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 License :: OSI Approved :: GNU Free Documentation License (FDL)
@@ -294,14 +304,15 @@
 License :: OSI Approved :: MITRE Collaborative Virtual Workspace License (CVW)
 License :: OSI Approved :: MirOS License (MirOS)
 License :: OSI Approved :: Motosoto License
 License :: OSI Approved :: Mozilla Public License 1.0 (MPL)
 License :: OSI Approved :: Mozilla Public License 1.1 (MPL 1.1)
 License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
+License :: OSI Approved :: NASA Open Source Agreement v1.3 (NASA-1.3)
 License :: OSI Approved :: Nethack General Public License
 License :: OSI Approved :: Nokia Open Source License
 License :: OSI Approved :: Open Group Test Suite License
 License :: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 License :: OSI Approved :: PostgreSQL License
 License :: OSI Approved :: Python License (CNRI Python License)
 License :: OSI Approved :: Python Software Foundation License
@@ -313,14 +324,15 @@
 License :: OSI Approved :: Sun Public License
 License :: OSI Approved :: The Unlicense (Unlicense)
 License :: OSI Approved :: Universal Permissive License (UPL)
 License :: OSI Approved :: University of Illinois/NCSA Open Source License
 License :: OSI Approved :: Vovida Software License 1.0
 License :: OSI Approved :: W3C License
 License :: OSI Approved :: X.Net License
+License :: OSI Approved :: Zero-Clause BSD (0BSD)
 License :: OSI Approved :: Zope Public License
 License :: OSI Approved :: zlib/libpng License
 License :: Other/Proprietary License
 License :: Public Domain
 License :: Repoze Public License
 Natural Language :: Afrikaans
 Natural Language :: Arabic
@@ -442,15 +454,17 @@
 Programming Language :: Emacs-Lisp
 Programming Language :: Erlang
 Programming Language :: Euler
 Programming Language :: Euphoria
 Programming Language :: F#
 Programming Language :: Forth
 Programming Language :: Fortran
+Programming Language :: Go
 Programming Language :: Haskell
+Programming Language :: Hy
 Programming Language :: Java
 Programming Language :: JavaScript
 Programming Language :: Kotlin
 Programming Language :: Lisp
 Programming Language :: Logo
 Programming Language :: Lua
 Programming Language :: ML
@@ -713,14 +727,17 @@
 Topic :: Software Development :: Build Tools
 Topic :: Software Development :: Code Generators
 Topic :: Software Development :: Compilers
 Topic :: Software Development :: Debuggers
 Topic :: Software Development :: Disassemblers
 Topic :: Software Development :: Documentation
 Topic :: Software Development :: Embedded Systems
+Topic :: Software Development :: Embedded Systems :: Controller Area Network (CAN)
+Topic :: Software Development :: Embedded Systems :: Controller Area Network (CAN) :: CANopen
+Topic :: Software Development :: Embedded Systems :: Controller Area Network (CAN) :: J1939
 Topic :: Software Development :: Internationalization
 Topic :: Software Development :: Interpreters
 Topic :: Software Development :: Libraries
 Topic :: Software Development :: Libraries :: Application Frameworks
 Topic :: Software Development :: Libraries :: Java Libraries
 Topic :: Software Development :: Libraries :: PHP Classes
 Topic :: Software Development :: Libraries :: Perl Modules
```

### Comparing `pypi-template-0.5.0/pypi_template/templates/base/index.md` & `pypi-template-0.6.0/pypi_template/templates/base/index.md`

 * *Files identical despite different names*

### Comparing `pypi-template-0.5.0/pypi_template/templates/docs/Makefile` & `pypi-template-0.6.0/pypi_template/templates/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pypi-template-0.5.0/pypi_template/templates/docs/conf.py` & `pypi-template-0.6.0/pypi_template/templates/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pypi-template-0.5.0/pypi_template/templates/docs/contributing.md` & `pypi-template-0.6.0/pypi_template/templates/docs/contributing.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Contributing
 
 This is Open Source software, so [given enough eyeballs, all bugs are shallow](https://en.wikipedia.org/wiki/Linus%27s_Law). Your contributions are more than welcome.
 
-This project is hosted on [GitHub](https://githhub.com/{{ github_account }}/{{ github_repo_name }}) and these (common) rules apply:
+This project is hosted on [GitHub](https://github.com/{{ github_account }}/{{ github_repo_name }}) and these (common) rules apply:
 
-* Do use the [issues tracker](https://githhub.com/{{ github_account }}/{{ github_repo_name }}/issues).
+* Do use the [issues tracker](https://github.com/{{ github_account }}/{{ github_repo_name }}/issues).
 * Let's discuss any proposed change or fix in an issue, so your work is not done in vain - I hate to reject pull requests...
-* Create [pull requests](https://githhub.com/{{ github_account }}/{{ github_repo_name }}/pulls) against `next` branch.
+* Create [pull requests](https://github.com/{{ github_account }}/{{ github_repo_name }}/pulls) against `next` branch.
 * Try to keep pull requests "atomic", and if possible related to an issue.
```

### Comparing `pypi-template-0.5.0/pypi_template/templates/docs/make.bat` & `pypi-template-0.6.0/pypi_template/templates/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pypi-template-0.5.0/pypi_template/templates/setup.py` & `pypi-template-0.6.0/pypi_template/templates/setup.py`

 * *Files identical despite different names*

### Comparing `pypi-template-0.5.0/pypi_template.egg-info/PKG-INFO` & `pypi-template-0.6.0/pypi_template.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-template
-Version: 0.5.0
+Version: 0.6.0
 Summary: Template-based common/best practices for managing a Python package on PyPi
 Home-page: https://github.com/christophevg/pypi-template
 Author: Christophe VG
 License: MIT
 Keywords: python pypi package management template
 Classifier: Environment :: Console
 Classifier: Development Status :: 4 - Beta
@@ -21,14 +21,16 @@
 License-File: LICENSE.txt
 Requires-Dist: jinja2
 Requires-Dist: pyyaml
 Requires-Dist: prompt-toolkit
 Requires-Dist: colorama
 Requires-Dist: fire
 Requires-Dist: importlib-resources
+Requires-Dist: requests
+Requires-Dist: packaging
 
 # PyPi Template
 
 > Template-based common/best practices for managing a Python package on PyPi
 
 [![Latest Version on PyPI](https://img.shields.io/pypi/v/pypi-template.svg)](https://pypi.python.org/pypi/pypi-template/)
 [![Supported Implementations](https://img.shields.io/pypi/pyversions/pypi-template.svg)](https://pypi.python.org/pypi/pypi-template/)
```

### Comparing `pypi-template-0.5.0/pypi_template.egg-info/SOURCES.txt` & `pypi-template-0.6.0/pypi_template.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,8 +41,9 @@
 pypi_template/templates/docs/index.md
 pypi_template/templates/docs/make.bat
 pypi_template/templates/docs/whats-in-the-box.md
 pypi_template/templates/docs/_static/.gitignore
 pypi_template/templates/docs/_static/__init__.py
 pypi_template/templates/tests/__init__.py
 pypi_template/templates/tests/test_example.py
-tests/test_example.py
+tests/test_example.py
+tests/test_values.py
```

### Comparing `pypi-template-0.5.0/setup.py` & `pypi-template-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 INSTALL_REQUIRES = [
   "jinja2",
   "pyyaml",
   "prompt-toolkit",
   "colorama",
   "fire",
   "importlib-resources",
+  "requests",
+  "packaging",
   
 ]
 ENTRY_POINTS = {
   "console_scripts" : [
     "pypi-template=pypi_template.__main__:cli",
     
   ]
```

