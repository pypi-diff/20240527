# Comparing `tmp/vascpy-0.1.1.tar.gz` & `tmp/vascpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vascpy-0.1.1.tar", last modified: Thu Apr  7 16:44:09 2022, max compression
+gzip compressed data, was "vascpy-0.1.2.tar", last modified: Mon May 27 07:34:38 2024, max compression
```

## Comparing `vascpy-0.1.1.tar` & `vascpy-0.1.2.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.770861 vascpy-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.762861 vascpy-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.762861 vascpy-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-04-07 16:44:04.000000 vascpy-0.1.1/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-04-07 16:44:04.000000 vascpy-0.1.1/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-04-07 16:44:04.000000 vascpy-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-04-07 16:44:04.000000 vascpy-0.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-07 16:44:04.000000 vascpy-0.1.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4470 2022-04-07 16:44:04.000000 vascpy-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-04-07 16:44:04.000000 vascpy-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-04-07 16:44:04.000000 vascpy-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-04-07 16:44:09.770861 vascpy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2892 2022-04-07 16:44:04.000000 vascpy-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.762861 vascpy-0.1.1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-04-07 16:44:04.000000 vascpy-0.1.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.762861 vascpy-0.1.1/doc/source/
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-04-07 16:44:04.000000 vascpy-0.1.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-04-07 16:44:04.000000 vascpy-0.1.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2661 2022-04-07 16:44:04.000000 vascpy-0.1.1/doc/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.762861 vascpy-0.1.1/doc/source/logo/
--rw-r--r--   0 runner    (1001) docker     (121)  1592874 2022-04-07 16:44:04.000000 vascpy-0.1.1/doc/source/logo/BBP-vascpy.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-04-07 16:44:04.000000 vascpy-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-07 16:44:09.770861 vascpy-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-04-07 16:44:04.000000 vascpy-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.766861 vascpy-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.766861 vascpy-0.1.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)    18138 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/capillary_with_loops_point_connectivity.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.766861 vascpy-0.1.1/tests/data/h5/
--rw-r--r--   0 runner    (1001) docker     (121)     7328 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/h5/capillary_with_loops.h5
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/h5/fork_diameters_point_spec.h5
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/h5/fork_diameters_section_spec.h5
--rw-r--r--   0 runner    (1001) docker     (121)    10584 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/h5/fork_diameters_sonata_spec.h5
--rw-r--r--   0 runner    (1001) docker     (121)     6928 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/h5/fork_multiple_properties.h5
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.766861 vascpy-0.1.1/tests/data/vtk/
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/vtk/fork_diameters_point_spec.vtk
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/vtk/fork_edge_radii_edges_field_data.vtk
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/vtk/fork_multiple_properties.vtk
--rw-r--r--   0 runner    (1001) docker     (121)     8304 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/vtk/one_loop(1).h5
--rw-r--r--   0 runner    (1001) docker     (121)     7381 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/vtk/one_loop.vtk
--rwxr-xr-x   0 runner    (1001) docker     (121)    55364 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/vtk/penetrating_artery.vtk
--rwxr-xr-x   0 runner    (1001) docker     (121)    34828 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/vtk/penetrating_artery2.vtk
--rw-r--r--   0 runner    (1001) docker     (121)    61536 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/vtk/penetrating_artery_diameters_on_points.vtk
--rw-r--r--   0 runner    (1001) docker     (121)    42832 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/vtk/penetrating_artery_diameters_on_points_sections.h5
--rwxr-xr-x   0 runner    (1001) docker     (121)    55364 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/vtk/penetrating_artery_radii_on_edges.vtk
--rw-r--r--   0 runner    (1001) docker     (121)    61536 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/vtk/penetrating_artery_standardized.vtk
--rwxr-xr-x   0 runner    (1001) docker     (121)    25444 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/data/vtk/test_smaller_vasculature.vtk
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.766861 vascpy-0.1.1/tests/point_graph/
--rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/point_graph/test_curation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/point_graph/test_features.py
--rw-r--r--   0 runner    (1001) docker     (121)    14173 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/point_graph/test_point_data_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     5127 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/test_adjacency.py
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    15436 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)    21597 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/test_point_vasculature.py
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/test_representation_conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/test_section_annotation.py
--rw-r--r--   0 runner    (1001) docker     (121)    16481 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/test_section_creation.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/test_section_vasculature.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-04-07 16:44:04.000000 vascpy-0.1.1/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-04-07 16:44:04.000000 vascpy-0.1.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.770861 vascpy-0.1.1/vascpy/
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     8078 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/conversion.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.770861 vascpy-0.1.1/vascpy/point_graph/
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/point_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2173 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/point_graph/curation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/point_graph/features.py
--rw-r--r--   0 runner    (1001) docker     (121)    10556 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/point_graph/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    11713 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/point_vasculature.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.770861 vascpy-0.1.1/vascpy/section_graph/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/section_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/section_graph/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/section_vasculature.py
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.770861 vascpy-0.1.1/vascpy/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7054 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/utils/adjacency.py
--rw-r--r--   0 runner    (1001) docker     (121)     4393 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     9291 2022-04-07 16:44:04.000000 vascpy-0.1.1/vascpy/utils/section_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 16:44:09.770861 vascpy-0.1.1/vascpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-04-07 16:44:09.000000 vascpy-0.1.1/vascpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-04-07 16:44:09.000000 vascpy-0.1.1/vascpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-07 16:44:09.000000 vascpy-0.1.1/vascpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-04-07 16:44:09.000000 vascpy-0.1.1/vascpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-04-07 16:44:09.000000 vascpy-0.1.1/vascpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-07 16:44:09.000000 vascpy-0.1.1/vascpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.598937 vascpy-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.582937 vascpy-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.586937 vascpy-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-27 07:34:31.000000 vascpy-0.1.2/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-27 07:34:31.000000 vascpy-0.1.2/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-27 07:34:31.000000 vascpy-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-27 07:34:31.000000 vascpy-0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:34:31.000000 vascpy-0.1.2/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-27 07:34:31.000000 vascpy-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-27 07:34:31.000000 vascpy-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 07:34:31.000000 vascpy-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-27 07:34:38.598937 vascpy-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-27 07:34:31.000000 vascpy-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.586937 vascpy-0.1.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-27 07:34:31.000000 vascpy-0.1.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.586937 vascpy-0.1.2/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-27 07:34:31.000000 vascpy-0.1.2/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-27 07:34:31.000000 vascpy-0.1.2/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-27 07:34:31.000000 vascpy-0.1.2/doc/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.586937 vascpy-0.1.2/doc/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)  1592874 2024-05-27 07:34:31.000000 vascpy-0.1.2/doc/source/logo/BBP-vascpy.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-27 07:34:31.000000 vascpy-0.1.2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-27 07:34:31.000000 vascpy-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:34:38.598937 vascpy-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-27 07:34:31.000000 vascpy-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.590937 vascpy-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.590937 vascpy-0.1.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    18138 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/capillary_with_loops_point_connectivity.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.590937 vascpy-0.1.2/tests/data/h5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/h5/capillary_with_loops.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/h5/fork_diameters_point_spec.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/h5/fork_diameters_section_spec.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/h5/fork_diameters_sonata_spec.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/h5/fork_multiple_properties.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.594937 vascpy-0.1.2/tests/data/vtk/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/vtk/fork_diameters_point_spec.vtk
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/vtk/fork_edge_radii_edges_field_data.vtk
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/vtk/fork_multiple_properties.vtk
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/vtk/one_loop(1).h5
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/vtk/one_loop.vtk
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55364 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/vtk/penetrating_artery.vtk
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34828 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/vtk/penetrating_artery2.vtk
+-rw-r--r--   0 runner    (1001) docker     (127)    61536 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/vtk/penetrating_artery_diameters_on_points.vtk
+-rw-r--r--   0 runner    (1001) docker     (127)    42832 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/vtk/penetrating_artery_diameters_on_points_sections.h5
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55364 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/vtk/penetrating_artery_radii_on_edges.vtk
+-rw-r--r--   0 runner    (1001) docker     (127)    61536 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/vtk/penetrating_artery_standardized.vtk
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25444 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/data/vtk/test_smaller_vasculature.vtk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.594937 vascpy-0.1.2/tests/point_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/point_graph/test_curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/point_graph/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/point_graph/test_point_data_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/test_adjacency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15436 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21597 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/test_point_vasculature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/test_representation_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/test_section_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/test_section_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/test_section_vasculature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-27 07:34:31.000000 vascpy-0.1.2/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-27 07:34:31.000000 vascpy-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.594937 vascpy-0.1.2/vascpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.594937 vascpy-0.1.2/vascpy/point_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/point_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/point_graph/curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/point_graph/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/point_graph/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/point_vasculature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.594937 vascpy-0.1.2/vascpy/section_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/section_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/section_graph/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/section_vasculature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.598937 vascpy-0.1.2/vascpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/utils/adjacency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-05-27 07:34:31.000000 vascpy-0.1.2/vascpy/utils/section_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:34:38.594937 vascpy-0.1.2/vascpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-27 07:34:38.000000 vascpy-0.1.2/vascpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-27 07:34:38.000000 vascpy-0.1.2/vascpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:34:38.000000 vascpy-0.1.2/vascpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 07:34:38.000000 vascpy-0.1.2/vascpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-27 07:34:38.000000 vascpy-0.1.2/vascpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 07:34:38.000000 vascpy-0.1.2/vascpy.egg-info/top_level.txt
```

### Comparing `vascpy-0.1.1/.github/workflows/publish-sdist.yml` & `vascpy-0.1.2/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/.github/workflows/run-tox.yml` & `vascpy-0.1.2/.github/workflows/run-tox.yml`

 * *Files 14% similar despite different names*

```diff
@@ -7,29 +7,29 @@
         - main
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
         pip install tox-gh-actions
     - name: Run tox
       run: |
         tox
     - name: Upload to codecov
-      if: ${{matrix.python-version == '3.9'}}
-      uses: codecov/codecov-action@v1
+      uses: codecov/codecov-action@v4
       with:
         fail_ci_if_error: false
         files: ./coverage.xml
         flags: pytest
-        name: "vascpy-py39"
+        name: "vascpy-py${{ matrix.python-version }}"
+        token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `vascpy-0.1.1/.gitignore` & `vascpy-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/.readthedocs.yml` & `vascpy-0.1.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/CONTRIBUTING.md` & `vascpy-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/LICENSE.txt` & `vascpy-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/PKG-INFO` & `vascpy-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: vascpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Vasculature API
 Home-page: https://github.com/BlueBrain/vascpy
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Project-URL: Tracker, https://github.com/BlueBrain/vascpy/issues
 Project-URL: Source, https://github.com/BlueBrain/vascpy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Provides-Extra: convert-vtk
 Provides-Extra: all
 Provides-Extra: docs
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
```

### Comparing `vascpy-0.1.1/README.md` & `vascpy-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 -----
 
 Load and write an h5 morphology file:
 
 ```python
 from vascpy import SectionVasculature
 
-v = SectionVasculature.load_hdf5("sample.h5")
+v = SectionVasculature.load("sample.h5")
 
 print(v.points)
 print(v.diameters)
 print(v.connectivity)
 print(v.sections)
 
-v.save_hdf5("sample2.h5")
+v.save("sample2.h5")
 ```
 
 Load and write an h5 SONATA file:
 ```python
 from vascpy import PointVasculature
 
 v = PointVasculature.load_sonata("sample_sonata.h5")
@@ -79,19 +79,19 @@
     'z': np.array([6., 7., 8.]),
     'diameter': np.array([0.1, 0.2, 0.3])
 })
 
 edge_properties = pd.DataFrame({
     'start_node': np.array([0, 0, 1]),
     'end_node': np.array([1, 2, 2]),
-    'type': np.array([0, 1, 1])
+    'type': np.array([1, 1, 1])
 })
 
 v = PointVasculature(node_properties=node_properties, edge_properties=edge_properties)
 v.save_sonata('my_vasculature.h5')
 ```
 Funding & Acknowledgements
 -------------------------
 
 The development of this software was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government's ETH Board of the Swiss Federal Institutes of Technology.
 
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2024 Blue Brain Project/EPFL
```

### Comparing `vascpy-0.1.1/doc/Makefile` & `vascpy-0.1.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/doc/source/conf.py` & `vascpy-0.1.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/doc/source/index.rst` & `vascpy-0.1.2/doc/source/index.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..
-    Copyright (c) 2022 Blue Brain Project/EPFL
+    Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/doc/source/installation.rst` & `vascpy-0.1.2/doc/source/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..
-    Copyright (c) 2022 Blue Brain Project/EPFL
+    Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/doc/source/logo/BBP-vascpy.jpg` & `vascpy-0.1.2/doc/source/logo/BBP-vascpy.jpg`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/setup.py` & `vascpy-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -21,14 +21,15 @@
 
 setup(
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     name="vascpy",
     description="Vasculature API",
     author="Blue Brain Project, EPFL",
     license="Apache-2",
     url="https://github.com/BlueBrain/vascpy",
     project_urls={
@@ -40,19 +41,19 @@
     install_requires=[
         "numpy>=1.17",
         "scipy>=1.0.0",
         "h5py>=3.4.0",
         "pandas>=1.0.0",
         "morphio>=3.0.0",
         "libsonata>=0.1.8",
-        "click>=8.0",
+        "click>=8.0",  # 8.0 required for isolated_filesystem
     ],
     extras_require={
         "convert-vtk": DEPS_VTK,
-        "all": DEPS_VTK + ["python-igraph>=0.8.0"],
+        "all": DEPS_VTK + ["igraph>=0.8.0"],
         "docs": ["sphinx", "sphinx-bluebrain-theme"],
     },
     packages=find_packages(),
     entry_points={"console_scripts": ["vascpy = vascpy.cli:app"]},
     include_package_data=True,
     python_requires=">=3.7",
 )
```

### Comparing `vascpy-0.1.1/tests/data/capillary_with_loops_point_connectivity.json` & `vascpy-0.1.2/tests/data/capillary_with_loops_point_connectivity.json`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/h5/capillary_with_loops.h5` & `vascpy-0.1.2/tests/data/h5/capillary_with_loops.h5`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/h5/fork_diameters_point_spec.h5` & `vascpy-0.1.2/tests/data/h5/fork_diameters_point_spec.h5`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/h5/fork_diameters_section_spec.h5` & `vascpy-0.1.2/tests/data/h5/fork_diameters_section_spec.h5`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/h5/fork_diameters_sonata_spec.h5` & `vascpy-0.1.2/tests/data/h5/fork_diameters_sonata_spec.h5`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/h5/fork_multiple_properties.h5` & `vascpy-0.1.2/tests/data/h5/fork_multiple_properties.h5`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/vtk/fork_multiple_properties.vtk` & `vascpy-0.1.2/tests/data/vtk/fork_multiple_properties.vtk`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/vtk/one_loop(1).h5` & `vascpy-0.1.2/tests/data/vtk/one_loop(1).h5`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/vtk/one_loop.vtk` & `vascpy-0.1.2/tests/data/vtk/one_loop.vtk`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/vtk/penetrating_artery.vtk` & `vascpy-0.1.2/tests/data/vtk/penetrating_artery.vtk`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/vtk/penetrating_artery2.vtk` & `vascpy-0.1.2/tests/data/vtk/penetrating_artery2.vtk`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/vtk/penetrating_artery_diameters_on_points.vtk` & `vascpy-0.1.2/tests/data/vtk/penetrating_artery_diameters_on_points.vtk`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/vtk/penetrating_artery_diameters_on_points_sections.h5` & `vascpy-0.1.2/tests/data/vtk/penetrating_artery_diameters_on_points_sections.h5`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/vtk/penetrating_artery_radii_on_edges.vtk` & `vascpy-0.1.2/tests/data/vtk/penetrating_artery_radii_on_edges.vtk`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/vtk/penetrating_artery_standardized.vtk` & `vascpy-0.1.2/tests/data/vtk/penetrating_artery_standardized.vtk`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/data/vtk/test_smaller_vasculature.vtk` & `vascpy-0.1.2/tests/data/vtk/test_smaller_vasculature.vtk`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/point_graph/test_curation.py` & `vascpy-0.1.2/tests/point_graph/test_curation.py`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/point_graph/test_features.py` & `vascpy-0.1.2/tests/point_graph/test_features.py`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/point_graph/test_point_data_io.py` & `vascpy-0.1.2/tests/point_graph/test_point_data_io.py`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/test_adjacency.py` & `vascpy-0.1.2/tests/test_adjacency.py`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/test_cli.py` & `vascpy-0.1.2/tests/test_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,53 @@
 import tempfile
 from pathlib import Path
 
 import click
+import libsonata
 import numpy as np
 import pytest
 from click.testing import CliRunner
 from numpy import testing as npt
 from pandas import testing as pdt
 
 from vascpy import PointVasculature, SectionVasculature
 from vascpy.cli import app
 
 DATA = Path(__file__).parent / "data"
 
-"""
-def test_version():
 
-    from vascpy.version import VERSION
+def test_convert__morphology_to_sonata_population_name():
+
+    morphology_file = str(DATA / "h5/fork_diameters_section_spec.h5")
 
     runner = CliRunner()
 
-    result = runner.invoke(app, "--version")
+    with tempfile.TemporaryDirectory() as temp_dir:
+
+        out_sonata_file = str(Path(temp_dir) / "sonata.h5")
+
+        with runner.isolated_filesystem(temp_dir=temp_dir):
 
-    assert result.exit_code == 0
-    assert result.output == f"vascpy, version {VERSION}\n"
-"""
+            result = runner.invoke(
+                app,
+                [
+                    "morphology-to-sonata",
+                    "--population-name",
+                    "mypopulation",
+                    morphology_file,
+                    out_sonata_file,
+                ],
+            )
+
+            assert result.exit_code == 0, result
+            assert Path(out_sonata_file).exists()
+            assert libsonata.NodeStorage(out_sonata_file).population_names == {"mypopulation"}
 
 
-def test_convert__sonata_morphology():
+def test_convert__sonata_morphology_cycle():
 
     morphology_file = str(DATA / "h5/fork_diameters_section_spec.h5")
     sonata_file = str(DATA / "h5/fork_diameters_sonata_spec.h5")
 
     runner = CliRunner()
 
     with tempfile.TemporaryDirectory() as temp_dir:
```

### Comparing `vascpy-0.1.1/tests/test_conversion.py` & `vascpy-0.1.2/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/test_geometry.py` & `vascpy-0.1.2/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/test_point_vasculature.py` & `vascpy-0.1.2/tests/test_point_vasculature.py`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/test_representation_conversions.py` & `vascpy-0.1.2/tests/test_representation_conversions.py`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/test_section_annotation.py` & `vascpy-0.1.2/tests/test_section_annotation.py`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/test_section_creation.py` & `vascpy-0.1.2/tests/test_section_creation.py`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tests/utils.py` & `vascpy-0.1.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `vascpy-0.1.1/tox.ini` & `vascpy-0.1.2/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,64 @@
 [base]
 name = vascpy
 testdeps =
-    mock
     pytest
+    pytest-cov
 
 [tox]
 minversion = 3.1.0
 envlist =
-    py{38,39}
-    py39-lint
-    py39-coverage
+    py{38,39,310,311,312}
+    docs
+    lint
+    format
 ignore_basepython_conflict = true
 
 [testenv]
 extras = all
 deps = {[base]testdeps}
-commands = py.test {posargs}  tests
+commands = pytest \
+    --cov={envsitepackagesdir}/{[base]name} \
+    --cov-report term-missing \
+    --cov-fail-under=100 \
+    --cov-report=xml \
+    --no-cov-on-fail \
+    --cov-fail-under=95 \
+    {posargs}
 
 [testenv:format]
 deps =
     black==22.3.0
     isort
 commands =
     isort -l 100 --profile black {[base]name} tests setup.py
     black -l 100 {[base]name} tests setup.py
 
-[testenv:py39-lint]
+[testenv:lint]
 deps =
     mypy
     isort
     black==22.3.0
     pycodestyle
     pylint
     click
 commands =
     isort -l 100 --profile black --check-only --diff {[base]name} tests setup.py
     black -l 100 --check {[base]name} tests setup.py
     mypy --ignore-missing-imports {[base]name}
     pycodestyle {[base]name}
     pylint -j2 --ignored-modules=vtk {[base]name}
 
-[testenv:py39-coverage]
-deps =
-    {[base]testdeps}
-    pytest-cov
-commands =
-    pytest \
-    --cov-report term-missing \
-    --cov-report xml \
-    --cov-report html \
-    --cov={envsitepackagesdir}/{[base]name} \
-    tests/
-
-[testenv:py39-docs]
+[testenv:docs]
 changedir = doc
 extras = docs
 commands =
     make clean
     make html SPHINXOPTS=-W
-whitelist_externals =
+allowlist_externals =
     make
     rm
 
 # E203 whitespace before :, see
 # https://github.com/psf/black/issues/315
 # E731: do not assign a lambda expression, use a def
 # W503 line break before binary operator
@@ -70,11 +66,12 @@
 [pycodestyle]
 exclude = extras, workflow, tests
 ignore = E203, E731, W503
 max-line-length = 100
 
 [gh-actions]
 python =
-    3.7 : py37
-    3.8 : py38
+    3.8 : py38, lint
     3.9 : py39
     3.10: py310
+    3.11: py311, docs
+    3.12: py312
```

### Comparing `vascpy-0.1.1/vascpy/__init__.py` & `vascpy-0.1.2/vascpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/vascpy/cli.py` & `vascpy-0.1.2/vascpy/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -43,17 +43,24 @@
     )
     L.setLevel(level)
 
 
 @app.command()
 @click.argument("input-file", type=FILE_TYPE)
 @click.argument("output-file", type=str)
-def morphology_to_sonata(input_file, output_file):
+@click.option(
+    "--population-name",
+    type=str,
+    required=False,
+    default="vasculature",
+    help="The name of the node population.",
+)
+def morphology_to_sonata(input_file, output_file, population_name):
     """Converts a section graph morphology to a sonata node population"""
-    SectionVasculature.load(input_file).as_point_graph().save_sonata(output_file)
+    SectionVasculature.load(input_file).as_point_graph().save_sonata(output_file, population_name)
 
 
 @app.command()
 @click.argument("input-file", type=FILE_TYPE)
 @click.argument("output-file", type=str)
 def sonata_to_morphology(input_file, output_file):
     """Convert sonata file to morphology geometry file"""
```

### Comparing `vascpy-0.1.1/vascpy/conversion.py` & `vascpy-0.1.2/vascpy/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/vascpy/point_graph/__init__.py` & `vascpy-0.1.2/vascpy/point_graph/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """"
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/vascpy/point_graph/curation.py` & `vascpy-0.1.2/vascpy/point_graph/curation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/vascpy/point_graph/features.py` & `vascpy-0.1.2/vascpy/point_graph/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/vascpy/point_graph/io.py` & `vascpy-0.1.2/vascpy/point_graph/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -80,15 +80,20 @@
 
         return (
             pd.DataFrame(node_properties_dict, index=pd.RangeIndex(0, uids.size, dtype=np.int64)),
             pd.DataFrame(edge_properties_dict, index=pd.RangeIndex(0, pop.size, dtype=np.int64)),
         )
 
     @staticmethod
-    def write(filepath: str, node_properties: pd.DataFrame, edge_properties: pd.DataFrame):
+    def write(
+        filepath: str,
+        population_name: str,
+        node_properties: pd.DataFrame,
+        edge_properties: pd.DataFrame,
+    ):
         """Write an hdf5 file using the SONATA specification"""
         import h5py
 
         SPEC = specs.SpecSONATA
 
         n_edges = len(edge_properties)
         beg_ids = edge_properties.loc[:, "start_node"]
@@ -102,15 +107,15 @@
         for name, dtype in SPEC.SONATA_POINT_DTYPES.items():
             column_location = node_properties.columns.get_loc(name)
             props[f"start_{name}"] = node_properties.iloc[beg_ids, column_location].astype(dtype)
             props[f"end_{name}"] = node_properties.iloc[end_ids, column_location].astype(dtype)
 
         with h5py.File(filepath, "w") as h5f:
 
-            population = h5f.create_group("/nodes/vasculature", track_order=True)
+            population = h5f.create_group(f"/nodes/{population_name}", track_order=True)
             population.create_dataset("node_type_id", data=np.full(n_edges, -1), dtype=np.int64)
 
             group = population.create_group("0")
             group.create_dataset(
                 "@library/model_type",
                 data=["vasculature"],
                 dtype=h5py.special_dtype(vlen=str),
```

### Comparing `vascpy-0.1.1/vascpy/point_vasculature.py` & `vascpy-0.1.2/vascpy/point_vasculature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -243,17 +243,17 @@
             raise VasculatureAPIError(f"{filepath} extension is unknown.")
 
     @classmethod
     def load_sonata(cls, filepath):
         """Load a SONATA file"""
         return cls(*io.SONATA.read(filepath))
 
-    def save_sonata(self, filepath):
+    def save_sonata(self, filepath, population_name="vasculature"):
         """Save data using the SONATA specification"""
-        io.SONATA.write(filepath, self.node_properties, self.edge_properties)
+        io.SONATA.write(filepath, population_name, self.node_properties, self.edge_properties)
 
     @property
     def diameters(self):
         """Returns the diameters of the point graph"""
         return self._node_properties.loc[:, "diameter"].to_numpy()
 
     @diameters.setter
```

### Comparing `vascpy-0.1.1/vascpy/section_graph/__init__.py` & `vascpy-0.1.2/vascpy/section_graph/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/vascpy/section_graph/io.py` & `vascpy-0.1.2/vascpy/section_graph/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/vascpy/section_vasculature.py` & `vascpy-0.1.2/vascpy/section_vasculature.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -22,17 +22,22 @@
 class SectionVasculature:
     """Section representation of graphs"""
 
     def __init__(self, filepath):
         self._graph = morphio.vasculature.Vasculature(filepath)
 
     @classmethod
+    def load_hdf5(cls, filepath):
+        """Load morphology from hdf5 file"""
+        return cls(filepath)
+
+    @classmethod
     def load(cls, filepath):
         """Load morphology from file"""
-        return cls(filepath)
+        return SectionVasculature.load_hdf5(filepath)
 
     @property
     def points(self):
         """Returns the coordinates of the vertices in the morphology"""
         return self._graph.points
 
     @property
@@ -55,10 +60,14 @@
             mutable:
                 If True it will return a mutable point graph
         Returns:
             Point graph
         """
         return vascpy.conversion.convert_section_to_point_vasculature(self)
 
-    def save(self, filepath):
+    def save_hdf5(self, filepath):
         """Write morphology to file"""
         vascpy.section_graph.io.HDF5.write(filepath, self.points, self.diameters, self.sections)
+
+    def save(self, filepath):
+        """Write morphology to file"""
+        self.save_hdf5(filepath)
```

### Comparing `vascpy-0.1.1/vascpy/specs.py` & `vascpy-0.1.2/vascpy/specs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/vascpy/utils/__init__.py` & `vascpy-0.1.2/vascpy/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/vascpy/utils/adjacency.py` & `vascpy-0.1.2/vascpy/utils/adjacency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/vascpy/utils/geometry.py` & `vascpy-0.1.2/vascpy/utils/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/vascpy/utils/section_creation.py` & `vascpy-0.1.2/vascpy/utils/section_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2022 Blue Brain Project/EPFL
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vascpy-0.1.1/vascpy.egg-info/PKG-INFO` & `vascpy-0.1.2/vascpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: vascpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Vasculature API
 Home-page: https://github.com/BlueBrain/vascpy
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Project-URL: Tracker, https://github.com/BlueBrain/vascpy/issues
 Project-URL: Source, https://github.com/BlueBrain/vascpy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Provides-Extra: convert-vtk
 Provides-Extra: all
 Provides-Extra: docs
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
```

### Comparing `vascpy-0.1.1/vascpy.egg-info/SOURCES.txt` & `vascpy-0.1.2/vascpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 .readthedocs.yml
 AUTHORS.txt
 CONTRIBUTING.md
 LICENSE.txt
 MANIFEST.in
 README.md
+pylintrc
 pyproject.toml
 setup.py
 tox.ini
 .github/workflows/publish-sdist.yml
 .github/workflows/run-tox.yml
 doc/Makefile
 doc/source/conf.py
```

