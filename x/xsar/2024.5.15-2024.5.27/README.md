# Comparing `tmp/xsar-2024.5.15.tar.gz` & `tmp/xsar-2024.5.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsar-2024.5.15.tar", last modified: Wed May 15 08:50:43 2024, max compression
+gzip compressed data, was "xsar-2024.5.27.tar", last modified: Mon May 27 14:35:31 2024, max compression
```

## Comparing `xsar-2024.5.15.tar` & `xsar-2024.5.27.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.616173 xsar-2024.5.15/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 08:50:32.000000 xsar-2024.5.15/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 08:50:32.000000 xsar-2024.5.15/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-15 08:50:32.000000 xsar-2024.5.15/.gitconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.608173 xsar-2024.5.15/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.608173 xsar-2024.5.15/.github/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-15 08:50:32.000000 xsar-2024.5.15/.github/actions/dynamic_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 08:50:32.000000 xsar-2024.5.15/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.608173 xsar-2024.5.15/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-15 08:50:32.000000 xsar-2024.5.15/.github/workflows/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-15 08:50:32.000000 xsar-2024.5.15/.github/workflows/conda-feedstock-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-15 08:50:32.000000 xsar-2024.5.15/.github/workflows/install-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-15 08:50:32.000000 xsar-2024.5.15/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-15 08:50:32.000000 xsar-2024.5.15/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-15 08:50:32.000000 xsar-2024.5.15/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 08:50:32.000000 xsar-2024.5.15/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 08:50:32.000000 xsar-2024.5.15/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 08:50:32.000000 xsar-2024.5.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 08:50:32.000000 xsar-2024.5.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-15 08:50:43.616173 xsar-2024.5.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-15 08:50:32.000000 xsar-2024.5.15/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-15 08:50:32.000000 xsar-2024.5.15/README_dev.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 08:50:32.000000 xsar-2024.5.15/condarc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.608173 xsar-2024.5.15/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.604173 xsar-2024.5.15/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.608173 xsar-2024.5.15/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/_static/css/xsar.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.608173 xsar-2024.5.15/docs/_static/uml/
--rw-r--r--   0 runner    (1001) docker     (127)   856119 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/_static/uml/classes_all_attributes.png
--rw-r--r--   0 runner    (1001) docker     (127)   126927 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/_static/uml/packages_all_attributes.png
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.612173 xsar-2024.5.15/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/mask.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/projections.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/radarsat2.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19403 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/rcm.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/xsar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16828 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/xsar_advanced.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   664426 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/xsar_batch_datarmor.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/xsar_multiple.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/xsar_tops_slc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/uml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 08:50:32.000000 xsar-2024.5.15/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.612173 xsar-2024.5.15/highlevel-checks/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-15 08:50:32.000000 xsar-2024.5.15/highlevel-checks/check_s1_xsar_opendataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-15 08:50:32.000000 xsar-2024.5.15/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-15 08:50:32.000000 xsar-2024.5.15/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:50:43.616173 xsar-2024.5.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-15 08:50:32.000000 xsar-2024.5.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.604173 xsar-2024.5.15/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.612173 xsar-2024.5.15/src/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4082 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/scripts/compress_safe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.616173 xsar-2024.5.15/src/xsar/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37154 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/base_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/ipython_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)    32278 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/radarsat2_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12462 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/radarsat2_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/raster_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    34783 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/rcm_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15175 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/rcm_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    72519 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/sentinel1_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/sentinel1_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    26102 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/xarray_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/xsar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.616173 xsar-2024.5.15/src/xsar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-15 08:50:43.000000 xsar-2024.5.15/src/xsar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-15 08:50:43.000000 xsar-2024.5.15/src/xsar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:50:43.000000 xsar-2024.5.15/src/xsar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 08:50:43.000000 xsar-2024.5.15/src/xsar.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 08:50:43.000000 xsar-2024.5.15/src/xsar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 08:50:43.000000 xsar-2024.5.15/src/xsar.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.616173 xsar-2024.5.15/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-15 08:50:32.000000 xsar-2024.5.15/test/test_raster_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.887566 xsar-2024.5.27/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 14:35:22.000000 xsar-2024.5.27/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-27 14:35:22.000000 xsar-2024.5.27/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-27 14:35:22.000000 xsar-2024.5.27/.gitconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.875566 xsar-2024.5.27/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.875566 xsar-2024.5.27/.github/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-27 14:35:22.000000 xsar-2024.5.27/.github/actions/dynamic_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-27 14:35:22.000000 xsar-2024.5.27/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.875566 xsar-2024.5.27/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-27 14:35:22.000000 xsar-2024.5.27/.github/workflows/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-27 14:35:22.000000 xsar-2024.5.27/.github/workflows/conda-feedstock-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-27 14:35:22.000000 xsar-2024.5.27/.github/workflows/install-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-27 14:35:22.000000 xsar-2024.5.27/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-27 14:35:22.000000 xsar-2024.5.27/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-27 14:35:22.000000 xsar-2024.5.27/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 14:35:22.000000 xsar-2024.5.27/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-27 14:35:22.000000 xsar-2024.5.27/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-27 14:35:22.000000 xsar-2024.5.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 14:35:22.000000 xsar-2024.5.27/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-27 14:35:31.883566 xsar-2024.5.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-27 14:35:22.000000 xsar-2024.5.27/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-27 14:35:22.000000 xsar-2024.5.27/README_dev.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 14:35:22.000000 xsar-2024.5.27/condarc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.875566 xsar-2024.5.27/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.871566 xsar-2024.5.27/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.875566 xsar-2024.5.27/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/_static/css/xsar.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.879566 xsar-2024.5.27/docs/_static/uml/
+-rw-r--r--   0 runner    (1001) docker     (127)   856119 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/_static/uml/classes_all_attributes.png
+-rw-r--r--   0 runner    (1001) docker     (127)   126927 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/_static/uml/packages_all_attributes.png
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.879566 xsar-2024.5.27/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/examples/mask.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/examples/projections.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/examples/radarsat2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19403 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/examples/rcm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/examples/xsar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16828 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/examples/xsar_advanced.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   664426 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/examples/xsar_batch_datarmor.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/examples/xsar_multiple.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/examples/xsar_tops_slc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-27 14:35:22.000000 xsar-2024.5.27/docs/uml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-27 14:35:22.000000 xsar-2024.5.27/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.879566 xsar-2024.5.27/highlevel-checks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-27 14:35:22.000000 xsar-2024.5.27/highlevel-checks/check_s1_xsar_opendataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-27 14:35:22.000000 xsar-2024.5.27/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 14:35:22.000000 xsar-2024.5.27/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:35:31.887566 xsar-2024.5.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-27 14:35:22.000000 xsar-2024.5.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.871566 xsar-2024.5.27/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.879566 xsar-2024.5.27/src/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4082 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/scripts/compress_safe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.883566 xsar-2024.5.27/src/xsar/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37154 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/base_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/ipython_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32278 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/radarsat2_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12462 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/radarsat2_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/raster_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34783 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/rcm_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15175 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/rcm_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72449 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/sentinel1_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/sentinel1_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26102 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/xarray_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-27 14:35:22.000000 xsar-2024.5.27/src/xsar/xsar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.883566 xsar-2024.5.27/src/xsar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-27 14:35:31.000000 xsar-2024.5.27/src/xsar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-27 14:35:31.000000 xsar-2024.5.27/src/xsar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:35:31.000000 xsar-2024.5.27/src/xsar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-27 14:35:31.000000 xsar-2024.5.27/src/xsar.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-27 14:35:31.000000 xsar-2024.5.27/src/xsar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 14:35:31.000000 xsar-2024.5.27/src/xsar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:35:31.883566 xsar-2024.5.27/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-27 14:35:22.000000 xsar-2024.5.27/test/test_raster_readers.py
```

### Comparing `xsar-2024.5.15/.github/actions/dynamic_matrix.py` & `xsar-2024.5.27/.github/actions/dynamic_matrix.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/.github/workflows/README.md` & `xsar-2024.5.27/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/.github/workflows/conda-feedstock-check.yml` & `xsar-2024.5.27/.github/workflows/conda-feedstock-check.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/.github/workflows/install-test.yml` & `xsar-2024.5.27/.github/workflows/install-test.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/.github/workflows/publish.yml` & `xsar-2024.5.27/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/.gitignore` & `xsar-2024.5.27/.gitignore`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/.gitlab-ci.yml` & `xsar-2024.5.27/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/Dockerfile` & `xsar-2024.5.27/Dockerfile`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/LICENSE` & `xsar-2024.5.27/LICENSE`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/PKG-INFO` & `xsar-2024.5.27/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsar
-Version: 2024.5.15
+Version: 2024.5.27
 Summary: xarray L1 SAR mapper
 Home-page: https://github.com/umr-lops/xsar
 Author: Olivier Archer, Alexandre Levieux, Antoine Grouazel
 Author-email: Olivier.Archer@ifremer.fr, Alexandre.Levieux@gmail.com, Antoine.Grouazel@ifremer.fr
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `xsar-2024.5.15/README.md` & `xsar-2024.5.27/README.md`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/README_dev.md` & `xsar-2024.5.27/README_dev.md`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/Makefile` & `xsar-2024.5.27/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/_static/uml/classes_all_attributes.png` & `xsar-2024.5.27/docs/_static/uml/classes_all_attributes.png`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/_static/uml/packages_all_attributes.png` & `xsar-2024.5.27/docs/_static/uml/packages_all_attributes.png`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/basic_api.rst` & `xsar-2024.5.27/docs/basic_api.rst`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/conf.py` & `xsar-2024.5.27/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/examples/mask.ipynb` & `xsar-2024.5.27/docs/examples/mask.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/examples/projections.ipynb` & `xsar-2024.5.27/docs/examples/projections.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/examples/radarsat2.ipynb` & `xsar-2024.5.27/docs/examples/radarsat2.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/examples/rcm.ipynb` & `xsar-2024.5.27/docs/examples/rcm.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/examples/xsar.ipynb` & `xsar-2024.5.27/docs/examples/xsar.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/examples/xsar_advanced.ipynb` & `xsar-2024.5.27/docs/examples/xsar_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/examples/xsar_batch_datarmor.ipynb` & `xsar-2024.5.27/docs/examples/xsar_batch_datarmor.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/examples/xsar_multiple.ipynb` & `xsar-2024.5.27/docs/examples/xsar_multiple.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/examples/xsar_tops_slc.ipynb` & `xsar-2024.5.27/docs/examples/xsar_tops_slc.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/index.rst` & `xsar-2024.5.27/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/docs/installing.rst` & `xsar-2024.5.27/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/highlevel-checks/check_s1_xsar_opendataset.py` & `xsar-2024.5.27/highlevel-checks/check_s1_xsar_opendataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/setup.py` & `xsar-2024.5.27/setup.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/scripts/compress_safe.py` & `xsar-2024.5.27/src/scripts/compress_safe.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/base_dataset.py` & `xsar-2024.5.27/src/xsar/base_dataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/base_meta.py` & `xsar-2024.5.27/src/xsar/base_meta.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/config.yml` & `xsar-2024.5.27/src/xsar/config.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/ipython_backends.py` & `xsar-2024.5.27/src/xsar/ipython_backends.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/radarsat2_dataset.py` & `xsar-2024.5.27/src/xsar/radarsat2_dataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/radarsat2_meta.py` & `xsar-2024.5.27/src/xsar/radarsat2_meta.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/raster_readers.py` & `xsar-2024.5.27/src/xsar/raster_readers.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/rcm_dataset.py` & `xsar-2024.5.27/src/xsar/rcm_dataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/rcm_meta.py` & `xsar-2024.5.27/src/xsar/rcm_meta.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/sentinel1_dataset.py` & `xsar-2024.5.27/src/xsar/sentinel1_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,30 +163,28 @@
 
         # calibration LUTs
         ds_luts = self.sar_meta.get_calibration_luts
         ds_luts.attrs['history'] = 'calibration'
 
         # noise levels LUTs
         ds_noise_range = self.sar_meta.get_noise_range_raw
-        ds_noise_range.attrs['history'] = 'noise'
         ds_noise_azi = self.sar_meta.get_noise_azi_raw
 
         # antenna pattern
         ds_antenna_pattern = self.sar_meta.get_antenna_pattern
 
         # swath merging
         ds_swath_merging = self.sar_meta.get_swath_merging
 
         if self.sar_meta.swath == 'WV':
             # since WV noise is not defined on azimuth we apply the patch on range noise
             # ds_noise_azi['noise_lut'] = self._patch_lut(ds_noise_azi[
             #                                                 'noise_lut'])  # patch applied here is distinct to same patch applied on interpolated noise LUT
             ds_noise_range['noise_lut'] = self._patch_lut(ds_noise_range[
                 'noise_lut'])  # patch applied here is distinct to same patch applied on interpolated noise LUT
-        ds_noise_azi.attrs['history'] = 'noise'
 
         self.datatree = datatree.DataTree.from_dict({'measurement': DN_tmp, 'geolocation_annotation': geoloc,
                                                      'bursts': bu, 'FMrate': FM, 'doppler_estimate': dop,
                                                      # 'image_information':
                                                      'orbit': self.sar_meta.orbit,
                                                      'image': self.sar_meta.image,
                                                      'calibration': ds_luts,
@@ -290,17 +288,18 @@
         self._dataset.attrs.update(self.sar_meta.to_dict("all"))
         self.datatree['measurement'] = self.datatree['measurement'].assign(
             self._dataset)
         self.datatree.attrs.update(self.sar_meta.to_dict("all"))
 
         # load land_mask by default for GRD products
 
-        self.add_high_resolution_variables(
-            patch_variable=patch_variable, luts=luts, lazy_loading=lazyloading)
+
         if 'GRD' in str(self.datatree.attrs['product']):
+            self.add_high_resolution_variables(
+                                   patch_variable=patch_variable, luts=luts, lazy_loading=lazyloading)
             if self.apply_recalibration:
                 self.select_gains()
             self.apply_calibration_and_denoising()
 
         # added 6 fev 23, to fill  empty attrs
         self.datatree['measurement'].attrs = self.datatree.attrs
         if self.sar_meta.product == 'SLC' and 'WV' not in self.sar_meta.swath:  # TOPS cases
```

### Comparing `xsar-2024.5.15/src/xsar/sentinel1_meta.py` & `xsar-2024.5.27/src/xsar/sentinel1_meta.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/utils.py` & `xsar-2024.5.27/src/xsar/utils.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/xarray_backends.py` & `xsar-2024.5.27/src/xsar/xarray_backends.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar/xsar.py` & `xsar-2024.5.27/src/xsar/xsar.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/src/xsar.egg-info/PKG-INFO` & `xsar-2024.5.27/src/xsar.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsar
-Version: 2024.5.15
+Version: 2024.5.27
 Summary: xarray L1 SAR mapper
 Home-page: https://github.com/umr-lops/xsar
 Author: Olivier Archer, Alexandre Levieux, Antoine Grouazel
 Author-email: Olivier.Archer@ifremer.fr, Alexandre.Levieux@gmail.com, Antoine.Grouazel@ifremer.fr
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `xsar-2024.5.15/src/xsar.egg-info/SOURCES.txt` & `xsar-2024.5.27/src/xsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xsar-2024.5.15/test/test_raster_readers.py` & `xsar-2024.5.27/test/test_raster_readers.py`

 * *Files identical despite different names*

