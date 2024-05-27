# Comparing `tmp/neurom-3.2.9.tar.gz` & `tmp/neurom-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurom-3.2.9.tar", last modified: Mon Apr 15 13:03:15 2024, max compression
+gzip compressed data, was "neurom-4.0.0.tar", last modified: Mon May 27 07:47:53 2024, max compression
```

## Comparing `neurom-3.2.9.tar` & `neurom-4.0.0.tar`

### file list

```diff
@@ -1,129 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.498174 neurom-3.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.482174 neurom-3.2.9/.binder/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 13:03:10.000000 neurom-3.2.9/.binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 13:03:10.000000 neurom-3.2.9/.binder/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-15 13:03:10.000000 neurom-3.2.9/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 13:03:10.000000 neurom-3.2.9/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 13:03:10.000000 neurom-3.2.9/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.478174 neurom-3.2.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.482174 neurom-3.2.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-15 13:03:10.000000 neurom-3.2.9/.github/workflows/mirror-ebrains.yml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-15 13:03:10.000000 neurom-3.2.9/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-15 13:03:10.000000 neurom-3.2.9/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-15 13:03:10.000000 neurom-3.2.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-15 13:03:10.000000 neurom-3.2.9/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-15 13:03:10.000000 neurom-3.2.9/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-15 13:03:10.000000 neurom-3.2.9/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-15 13:03:10.000000 neurom-3.2.9/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-15 13:03:10.000000 neurom-3.2.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-15 13:03:10.000000 neurom-3.2.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 13:03:10.000000 neurom-3.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-15 13:03:15.498174 neurom-3.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-15 13:03:10.000000 neurom-3.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-15 13:03:10.000000 neurom-3.2.9/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.486173 neurom-3.2.9/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/clean.sh
--rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.486173 neurom-3.2.9/doc/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/definitions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/developer.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/features.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.486173 neurom-3.2.9/doc/source/images/
--rw-r--r--   0 runner    (1001) docker     (127)    27330 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/images/spherical_coordinates.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/images/spherical_coordinates.tex
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.486173 neurom-3.2.9/doc/source/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   403060 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/logo/NeuroM.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/migration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/morph_check.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/morph_stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/spherical_coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/validation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.490174 neurom-3.2.9/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/density_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4541 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/end_to_end_distance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2969 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/extract_distribution.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3710 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/features_graph_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6790 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/get_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/histogram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6050 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/iteration_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3226 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/nl_fst_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2957 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/plot_somas.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/radius_of_gyration.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2575 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/section_ids.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2859 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/soma_radius_fit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.490174 neurom-3.2.9/neurom/
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.494174 neurom-3.2.9/neurom/apps/
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.494174 neurom-3.2.9/neurom/apps/config/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/config/morph_check.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/config/morph_stats.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/morph_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/morph_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.494174 neurom-3.2.9/neurom/check/
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/check/morphology_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/check/morphtree.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/check/neuron_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/check/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.494174 neurom-3.2.9/neurom/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/dataformat.py
--rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/neuron.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/population.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12976 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/soma.py
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.494174 neurom-3.2.9/neurom/features/
--rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/bifurcation.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/bifurcationfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    27669 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)    15769 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/neurite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/population.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/section.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/sectionfunc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.494174 neurom-3.2.9/neurom/geom/
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/geom/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.498174 neurom-3.2.9/neurom/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/morphmath.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.498174 neurom-3.2.9/neurom/view/
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/view/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    17722 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/view/matplotlib_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16900 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/view/matplotlib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/view/plotly_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.498174 neurom-3.2.9/neurom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-15 13:03:15.000000 neurom-3.2.9/neurom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-15 13:03:15.000000 neurom-3.2.9/neurom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:03:15.000000 neurom-3.2.9/neurom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 13:03:15.000000 neurom-3.2.9/neurom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-15 13:03:15.000000 neurom-3.2.9/neurom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 13:03:15.000000 neurom-3.2.9/neurom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-15 13:03:10.000000 neurom-3.2.9/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-15 13:03:10.000000 neurom-3.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:03:15.498174 neurom-3.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:03:10.000000 neurom-3.2.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-15 13:03:10.000000 neurom-3.2.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.484569 neurom-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.468569 neurom-4.0.0/.binder/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 07:47:47.000000 neurom-4.0.0/.binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 07:47:47.000000 neurom-4.0.0/.binder/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-27 07:47:47.000000 neurom-4.0.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 07:47:47.000000 neurom-4.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 07:47:47.000000 neurom-4.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.464569 neurom-4.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.468569 neurom-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-27 07:47:47.000000 neurom-4.0.0/.github/workflows/mirror-ebrains.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-27 07:47:47.000000 neurom-4.0.0/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-27 07:47:47.000000 neurom-4.0.0/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-27 07:47:47.000000 neurom-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-27 07:47:47.000000 neurom-4.0.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-27 07:47:47.000000 neurom-4.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-27 07:47:47.000000 neurom-4.0.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-27 07:47:47.000000 neurom-4.0.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-27 07:47:47.000000 neurom-4.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-27 07:47:47.000000 neurom-4.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 07:47:47.000000 neurom-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-27 07:47:53.484569 neurom-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-27 07:47:47.000000 neurom-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-27 07:47:47.000000 neurom-4.0.0/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.464569 neurom-4.0.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.472569 neurom-4.0.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/definitions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/heterogeneous.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.472569 neurom-4.0.0/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/images/heterogeneous_neurite.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32564 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/images/heterogeneous_neuron.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27330 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/images/spherical_coordinates.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/images/spherical_coordinates.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.472569 neurom-4.0.0/doc/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   403060 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/logo/NeuroM.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/morph_check.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/morph_stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/spherical_coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/validation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.476569 neurom-4.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/density_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4549 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/end_to_end_distance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2959 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/extract_distribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3713 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/features_graph_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6847 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/get_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/histogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6065 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/iteration_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3272 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/nl_fst_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2826 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/plot_somas.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4922 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/radius_of_gyration.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2576 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/section_ids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2869 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/soma_radius_fit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.476569 neurom-4.0.0/neurom/
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.480569 neurom-4.0.0/neurom/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.480569 neurom-4.0.0/neurom/apps/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/config/morph_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/config/morph_stats.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/morph_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/morph_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.480569 neurom-4.0.0/neurom/check/
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/check/morphology_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/check/morphtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/check/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.480569 neurom-4.0.0/neurom/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/core/dataformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22149 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/core/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/core/population.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17859 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/core/soma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.484569 neurom-4.0.0/neurom/features/
+-rw-r--r--   0 runner    (1001) docker     (127)    10639 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/features/bifurcation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30454 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/features/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/features/neurite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/features/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/features/section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.484569 neurom-4.0.0/neurom/geom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/geom/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.484569 neurom-4.0.0/neurom/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17209 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/morphmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.484569 neurom-4.0.0/neurom/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/view/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17707 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/view/matplotlib_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16391 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/view/matplotlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/view/plotly_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.484569 neurom-4.0.0/neurom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-27 07:47:53.000000 neurom-4.0.0/neurom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-27 07:47:53.000000 neurom-4.0.0/neurom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:47:53.000000 neurom-4.0.0/neurom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 07:47:53.000000 neurom-4.0.0/neurom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-27 07:47:53.000000 neurom-4.0.0/neurom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 07:47:53.000000 neurom-4.0.0/neurom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-27 07:47:47.000000 neurom-4.0.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-27 07:47:47.000000 neurom-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:47:53.484569 neurom-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:47:47.000000 neurom-4.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-27 07:47:47.000000 neurom-4.0.0/tox.ini
```

### Comparing `neurom-3.2.9/.github/workflows/mirror-ebrains.yml` & `neurom-4.0.0/.github/workflows/mirror-ebrains.yml`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/.github/workflows/publish-sdist.yml` & `neurom-4.0.0/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/.github/workflows/run-tox.yml` & `neurom-4.0.0/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/.gitlab-ci.yml` & `neurom-4.0.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/.zenodo.json` & `neurom-4.0.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/CHANGELOG.rst` & `neurom-4.0.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 Changelog
 =========
 
+Version 4.0.0
+-------------
+
+- Morphology class accepts only morphio objects, not files anymore. (#1120)
+- Replace ``iter_*`` methods by properties in core objects and improve ``iter_segments``. (#1054)
+- NeuriteType extended to allow mixed type declarations as tuple of ints. (#1071)
+- All features return built-in types (#1064)
+- Morphology class also allows mutable morphio objects to be passed explicitly. (#1049)
+- Morphology class uses morphio immutable class by composition, istead of inheritance. (#979)
+- Morphology level radial distance features use the soma as reference point. (#1030)
+- Make ``neurom.core.Population`` resolve paths. Symlinks are not resolved. (#1047)
+- Mixed subtree processing can be used in morph_stats app via the use_subtrees flag. (#1034)
+- ``neurom.view.[plot_tree|plot_tree3d|plot_soma|plot_soma3D]`` were hidden from the
+  neurom.view module. They can still be imported from neurom.view.matplotlib_impl. (#1032)
+- Mixed subtree processing. (#981)
+- Deprecated modules and classes were removed. (#1026)
+
+
 Version 3.2.3
 -------------
 
 - Fix neurom.app.morph_stats.extract_dataframe for Population objects with several workers (#1080)
 - Update readthedocs config (#1077)
 - Can pass List[Population] args to neurom.app.morph_stats.extract_dataframe (#1076)
 - Fix compatibility with MorphIO>=3.3.6 (#1075)
```

### Comparing `neurom-3.2.9/LICENSE.txt` & `neurom-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/PKG-INFO` & `neurom-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurom
-Version: 3.2.9
+Version: 4.0.0
 Summary: NeuroM: a light-weight neuron morphology analysis package
 Author: Blue Brain Project, EPFL
 License: Copyright (c) 2015-2022 Blue Brain Project/EPFL 
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -50,14 +50,15 @@
 Requires-Dist: matplotlib>=3.2.1
 Requires-Dist: morphio>=3.3.6
 Requires-Dist: numpy>=1.8.0
 Requires-Dist: pandas>=1.0.5
 Requires-Dist: pyyaml>=3.10
 Requires-Dist: scipy>=1.2.0
 Requires-Dist: tqdm>=4.8.4
+Requires-Dist: cached_property>=1.5.1
 Requires-Dist: importlib_resources>=1.3; python_version < "3.9"
 Provides-Extra: plotly
 Requires-Dist: plotly>=3.6.0; extra == "plotly"
 Requires-Dist: psutil>=5.5.1; extra == "plotly"
 Provides-Extra: docs
 Requires-Dist: sphinx-bluebrain-theme; extra == "docs"
 Requires-Dist: sphinx-autorun; extra == "docs"
```

### Comparing `neurom-3.2.9/README.md` & `neurom-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/asv.conf.json` & `neurom-4.0.0/asv.conf.json`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/api.rst` & `neurom-4.0.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/cli.rst` & `neurom-4.0.0/doc/source/cli.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/conf.py` & `neurom-4.0.0/doc/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,32 +45,34 @@
 import importlib.metadata
 
 VERSION = importlib.metadata.version('neurom')
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.insert(0, os.path.abspath('.'))
+# sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.napoleon',
+    'sphinx.ext.doctest',
 ]
 
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # General information about the project.
 project = u'NeuroM'
 author = u'BBP Algorithm Development Section'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
@@ -82,184 +84,183 @@
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = []
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
-#keep_warnings = False
+# keep_warnings = False
 
 suppress_warnings = ["ref.python"]
 autosummary_generate = True
 autoclass_content = 'both'
 autodoc_default_options = {
     'members': True,
 }
 autosummary_mock_imports = ['plotly']
 
-#autoclass_content = 'both'
+# autoclass_content = 'both'
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = 'sphinx-bluebrain-theme'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
     "repo_url": "https://github.com/BlueBrain/NeuroM/",
-    "repo_name": "BlueBrain/NeuroM"
+    "repo_name": "BlueBrain/NeuroM",
 }
 
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 html_title = 'NeuroM'
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 # html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
-#html_extra_path = []
+# html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 # html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
 html_show_sourcelink = False
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Language to be used for generating the HTML full-text search index.
 # Sphinx supports the following languages:
 #   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
 #   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr'
-#html_search_language = 'en'
+# html_search_language = 'en'
 
 # A dictionary with options for the search language support, empty by default.
 # Now only 'ja' uses this config value
-#html_search_options = {'type': 'default'}
+# html_search_options = {'type': 'default'}
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
-#html_search_scorer = 'scorer.js'
+# html_search_scorer = 'scorer.js'
 
 # -- Options for LaTeX output ---------------------------------------------
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
-
+# man_show_urls = False
 
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
```

### Comparing `neurom-3.2.9/doc/source/definitions.rst` & `neurom-4.0.0/doc/source/definitions.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/developer.rst` & `neurom-4.0.0/doc/source/developer.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/documentation.rst` & `neurom-4.0.0/doc/source/documentation.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/examples.rst` & `neurom-4.0.0/doc/source/examples.rst`

 * *Files 6% similar despite different names*

```diff
@@ -31,42 +31,40 @@
 
 .. note::
 
     In following code samples, the prompt ``>>>`` indicates a python interpreter session
     started *with the virtualenv activated*. That gives access to the ``neurom``
     installation.
 
-Fast analysis with :py:mod:`neurom`
-***********************************
+Analysis with :py:mod:`neurom`
+******************************
 
 Here we load a morphology and obtain some information from it:
 
-.. code-block:: python
+.. doctest:: [examples]
 
     >>> import neurom as nm
-    >>> m = nm.load_morphology('some/data/path/morph_file.swc')
+    >>> m = nm.load_morphology("tests/data/swc/Neuron.swc")
     >>> ap_seg_len = nm.get('segment_lengths', m, neurite_type=nm.APICAL_DENDRITE)
     >>> ax_sec_len = nm.get('section_lengths', m, neurite_type=nm.AXON)
 
 
-Morphology visualization with the :py:mod:`neurom.viewer` module
-****************************************************************
+Morphology visualization with the :py:mod:`neurom.view` module
+**************************************************************
 
 Here we visualize a morphology:
 
 
-.. code-block:: python
+.. doctest:: [examples]
 
     >>> # Initialize m as above
-    >>> from neurom import viewer
-    >>> fig, ax = viewer.draw(m)
-    >>> fig.show()
-    >>>
-    >>> fig, ax = viewer.draw(m, mode='3d') # valid modes '2d', '3d', 'dendrogram'
-    >>> fig.show()
+    >>> from neurom.view import plot_morph, plot_morph3d, plot_dendrogram
+    >>> plot_morph(m)
+    >>> plot_morph3d(m)
+    >>> plot_dendrogram(m)
 
 Advanced iterator-based feature extraction example
 **************************************************
 
 These slightly more complex examples illustrate what can be done with the ``neurom``
 module's various generic iterators and simple morphometric functions.
 
@@ -85,15 +83,15 @@
 Getting Log Information
 ***********************
 
 ``neurom`` emits many logging statements during the course of its functioning.
 They are emitted in the ``neurom`` namespace, and can thus be filtered based
 on this.  An example of setting up a handler is:
 
-.. code-block:: python
+.. doctest::
 
     >>> import logging
     >>> # setup which namespace will be examined, and at what level
     >>> # in this case we only want messages from 'neurom' and all messages
     >>> # (ie: DEBUG, INFO, etc)
     >>> logger = logging.getLogger('neurom')
     >>> logger.setLevel(logging.DEBUG)
```

### Comparing `neurom-3.2.9/doc/source/features.rst` & `neurom-4.0.0/doc/source/features.rst`

 * *Files 8% similar despite different names*

```diff
@@ -44,62 +44,72 @@
 This restriction can be bypassed if you call a feature from ``neurite`` via the features
 mechanism ``features.get``. However the mechanism does not allow to appply ``population``
 features to anything other than a morphology population, and ``morphology`` features can be applied
 only to a morphology or a morphology population.
 
 An example for ``neurite``:
 
-.. code-block:: python
+.. testcode::
 
-   from neurom import load_morphology, features
-   from neurom.features.neurite import max_radial_distance
+    from neurom import load_morphology, features
+    from neurom.features.neurite import max_radial_distance
+
+    m = load_morphology("tests/data/swc/Neuron.swc")
+
+    # valid input
+    rd = max_radial_distance(m.neurites[0])
+
+    # invalid input
+    # rd = max_radial_distance(m)
+
+    # valid input
+    rd = features.get('max_radial_distance', m)
 
-   m = load_morphology('path/to/morphology')
-   # valid input
-   max_radial_distance(m.neurites[0])
-   # invalid input
-   max_radial_distance(m)
-   # valid input
-   features.get('max_radial_distance', m)
 
 The features mechanism assumes that a neurite feature must be summed if it returns a number, and
 concatenated if it returns a list. Other types of returns are invalid. For example lets take
 a feature ``number_of_segments`` of ``neurite``. It returns a number of segments in a neurite.
 Calling it on a morphology will return a sum of ``number_of_segments`` of all the morphology's neurites.
 Calling it on a morphology population will return a list of ``number_of_segments`` of each morphology
 within the population.
 
 
-.. code-block:: python
+.. testcode::
+
+   from neurom import load_morphology, load_morphologies, features
 
-   from neurom import load_morphology, features
+   m = load_morphology("tests/data/swc/Neuron.swc")
 
-   m = load_morphology('path/to/morphology')
    # a single number
    features.get('number_of_segments', m.neurites[0])
+
    # a single number that is a sum for all `m.neurites`.
    features.get('number_of_segments', m)
 
-   pop = load_morphology('path/to/morphology population')
+   pop = load_morphologies("tests/data/valid_set")
+
    # a list of numbers
    features.get('number_of_segments', pop)
 
 if a list is returned then the feature results are concatenated.
 
-.. code-block:: python
+.. testcode::
+
+   from neurom import load_morphology, load_morphologies, features
 
-   from neurom import load_morphology, features
+   m = load_morphology("tests/data/swc/Neuron.swc")
 
-   m = load_morphology('path/to/morphology')
    # a list of lengths in a neurite
    features.get('section_lengths', m.neurites[0])
+
    # a flat list of lengths in a morphology, no separation among neurites
    features.get('section_lengths', m)
 
-   pop = load_morphology('path/to/morphology population')
+   pop = load_morphologies("tests/data/valid_set")
+
    # a flat list of lengths in a population, no separation among morphologies
    features.get('section_lengths', pop)
 
 In case such implicit behaviour does not work a feature can be rewritten for each input separately.
 For example, a feature ``max_radial_distance`` that requires a `max` operation instead of implicit
 `sum`. Its definition in ``neurite``:
```

### Comparing `neurom-3.2.9/doc/source/images/spherical_coordinates.svg` & `neurom-4.0.0/doc/source/images/spherical_coordinates.svg`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/images/spherical_coordinates.tex` & `neurom-4.0.0/doc/source/images/spherical_coordinates.tex`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/index.rst` & `neurom-4.0.0/doc/source/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
    quickstart
    install
    validation
    tutorial
    features
    spherical_coordinates
    examples
+   heterogeneous
    cli
    definitions
    api
    developer
    documentation
    migration
    changelog
```

### Comparing `neurom-3.2.9/doc/source/install.rst` & `neurom-4.0.0/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/license.rst` & `neurom-4.0.0/doc/source/license.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/logo/NeuroM.jpg` & `neurom-4.0.0/doc/source/logo/NeuroM.jpg`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/migration.rst` & `neurom-4.0.0/examples/density_plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,156 @@
-.. Copyright (c) 2015, Ecole Polytechnique Federale de Lausanne, Blue Brain Project
-   All rights reserved.
+# Copyright (c) 2015, Ecole Polytechnique Federale de Lausanne, Blue Brain Project
+# All rights reserved.
+#
+# This file is part of NeuroM <https://github.com/BlueBrain/NeuroM>
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are met:
+#
+#     1. Redistributions of source code must retain the above copyright
+#        notice, this list of conditions and the following disclaimer.
+#     2. Redistributions in binary form must reproduce the above copyright
+#        notice, this list of conditions and the following disclaimer in the
+#        documentation and/or other materials provided with the distribution.
+#     3. Neither the name of the copyright holder nor the names of
+#        its contributors may be used to endorse or promote products
+#        derived from this software without specific prior written permission.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY
+# DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+# ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+"""Example for generating density plots."""
+from pathlib import Path
+
+import pylab as plt
+import matplotlib as mpl
+import numpy as np
+
+from neurom import get as get_feat
+from neurom.view import matplotlib_utils, matplotlib_impl
+from neurom.core.types import NeuriteType
+
+from neurom import load_morphologies
+
+PACKAGE_DIR = Path(__file__).resolve().parent.parent
+
+
+def extract_density(population, plane="xy", bins=100, neurite_type=NeuriteType.basal_dendrite):
+    """Extracts the 2d histogram of the center
+    coordinates of segments in the selected plane.
+    """
+    segment_midpoints = np.array(
+        get_feat("segment_midpoints", population, neurite_type=neurite_type)
+    )
+    horiz = segment_midpoints[:, "xyz".index(plane[0])]
+    vert = segment_midpoints[:, "xyz".index(plane[1])]
+    return np.histogram2d(np.array(horiz), np.array(vert), bins=(bins, bins))
+
+
+def plot_density(
+    population,  # pylint: disable=too-many-arguments, too-many-locals
+    bins=100,
+    new_fig=True,
+    subplot=111,
+    levels=None,
+    plane="xy",
+    colorlabel="Nodes per unit area",
+    labelfontsize=16,
+    color_map="Reds",
+    no_colorbar=False,
+    threshold=0.01,
+    neurite_type=NeuriteType.basal_dendrite,
+    **kwargs,
+):
+    """Plots the 2d histogram of the center
+    coordinates of segments in the selected plane.
+    """
+    fig, ax = matplotlib_utils.get_figure(new_fig=new_fig, subplot=subplot)
+
+    H1, xedges1, yedges1 = extract_density(
+        population, plane=plane, bins=bins, neurite_type=neurite_type
+    )
+
+    mask = H1 < threshold  # mask = H1==0
+    H2 = np.ma.masked_array(H1, mask)
+
+    colormap = plt.get_cmap(color_map).copy()
+    colormap.set_bad(color='white', alpha=None)
+
+    plots = ax.contourf(
+        (xedges1[:-1] + xedges1[1:]) / 2,
+        (yedges1[:-1] + yedges1[1:]) / 2,
+        np.transpose(H2),  # / np.max(H2),
+        cmap=colormap,
+        levels=levels,
+    )
+
+    if not no_colorbar:
+        cbar = plt.colorbar(plots)
+        cbar.ax.set_ylabel(colorlabel, fontsize=labelfontsize)
+
+    kwargs["title"] = kwargs.get("title", "")
+    kwargs["xlabel"] = kwargs.get("xlabel", plane[0])
+    kwargs["ylabel"] = kwargs.get("ylabel", plane[1])
+
+    return matplotlib_utils.plot_style(fig=fig, ax=ax, **kwargs)
+
+
+def plot_neuron_on_density(
+    population,  # pylint: disable=too-many-arguments
+    bins=100,
+    new_fig=True,
+    subplot=111,
+    levels=None,
+    plane="xy",
+    colorlabel="Nodes per unit area",
+    labelfontsize=16,
+    color_map="Reds",
+    no_colorbar=False,
+    threshold=0.01,
+    neurite_type=NeuriteType.basal_dendrite,
+    **kwargs,
+):
+    """Plots the 2d histogram of the center
+    coordinates of segments in the selected plane
+    and superimposes the view of the first neurite of the collection.
+    """
+    _, ax = matplotlib_utils.get_figure(new_fig=new_fig)
+
+    ref_neuron = population[0]
+    matplotlib_impl.plot_tree(ref_neuron.neurites[0], ax)
+
+    return plot_density(
+        population,
+        plane=plane,
+        bins=bins,
+        new_fig=False,
+        subplot=subplot,
+        colorlabel=colorlabel,
+        labelfontsize=labelfontsize,
+        levels=levels,
+        color_map=color_map,
+        no_colorbar=no_colorbar,
+        threshold=threshold,
+        neurite_type=neurite_type,
+        **kwargs,
+    )
+
+
+def main():
+    morphology_directory = Path(PACKAGE_DIR, "tests/data/valid_set")
+    neurons = load_morphologies(morphology_directory)
 
-   This file is part of NeuroM <https://github.com/BlueBrain/NeuroM>
+    plot_density(neurons)
+    plot_neuron_on_density(neurons)
 
-   Redistribution and use in source and binary forms, with or without
-   modification, are permitted provided that the following conditions are met:
 
-       1. Redistributions of source code must retain the above copyright
-          notice, this list of conditions and the following disclaimer.
-       2. Redistributions in binary form must reproduce the above copyright
-          notice, this list of conditions and the following disclaimer in the
-          documentation and/or other materials provided with the distribution.
-       3. Neither the name of the copyright holder nor the names of
-          its contributors may be used to endorse or promote products
-          derived from this software without specific prior written permission.
-
-   THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-   ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-   WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-   DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY
-   DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-   (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-   LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-   ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-   (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-   SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-Migration guides
-=======================
-
-.. _migration-v3.0.0:
-
-Migration to v3 version
------------------------
-
-- ``neurom.view.viewer`` is deprecated. To get the same results as before, use the replacement:
-
-   .. code-block:: python
-
-      import neurom as nm
-      # instead of: from neurom import viewer
-      from neurom.view import matplotlib_impl, matplotlib_utils
-      m = nm.load_morphology('some/data/path/morph_file.asc')
-
-      # instead of: viewer.draw(m)
-      matplotlib_impl.plot_morph(m)
-
-      # instead of: viewer.draw(m, mode='3d')
-      matplotlib_impl.plot_morph3d(m)
-
-      # instead of: viewer.draw(m, mode='dendrogram')
-      matplotlib_impl.plot_dendrogram(m)
-
-      # If you used ``output_path`` with any of functions above then the solution is:
-      fig, ax = matplotlib_utils.get_figure()
-      matplotlib_impl.plot_dendrogram(m, ax)
-      matplotlib_utils.plot_style(fig=fig, ax=ax)
-      matplotlib_utils.save_plot(fig=fig, output_path=output_path)
-      # for other plots like `plot_morph` it is the same, you just need to call `plot_morph` instead
-      # of `plot_dendrogram`.
-
-      # instead of `plotly.draw`
-      from neurom import plotly_impl
-      plotly_impl.plot_morph(m)  # for 2d
-      plotly_impl.plot_morph3d(m)  # for 3d
-
-- breaking features changes:
-   - use `max_radial_distance` instead of `max_radial_distances`
-   - use `number_of_segments` instead of `n_segments`
-   - use `number_of_neurites` instead of `n_neurites`
-   - use `number_of_sections` instead of `n_sections`
-   - use `number_of_bifurcations` instead of `n_bifurcation_points`
-   - use `number_of_forking_points` instead of `n_forking_points`
-   - use `number_of_leaves` instead of `number_of_terminations`, `n_leaves`
-   - use `soma_radius` instead of `soma_radii`
-   - use `soma_surface_area` instead of `soma_surface_areas`
-   - use `soma_volume` instead of `soma_volumes`
-   - use `total_length_per_neurite` instead of `neurite_lengths`
-   - use `total_volume_per_neurite` instead of `neurite_volumes`
-   - use `terminal_path_lengths` instead of `terminal_path_lengths_per_neurite`
-   - use `bifurcation_partitions` instead of `partition`
-   - new neurite feature `total_area` that complements `total_area_per_neurite`
-   - new neurite feature `volume_density` that complements `neurite_volume_density`
-
-
-Migration to v2 version
------------------------
-.. _migration-v2:
-
-- ``Neuron`` object now extends ``morphio.Morphology``.
-- NeuroM does not remove unifurcations on load. Unifurcation is a section with a single child. Such
-  sections are possible in H5 and ASC formats. Now, in order to remove them on your morphology, you
-  would need to call ``remove_unifurcations()`` right after the morphology is constructed.
-
-  .. code-block:: python
-
-      import neurom as nm
-      nrn = nm.load_morphology('some/data/path/morph_file.asc')
-      nrn.remove_unifurcations()
-
-- Soma is not considered as a section anymore. Soma is skipped when iterating over morphology's
-  sections. It means that section indexing offset needs to be adjusted by
-  ``-(number of soma sections)`` which is usually ``-1``.
-- drop ``benchmarks``
-- drop ``neurom.check.structural_checks`` as MorphIO does not allow to load invalid morphologies,
-  and it does not give access to raw data.
-- drop ``Tree`` class. Use ``Section`` instead as it includes its functionality but if you need
-  ``Tree`` separately then copy-paste ``Tree`` code from v1 version to your project.
-- ``Section`` and ``Neurite`` class can't be copied anymore because their underlying MorphIO
-  objects can't be copied (pickled). Only copying of ``Neuron`` is preserved.
-- drop ``FstNeuron``. It functionality is included in ``Neuron`` class. Use ``Neuron`` instead of
-  ``FstNeuron``.
-- Validation of morphologies changed.
-    The following is not an invalid morphology anymore:
-
-    - 2 point soma
-    - non-sequential ids
-- script ``morph_check`` and ``morph_stats`` changed to ``neurom check`` and ``neurom stats``
-    correspondingly.
+if __name__ == "__main__":
+    main()
```

### Comparing `neurom-3.2.9/doc/source/morph_check.rst` & `neurom-4.0.0/doc/source/morph_check.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/morph_stats.rst` & `neurom-4.0.0/doc/source/morph_stats.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/quickstart.rst` & `neurom-4.0.0/doc/source/quickstart.rst`

 * *Files 3% similar despite different names*

```diff
@@ -53,39 +53,38 @@
 
 Extract morphometrics with :func:`neurom.features.get`
 ------------------------------------------------------
 
 Analyze morphologies via :func:`neurom.features.get`. This way you can get things like segment
 lengths, section lengths, etc.
 
-.. code::
+.. testcode::
 
     import neurom as nm
-    m = nm.load_morphology('some/data/path/morph_file0.swc')
+    m = nm.load_morphology('tests/data/swc/Neuron.swc')
     m_ap_seg_len = nm.features.get('segment_lengths', m, neurite_type=nm.APICAL_DENDRITE)
-    pop = nm.load_morphologies('some/data/path')
+    pop = nm.load_morphologies('tests/data/valid_set/')
     pop_ap_seg_len = nm.features.get('segment_lengths', pop, neurite_type=nm.APICAL_DENDRITE)
 
 For more details see :ref:`features`.
 
 Iterate over neurites with :func:`neurom.core.morphology.iter_neurites`
 -----------------------------------------------------------------------
 
 :func:`neurom.core.morphology.iter_neurites` function allows to iterate over the neurites
 of a single morphology or a morphology population. It can also be applied to a single
 neurite or a list of neurites. It allows to optionally pass a function to be
 mapped onto each neurite, as well as a neurite filter function. In this example,
 we apply a simple user defined function to the apical dendrites in a population:
 
-.. code::
+.. testcode::
 
     import neurom as nm
 
-    def user_func(neurite):
-        print('Analysing neurite', neurite)
+    def user_func(neurite, section_type):
         return len(neurite.points)
 
     stuff = [x for x in nm.iter_neurites(pop, user_func, lambda n : n.type == nm.APICAL_DENDRITE)]
 
 View morphologies with :mod:`neurom.viewer`
 -------------------------------------------
```

### Comparing `neurom-3.2.9/doc/source/spherical_coordinates.rst` & `neurom-4.0.0/doc/source/spherical_coordinates.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/tutorial.rst` & `neurom-4.0.0/doc/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/doc/source/validation.rst` & `neurom-4.0.0/doc/source/validation.rst`

 * *Files 8% similar despite different names*

```diff
@@ -32,27 +32,27 @@
 *********************
 
 What morphology is valid or invalid? NeuroM completely follows MorphIO in this question because
 NeuroM uses MorphIO for reading/writing of morphologies. The rule is be less rigid as possible.
 If there is a problem with morphology then NeuroM rather print a warning about instead of raising
 an error. If you want validate morphologies as strictly as possible then
 
-.. code-block:: python
+.. testcode:: [validation]
 
    import morphio
    morphio.set_raise_warnings(True)
 
 This will make MorphIO (hence NeuroM as well) raise warnings as errors. You might want to skip some
 warnings at all. For example, zero diameter is ok to have in your morpology. Then you can:
 
-.. code-block:: python
+.. testcode:: [validation]
 
    try:
        morphio.set_raise_warnings(True)
        # warnings you are not interested in
        morphio.set_ignored_warning(morphio.Warning.zero_diameter, True)
-       m = morphio.Morphology('path/to/morph')
+       m = morphio.Morphology('tests/data/swc/soma_zero_radius.swc')
    finally:
        morphio.set_ignored_warning(morphio.Warning.zero_diameter, False)
        morphio.set_raise_warnings(False)
 
-For more documentation on that topic refer to `<https://morphio.readthedocs.io/en/latest/warnings.html>`__.
+For more documentation on that topic refer to `<https://morphio.readthedocs.io/en/latest/warnings.html>`__.
```

### Comparing `neurom-3.2.9/examples/boxplot.py` & `neurom-4.0.0/examples/boxplot.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     ax.set_xticklabels(x_labels)
 
     # uncomment below to show image
     # pylab.show()
 
 
 def main():
-
-    morphology_directory =  Path(PACKAGE_DIR, "tests/data/valid_set")
+    morphology_directory = Path(PACKAGE_DIR, "tests/data/valid_set")
     neurons = load_morphologies(morphology_directory)
     boxplot(neurons, "section_lengths")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `neurom-3.2.9/examples/end_to_end_distance.py` & `neurom-4.0.0/examples/end_to_end_distance.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,66 +38,75 @@
 
 PACKAGE_DIR = Path(__file__).resolve().parent.parent
 
 
 def path_end_to_end_distance(neurite):
     """Calculate and return end-to-end-distance of a given neurite."""
     trunk = neurite.root_node.points[0]
-    return max(morphmath.point_dist(l.points[-1], trunk)
-               for l in neurite.root_node.ileaf())
+    return max(morphmath.point_dist(l.points[-1], trunk) for l in neurite.root_node.ileaf())
 
 
 def mean_end_to_end_dist(neurites):
     """Calculate mean end to end distance for set of neurites."""
     return np.mean([path_end_to_end_distance(n) for n in neurites])
 
 
 def make_end_to_end_distance_plot(nb_segments, end_to_end_distance, neurite_type):
     """Plot end-to-end distance vs number of segments."""
     plt.figure()
     plt.plot(nb_segments, end_to_end_distance)
     plt.title(neurite_type)
-    plt.xlabel('Number of segments')
-    plt.ylabel('End-to-end distance')
+    plt.xlabel("Number of segments")
+    plt.ylabel("End-to-end distance")
     # uncomment to show
-    #plt.show()
+    # plt.show()
 
 
 def calculate_and_plot_end_to_end_distance(neurite):
     """Calculate and plot the end-to-end distance vs the number of segments for
     an increasingly larger part of a given neurite.
 
     Note that the plots are not very meaningful for bifurcating trees."""
+
     def _dist(seg):
         """Distance between segmenr end and trunk."""
         return morphmath.point_dist(seg[1], neurite.root_node.points[0])
 
     end_to_end_distance = [_dist(s) for s in nm.iter_segments(neurite)]
-    make_end_to_end_distance_plot(np.arange(len(end_to_end_distance)) + 1,
-                                  end_to_end_distance, neurite.type)
+    make_end_to_end_distance_plot(
+        np.arange(len(end_to_end_distance)) + 1, end_to_end_distance, neurite.type
+    )
 
 
 def main():
     #  load a neuron from an SWC file
-    filename = Path(PACKAGE_DIR, 'tests/data/swc/Neuron_3_random_walker_branches.swc')
+    filename = Path(PACKAGE_DIR, "tests/data/swc/Neuron_3_random_walker_branches.swc")
     m = nm.load_morphology(filename)
 
     # print mean end-to-end distance per neurite type
-    print('Mean end-to-end distance for axons: ',
-          mean_end_to_end_dist(n for n in m.neurites if n.type == nm.AXON))
-    print('Mean end-to-end distance for basal dendrites: ',
-          mean_end_to_end_dist(n for n in m.neurites if n.type == nm.BASAL_DENDRITE))
-    print('Mean end-to-end distance for apical dendrites: ',
-          mean_end_to_end_dist(n for n in m.neurites
-                               if n.type == nm.APICAL_DENDRITE))
+    print(
+        "Mean end-to-end distance for axons: ",
+        mean_end_to_end_dist(n for n in m.neurites if n.type == nm.AXON),
+    )
+    print(
+        "Mean end-to-end distance for basal dendrites: ",
+        mean_end_to_end_dist(n for n in m.neurites if n.type == nm.BASAL_DENDRITE),
+    )
+    print(
+        "Mean end-to-end distance for apical dendrites: ",
+        mean_end_to_end_dist(n for n in m.neurites if n.type == nm.APICAL_DENDRITE),
+    )
 
-    print('End-to-end distance per neurite (nb segments, end-to-end distance, neurite type):')
+    print("End-to-end distance per neurite (nb segments, end-to-end distance, neurite type):")
     for nrte in m.neurites:
         # plot end-to-end distance for increasingly larger parts of neurite
         calculate_and_plot_end_to_end_distance(nrte)
         # print (number of segments, end-to-end distance, neurite type)
-        print(sum(len(s.points) - 1 for s in nrte.root_node.ipreorder()),
-              path_end_to_end_distance(nrte), nrte.type)
+        print(
+            sum(len(s.points) - 1 for s in nrte.root_node.ipreorder()),
+            path_end_to_end_distance(nrte),
+            nrte.type,
+        )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `neurom-3.2.9/examples/extract_distribution.py` & `neurom-4.0.0/examples/extract_distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,34 +43,31 @@
 
 
 PACKAGE_DIR = Path(__file__).resolve().parent.parent
 
 
 def find_optimal_distribution(population_directory, feature):
     """Loads a list of morphologies, extracts feature
-       and transforms the fitted distribution in the correct format.
-       Returns the optimal distribution, corresponding parameters,
-       minimun and maximum values.
+    and transforms the fitted distribution in the correct format.
+    Returns the optimal distribution, corresponding parameters,
+    minimun and maximum values.
     """
     population = nm.load_morphologies(population_directory)
 
     feature_data = [nm.get(feature, n) for n in population]
     feature_data = list(chain(*feature_data))
 
     return stats.optimal_distribution(feature_data)
 
 
 def main():
-
     population_directory = Path(PACKAGE_DIR, "tests/data/valid_set")
 
     result = stats.fit_results_to_dict(
-	find_optimal_distribution(population_directory, "section_lengths")
+        find_optimal_distribution(population_directory, "section_lengths")
     )
 
-    print(json.dumps(
-	result, indent=2, separators=(',', ': '), cls=NeuromJSON
-    ))
+    print(json.dumps(result, indent=2, separators=(",", ": "), cls=NeuromJSON))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `neurom-3.2.9/examples/features_graph_table.py` & `neurom-4.0.0/examples/features_graph_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,18 +35,17 @@
 from neurom.io.utils import get_morph_files
 
 
 PACKAGE_DIR = Path(__file__).resolve().parent.parent
 
 
 def stylize(ax, name, feature):
-    """Stylization modifications to the plots
-    """
+    """Stylization modifications to the plots"""
     ax.set_ylabel(feature)
-    ax.set_title(name, fontsize='small')
+    ax.set_title(name, fontsize="small")
 
 
 def histogram(neuron, feature, ax, bins=15, normed=True, cumulative=False):
     """
     Plot a histogram of the selected feature for the population of morphologies.
     Plots x-axis versus y-axis on a scatter|histogram|binned values plot.
 
@@ -69,43 +68,41 @@
 
     feature_values = nm.get(feature, neuron)
     # generate histogram
     ax.hist(feature_values, bins=bins, cumulative=cumulative, density=normed)
 
 
 def plot_feature(feature, cell):
-    """Plot a feature
-    """
+    """Plot a feature"""
     fig = pl.figure()
     ax = fig.add_subplot(111)
 
     if cell is not None:
         try:
             histogram(cell, feature, ax)
         except ValueError:
             pass
         stylize(ax, cell.name, feature)
     return fig
 
 
 def create_feature_plots(morphologies_dir, feature_list, output_dir):
-
     for morph_file in get_morph_files(morphologies_dir):
         m = nm.load_morphology(morph_file)
 
         for feature_name in feature_list:
             f = plot_feature(feature_name, m)
             figname = f"{feature_name}_{m.name}.eps"
             f.savefig(Path(output_dir, figname))
             pl.close(f)
 
 
 def main():
     create_feature_plots(
         morphologies_dir=Path(PACKAGE_DIR, "tests/data/valid_set"),
-	feature_list=["section_lengths"],
-	output_dir=".",
+        feature_list=["section_lengths"],
+        output_dir=".",
     )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `neurom-3.2.9/examples/histogram.py` & `neurom-4.0.0/examples/histogram.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,48 +72,45 @@
             The first item is either a figure object (if subplot is False) or an
             axis object. The second item is an object containing the data used to
             generate the figure. The final item is text used in report generation
             as a figure legend. This text needs to be manually entered in each
             figure file.
     """
 
-    bins = kwargs.get('bins', 25)
-    cumulative = kwargs.get('cumulative', False)
+    bins = kwargs.get("bins", 25)
+    cumulative = kwargs.get("cumulative", False)
 
     fig, ax = matplotlib_utils.get_figure(new_fig=new_fig, subplot=subplot)
 
-    kwargs['xlabel'] = kwargs.get('xlabel', feature)
+    kwargs["xlabel"] = kwargs.get("xlabel", feature)
 
-    kwargs['ylabel'] = kwargs.get('ylabel', feature + ' fraction')
+    kwargs["ylabel"] = kwargs.get("ylabel", feature + " fraction")
 
-    kwargs['title'] = kwargs.get('title', feature + ' histogram')
+    kwargs["title"] = kwargs.get("title", feature + " histogram")
 
     feature_values = [neurom.features.get(feature, neu) for neu in neurons]
 
     neu_labels = [neu.name for neu in neurons]
 
     ax.hist(feature_values, bins=bins, cumulative=cumulative, label=neu_labels, density=normed)
 
-    kwargs['no_legend'] = len(neu_labels) == 1
+    kwargs["no_legend"] = len(neu_labels) == 1
 
     return matplotlib_utils.plot_style(fig=fig, ax=ax, **kwargs)
 
 
 def population_feature_values(pops, feature):
-    """Extracts feature values per population
-    """
+    """Extracts feature values per population"""
     pops_feature_values = []
 
     for pop in pops:
-
         feature_values = [neurom.features.get(feature, neu) for neu in pop]
 
         # ugly hack to chain in case of list of lists
         if any([isinstance(p, (list, np.ndarray)) for p in feature_values]):
-
             feature_values = list(chain(*feature_values))
 
         pops_feature_values.append(feature_values)
 
     return pops_feature_values
 
 
@@ -148,38 +145,39 @@
             The first item is either a figure object (if subplot is False) or an
             axis object. The second item is an object containing the data used to
             generate the figure. The final item is text used in report generation
             as a figure legend. This text needs to be manually entered in each
             figure file.
     """
 
-    bins = kwargs.get('bins', 25)
-    cumulative = kwargs.get('cumulative', False)
+    bins = kwargs.get("bins", 25)
+    cumulative = kwargs.get("cumulative", False)
 
     fig, ax = matplotlib_utils.get_figure(new_fig=new_fig, subplot=subplot)
 
-    kwargs['xlabel'] = kwargs.get('xlabel', feature)
+    kwargs["xlabel"] = kwargs.get("xlabel", feature)
 
-    kwargs['ylabel'] = kwargs.get('ylabel', feature + ' fraction')
+    kwargs["ylabel"] = kwargs.get("ylabel", feature + " fraction")
 
-    kwargs['title'] = kwargs.get('title', feature + ' histogram')
+    kwargs["title"] = kwargs.get("title", feature + " histogram")
 
     pops_feature_values = population_feature_values(pops, feature)
 
     pops_labels = [pop.name for pop in pops]
 
-    ax.hist(pops_feature_values, bins=bins, cumulative=cumulative, label=pops_labels, density=normed)
+    ax.hist(
+        pops_feature_values, bins=bins, cumulative=cumulative, label=pops_labels, density=normed
+    )
 
-    kwargs['no_legend'] = len(pops_labels) == 1
+    kwargs["no_legend"] = len(pops_labels) == 1
 
     return matplotlib_utils.plot_style(fig=fig, ax=ax, **kwargs)
 
 
 def main():
-
     pop1 = load_morphologies(Path(PACKAGE_DIR, "tests/data/valid_set"))
     pop2 = load_morphologies(Path(PACKAGE_DIR, "tests/data/valid_set"))
     population_histogram([pop1, pop2], "section_lengths")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `neurom-3.2.9/examples/iteration_analysis.py` & `neurom-4.0.0/examples/iteration_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,16 +44,15 @@
 from neurom import morphmath as mm
 import numpy as np
 
 PACKAGE_DIR = Path(__file__).resolve().parent.parent
 
 
 def main():
-
-    filename = Path(PACKAGE_DIR, 'tests/data/swc/Neuron.swc')
+    filename = Path(PACKAGE_DIR, "tests/data/swc/Neuron.swc")
 
     #  load a neuron from an SWC file
     m = nm.load_morphology(filename)
 
     # Some examples of what can be done using iteration
     # instead of pre-packaged functions that return lists.
     # The iterations give us a lot of flexibility: we can map
@@ -61,90 +60,102 @@
 
     # Get of all neurites in cell by iterating over sections,
     # and summing the section lengths
     def sec_len(sec):
         """Return the length of a section."""
         return mm.section_length(sec.points)
 
-    print('Total neurite length (sections):',
-          sum(sec_len(s) for s in nm.iter_sections(m)))
+    print("Total neurite length (sections):", sum(sec_len(s) for s in nm.iter_sections(m)))
 
     # Get length of all neurites in cell by iterating over segments,
     # and summing the segment lengths.
     # This should yield the same result as iterating over sections.
-    print('Total neurite length (segments):',
-          sum(mm.segment_length(s) for s in nm.iter_segments(m)))
+    print(
+        "Total neurite length (segments):", sum(mm.segment_length(s) for s in nm.iter_segments(m))
+    )
 
     # get volume of all neurites in cell by summing over segment
     # volumes
-    print('Total neurite volume:',
-          sum(mm.segment_volume(s) for s in nm.iter_segments(m)))
+    print("Total neurite volume:", sum(mm.segment_volume(s) for s in nm.iter_segments(m)))
 
     # get area of all neurites in cell by summing over segment
     # areas
-    print('Total neurite surface area:',
-          sum(mm.segment_area(s) for s in nm.iter_segments(m)))
+    print("Total neurite surface area:", sum(mm.segment_area(s) for s in nm.iter_segments(m)))
 
     # get total number of neurite points in cell.
     def n_points(sec):
         """number of points in a section."""
         n = len(sec.points)
         # Non-root sections have duplicate first point
         return n if sec.parent is None else n - 1
 
-    print('Total number of points:',
-          sum(n_points(s) for s in nm.iter_sections(m)))
+    print("Total number of points:", sum(n_points(s) for s in nm.iter_sections(m)))
 
     # get mean radius of neurite points in cell.
     # p[COLS.R] yields the radius for point p.
     # Note: this includes duplicated points at beginning of
     # non-trunk sections
-    print('Mean radius of points:',
-          np.mean([s.points[:, COLS.R] for s in nm.iter_sections(m)]))
+    print("Mean radius of points:", np.mean([s.points[:, COLS.R] for s in nm.iter_sections(m)]))
 
     # get mean radius of neurite points in cell.
     # p[COLS.R] yields the radius for point p.
     # Note: this includes duplicated points at beginning of
     # non-trunk sections
     pts = [p[COLS.R] for s in m.sections[1:] for p in s.points]
-    print('Mean radius of points:',
-          np.mean(pts))
+    print("Mean radius of points:", np.mean(pts))
 
     # get mean radius of segments
-    print('Mean radius of segments:',
-          np.mean(list(mm.segment_radius(s) for s in nm.iter_segments(m))))
+    print(
+        "Mean radius of segments:", np.mean(list(mm.segment_radius(s) for s in nm.iter_segments(m)))
+    )
 
     # get stats for the segment taper rate, for different types of neurite
     for ttype in NEURITES:
         ttt = ttype
-        seg_taper_rate = [mm.segment_taper_rate(s)
-                          for s in nm.iter_segments(m, neurite_filter=tree_type_checker(ttt))]
-
-        print('Segment taper rate (', ttype,
-              '):\n  mean=', np.mean(seg_taper_rate),
-              ', std=', np.std(seg_taper_rate),
-              ', min=', np.min(seg_taper_rate),
-              ', max=', np.max(seg_taper_rate),
-              sep='')
+        seg_taper_rate = [
+            mm.segment_taper_rate(s)
+            for s in nm.iter_segments(m, neurite_filter=tree_type_checker(ttt))
+        ]
+
+        print(
+            "Segment taper rate (",
+            ttype,
+            "):\n  mean=",
+            np.mean(seg_taper_rate),
+            ", std=",
+            np.std(seg_taper_rate),
+            ", min=",
+            np.min(seg_taper_rate),
+            ", max=",
+            np.max(seg_taper_rate),
+            sep="",
+        )
 
     # Number of bifurcation points.
-    print('Number of bifurcation points:',
-          sum(1 for _ in nm.iter_sections(m,
-                                          iterator_type=Section.ibifurcation_point)))
+    print(
+        "Number of bifurcation points:",
+        sum(1 for _ in nm.iter_sections(m, iterator_type=Section.ibifurcation_point)),
+    )
 
     # Number of bifurcation points for apical dendrites
-    print('Number of bifurcation points (apical dendrites):',
-          sum(1 for _ in nm.iter_sections(m,
-                                          iterator_type=Section.ibifurcation_point,
-                                          neurite_filter=tree_type_checker(nm.APICAL_DENDRITE))))
+    print(
+        "Number of bifurcation points (apical dendrites):",
+        sum(
+            1
+            for _ in nm.iter_sections(
+                m,
+                iterator_type=Section.ibifurcation_point,
+                neurite_filter=tree_type_checker(nm.APICAL_DENDRITE),
+            )
+        ),
+    )
 
     # Maximum branch order
-    print('Maximum branch order:',
-          max(section.branch_order(s) for s in nm.iter_sections(m)))
+    print("Maximum branch order:", max(section.branch_order(s) for s in nm.iter_sections(m)))
 
     # Morphology's bounding box
     # Note: does not account for soma radius
-    print('Bounding box ((min x, y, z), (max x, y, z))', geom.bounding_box(m))
+    print("Bounding box ((min x, y, z), (max x, y, z))", geom.bounding_box(m))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `neurom-3.2.9/examples/nl_fst_compat.py` & `neurom-4.0.0/examples/nl_fst_compat.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,31 +36,34 @@
 from neurom.features import neurite as nf
 from neurom.features import morphology as mf
 
 PACKAGE_DIR = Path(__file__).resolve().parent.parent
 
 
 def main():
+    m_h5 = nm.load_morphology(Path(PACKAGE_DIR, "tests/data/h5/v1/bio_neuron-001.h5"))
+    m_asc = nm.load_morphology(Path(PACKAGE_DIR, "tests/data/neurolucida/bio_neuron-001.asc"))
 
-    m_h5 = nm.load_morphology(Path(PACKAGE_DIR, 'tests/data/h5/v1/bio_neuron-001.h5'))
-    m_asc = nm.load_morphology(Path(PACKAGE_DIR, 'tests/data/neurolucida/bio_neuron-001.asc'))
+    print("h5 number of sections:", nm.get("number_of_sections", m_h5))
+    print("nl number of sections:", nm.get("number_of_sections", m_asc))
+    print("h5 number of segments:", nm.get("number_of_segments", m_h5))
+    print("nl number of segments:", nm.get("number_of_segments", m_asc))
+    print("h5 total neurite length:", np.sum(nm.get("section_lengths", m_h5)))
+    print("nl total neurite length:", np.sum(nm.get("section_lengths", m_asc)))
+    print("h5 principal direction extents:", nm.get("principal_direction_extents", m_h5))
+    print("nl principal direction extents:", nm.get("principal_direction_extents", m_asc))
 
-    print('h5 number of sections:', nm.get('number_of_sections', m_h5))
-    print('nl number of sections:', nm.get('number_of_sections', m_asc))
-    print('h5 number of segments:', nm.get('number_of_segments', m_h5))
-    print('nl number of segments:', nm.get('number_of_segments', m_asc))
-    print('h5 total neurite length:', np.sum(nm.get('section_lengths', m_h5)))
-    print('nl total neurite length:', np.sum(nm.get('section_lengths', m_asc)))
-    print('h5 principal direction extents:', nm.get('principal_direction_extents', m_h5))
-    print('nl principal direction extents:', nm.get('principal_direction_extents', m_asc))
-
-    print('\nNumber of neurites:')
+    print("\nNumber of neurites:")
     for nt in iter(nm.NeuriteType):
-        print(nt, mf.number_of_neurites(m_h5, neurite_type=nt), mf.number_of_neurites(m_asc, neurite_type=nt))
+        print(
+            nt,
+            mf.number_of_neurites(m_h5, neurite_type=nt),
+            mf.number_of_neurites(m_asc, neurite_type=nt),
+        )
 
-    print('\nNumber of segments:')
+    print("\nNumber of segments:")
     for nt in iter(nm.NeuriteType):
         print(nt, nf.number_of_segments(m_h5.neurites[0]), nf.number_of_segments(m_asc.neurites[0]))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `neurom-3.2.9/examples/plot_somas.py` & `neurom-4.0.0/examples/plot_somas.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,38 +32,41 @@
 from pathlib import Path
 
 from neurom import load_morphology
 from neurom.view import matplotlib_utils
 import matplotlib.pyplot as plt
 import numpy as np
 
-DATA_PATH = Path(__file__).resolve().parent.parent / 'tests/data/swc'
+DATA_PATH = Path(__file__).resolve().parent.parent / "tests/data/swc"
 
 
 def random_color():
     """Random color generation."""
     return np.random.rand(4)
 
 
 def plot_somas(somas):
     """Plot set of somas on same figure as spheres, each with different color."""
-    _, ax = matplotlib_utils.get_figure(new_fig=True, subplot=111,
-                                        params={'projection': '3d', 'aspect': 'auto'})
+    _, ax = matplotlib_utils.get_figure(
+        new_fig=True, subplot=111, params={"projection": "3d", "aspect": "auto"}
+    )
     for s in somas:
         matplotlib_utils.plot_sphere(ax, s.center, s.radius, color=random_color(), alpha=1)
 
     # uncomment to show
     # plt.show()
 
 
 def main():
     #  define set of files containing relevant morphs
-    file_nms = [Path(DATA_PATH, file_nm) for file_nm in ['Soma_origin.swc',
-                                                                'Soma_translated_1.swc',
-                                                                'Soma_translated_2.swc']]
+    file_nms = [
+        Path(DATA_PATH, file_nm)
+        for file_nm in ["Soma_origin.swc", "Soma_translated_1.swc", "Soma_translated_2.swc"]
+    ]
 
     # load from file and plot
     sms = [load_morphology(file_nm).soma for file_nm in file_nms]
     plot_somas(sms)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
```

### Comparing `neurom-3.2.9/examples/radius_of_gyration.py` & `neurom-4.0.0/examples/radius_of_gyration.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,28 +88,40 @@
 
 def mean_rad_of_gyration(neurites):
     """Calculate mean radius of gyration for set of neurites."""
     return np.mean([radius_of_gyration(n) for n in neurites])
 
 
 def main():
-
     #  load a neuron from an SWC file
-    filename = Path(PACKAGE_DIR, 'tests/data/swc/Neuron.swc')
+    filename = Path(PACKAGE_DIR, "tests/data/swc/Neuron.swc")
     m = nm.load_morphology(filename)
 
     # for every neurite, print (number of segments, radius of gyration, neurite type)
-    print([(sum(len(s.points) - 1 for s in nrte.iter_sections()),
-            radius_of_gyration(nrte), nrte.type) for nrte in m.neurites])
+    print(
+        [
+            (
+                sum(len(s.points) - 1 for s in nrte.sections),
+                radius_of_gyration(nrte),
+                nrte.type,
+            )
+            for nrte in m.neurites
+        ]
+    )
 
     # print mean radius of gyration per neurite type
-    print('Mean radius of gyration for axons: ',
-          mean_rad_of_gyration(n for n in m.neurites if n.type == nm.AXON))
-    print('Mean radius of gyration for basal dendrites: ',
-          mean_rad_of_gyration(n for n in m.neurites if n.type == nm.BASAL_DENDRITE))
-    print('Mean radius of gyration for apical dendrites: ',
-          mean_rad_of_gyration(n for n in m.neurites
-                               if n.type == nm.APICAL_DENDRITE))
+    print(
+        "Mean radius of gyration for axons: ",
+        mean_rad_of_gyration(n for n in m.neurites if n.type == nm.AXON),
+    )
+    print(
+        "Mean radius of gyration for basal dendrites: ",
+        mean_rad_of_gyration(n for n in m.neurites if n.type == nm.BASAL_DENDRITE),
+    )
+    print(
+        "Mean radius of gyration for apical dendrites: ",
+        mean_rad_of_gyration(n for n in m.neurites if n.type == nm.APICAL_DENDRITE),
+    )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `neurom-3.2.9/examples/section_ids.py` & `neurom-4.0.0/examples/section_ids.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,22 +41,21 @@
 def get_segment(neuron, section_id, segment_id):
     """Get a segment given a section and segment id
 
     Returns:
         array of two [x, y, z, r] points defining segment
     """
     sec = neuron.sections[section_id]
-    return sec.points[segment_id:segment_id + 2][:, COLS.XYZR]
+    return sec.points[segment_id : segment_id + 2][:, COLS.XYZR]
 
 
 def main():
-
-    m = nm.load_morphology(Path(PACKAGE_DIR, 'tests/data/h5/v1/Neuron.h5'))
+    m = nm.load_morphology(Path(PACKAGE_DIR, "tests/data/h5/v1/Neuron.h5"))
 
     seg = get_segment(m, 3, 2)
-    print('Segment:\n', seg)
-    print('Mid-point (x, y, z):\n', mm.linear_interpolate(seg[0], seg[1], 0.5))
-    print('Mid-point R:\n', mm.interpolate_radius(seg[0][COLS.R], seg[1][COLS.R], 0.5))
+    print("Segment:\n", seg)
+    print("Mid-point (x, y, z):\n", mm.linear_interpolate(seg[0], seg[1], 0.5))
+    print("Mid-point R:\n", mm.interpolate_radius(seg[0][COLS.R], seg[1][COLS.R], 0.5))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `neurom-3.2.9/examples/soma_radius_fit.py` & `neurom-4.0.0/examples/soma_radius_fit.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,32 +38,33 @@
 
 
 PACKAGE_DIR = Path(__file__).resolve().parent.parent
 
 
 def test_multiple_distr(filepath):
     """Runs the distribution fit for multiple distributions and returns
-       the optimal distribution along with the corresponding parameters.
+    the optimal distribution along with the corresponding parameters.
     """
     #  load a neuron from an SWC file
     population = nm.load_morphologies(filepath)
 
     # Create a list of basic distributions
-    distr_to_check = ('norm', 'expon', 'uniform')
+    distr_to_check = ("norm", "expon", "uniform")
 
     # Get the soma radii of a population of morphs
-    soma_size = nm.get('soma_radius', population)
+    soma_size = nm.get("soma_radius", population)
 
     # Find the best fit distribution
     return st.optimal_distribution(soma_size, distr_to_check)
 
 
 def main():
-
     morphology_path = Path(PACKAGE_DIR, "tests/data/swc/Neuron.swc")
 
     result = test_multiple_distr(morphology_path)
-    print(f"Optimal distribution fit for soma radius is: {result.type} with parameters {result.params}")
+    print(
+        f"Optimal distribution fit for soma radius is: {result.type} with parameters {result.params}"
+    )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `neurom-3.2.9/neurom/__init__.py` & `neurom-4.0.0/neurom/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,21 +51,24 @@
     This example gets the number of points in each axon in a morphology population
 
     >>> import neurom as nm
     >>> filter = lambda n : n.type == nm.AXON
     >>> mapping = lambda n : len(n.points)
     >>> n_points = [n for n in nm.iter_neurites(pop, mapping, filter)]
 """
+from importlib.metadata import version
+
+__version__ = version(__package__)
+
 from neurom.core.dataformat import COLS
-from neurom.core.types import NeuriteType, NeuriteIter, NEURITES as NEURITE_TYPES
 from neurom.core.morphology import graft_morphology, iter_neurites, iter_sections, iter_segments
-
-from neurom.features import get
-from neurom.io.utils import MorphLoader, load_morphology, load_morphologies
-from neurom.io.utils import load_neuron, load_neurons
+from neurom.core.types import NEURITES as NEURITE_TYPES
+from neurom.core.types import NeuriteIter, NeuriteType
 from neurom.exceptions import NeuroMDeprecationWarning
+from neurom.features import get
+from neurom.io.utils import MorphLoader, load_morphologies, load_morphology
 
 APICAL_DENDRITE = NeuriteType.apical_dendrite
 BASAL_DENDRITE = NeuriteType.basal_dendrite
 AXON = NeuriteType.axon
 SOMA = NeuriteType.soma
 ANY_NEURITE = NeuriteType.all
```

### Comparing `neurom-3.2.9/neurom/apps/__init__.py` & `neurom-4.0.0/neurom/apps/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Helper code for neurom applications."""
-import sys
 import logging
+import sys
 from pathlib import Path
+
 import yaml
 
 from neurom.exceptions import ConfigError
 
 if sys.version_info >= (3, 9):  # pragma: no cover
     import importlib.resources as importlib_resources
 else:
```

### Comparing `neurom-3.2.9/neurom/apps/annotate.py` & `neurom-4.0.0/neurom/apps/annotate.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,25 +42,33 @@
 
     Returns:
         An S-expression-like string representing the annotation
     """
     if result.status:
         return ''
 
-    header = ('\n\n'
-              f'({settings["label"]}   ; MUK_ANNOTATION\n'
-              f'    (Color {settings["color"]})   ; MUK_ANNOTATION\n'
-              f'    (Name "{settings["name"]}")   ; MUK_ANNOTATION')
+    header = (
+        '\n\n'
+        f'({settings["label"]}   ; MUK_ANNOTATION\n'
+        f'    (Color {settings["color"]})   ; MUK_ANNOTATION\n'
+        f'    (Name "{settings["name"]}")   ; MUK_ANNOTATION'
+    )
     points = [p for _, _points in result.info for p in _points]
-    annotations = '\n'.join((f'    '
-                             f'({p[COLS.X]:10.2f} {p[COLS.Y]:10.2f} {p[COLS.Z]:10.2f} 0.50)'
-                             f'   ; MUK_ANNOTATION' for p in points))
+    annotations = '\n'.join(
+        (
+            f'    '
+            f'({p[COLS.X]:10.2f} {p[COLS.Y]:10.2f} {p[COLS.Z]:10.2f} 0.50)'
+            f'   ; MUK_ANNOTATION'
+            for p in points
+        )
+    )
     footer = ')   ; MUK_ANNOTATION\n'
 
     return f'{header}\n{annotations}\n{footer}'
 
 
 def annotate(results, settings):
     """Concatenate the annotations of all checkers."""
-    annotations = (generate_annotation(result, setting)
-                   for result, setting in zip(results, settings))
+    annotations = (
+        generate_annotation(result, setting) for result, setting in zip(results, settings)
+    )
     return '\n'.join(annot for annot in annotations if annot)
```

### Comparing `neurom-3.2.9/neurom/apps/cli.py` & `neurom-4.0.0/neurom/apps/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,87 +29,142 @@
 """The morph-tool command line launcher."""
 import logging
 from functools import partial
 
 import click
 import matplotlib.pyplot as plt
 
-from neurom.apps import morph_stats, morph_check, EXAMPLE_CHECK_CONFIG, EXAMPLE_STATS_CONFIG
 from neurom import load_morphology
+from neurom.apps import morph_check, morph_stats
 from neurom.view import matplotlib_impl, matplotlib_utils
 
 
 @click.group()
-@click.option('-v', '--verbose', count=True, default=0,
-              help='-v for WARNING, -vv for INFO, -vvv for DEBUG')
+@click.option(
+    '-v', '--verbose', count=True, default=0, help='-v for WARNING, -vv for INFO, -vvv for DEBUG'
+)
 def cli(verbose):
     """The CLI entry point."""
     level = (logging.WARNING, logging.INFO, logging.DEBUG)[min(verbose, 2)]
     logging.basicConfig(level=level)
 
 
 @cli.command()
 @click.argument('input_file')
 @click.option('--3d', 'is_3d', is_flag=True)
 @click.option('--plane', type=click.Choice(['xy', 'yx', 'yz', 'zy', 'xz', 'zx']), default='xy')
 @click.option('--backend', type=click.Choice(['plotly', 'matplotlib']), default='matplotlib')
-@click.option('-r', '--realistic-diameters/--no-realistic-diameters', default=False,
-              help='Scale diameters according to the plot axis\n'
-                   'Warning: Only works with the matplotlib backend')
+@click.option(
+    '-r',
+    '--realistic-diameters/--no-realistic-diameters',
+    default=False,
+    help='Scale diameters according to the plot axis\n'
+    'Warning: Only works with the matplotlib backend',
+)
 def view(input_file, is_3d, plane, backend, realistic_diameters):
     """CLI interface to draw morphologies."""
     # pylint: disable=import-outside-toplevel
     is_matplotlib = backend == 'matplotlib'
     if is_matplotlib:
         if is_3d:
             _, ax = matplotlib_utils.get_figure(params={'projection': '3d'})
             plot = partial(matplotlib_impl.plot_morph3d, ax=ax)
         else:
             _, ax = matplotlib_utils.get_figure()
-            plot = partial(matplotlib_impl.plot_morph, ax=ax,
-                           plane=plane, realistic_diameters=realistic_diameters)
+            plot = partial(
+                matplotlib_impl.plot_morph,
+                ax=ax,
+                plane=plane,
+                realistic_diameters=realistic_diameters,
+            )
     else:
         from neurom.view import plotly_impl
+
         if is_3d:
             plot = plotly_impl.plot_morph3d
         else:
             plot = partial(plotly_impl.plot_morph, plane=plane)
 
     plot(load_morphology(input_file))
     if is_matplotlib:
         if not is_3d:
             plt.axis('equal')
         plt.show()
 
 
-@cli.command(short_help='Morphology statistics extractor, more details at'
-                        'https://neurom.readthedocs.io/en/latest/morph_stats.html')
+@cli.command(
+    short_help='Morphology statistics extractor, more details at'
+    'https://neurom.readthedocs.io/en/latest/morph_stats.html'
+)
 @click.argument('datapath', required=False)
-@click.option('-C', '--config', type=click.Path(exists=True, dir_okay=False),
-              default=EXAMPLE_STATS_CONFIG, show_default=True,
-              help='Configuration File')
-@click.option('-o', '--output', type=click.Path(exists=False, dir_okay=False),
-              help='Path to output file, if it ends in .json, a json file is created,'
-                   'otherwise a csv file is created')
-@click.option('-f', '--full-config', is_flag=True, default=False,
-              help='If passed then --config is ignored. Compute statistics for all neurite'
-                   'types, all modes and all features')
-@click.option('--as-population', is_flag=True, default=False,
-              help='If enabled the directory is treated as a population')
-@click.option('-I', '--ignored-exceptions', help='Exception to ignore',
-              type=click.Choice(morph_stats.IGNORABLE_EXCEPTIONS.keys()))
-def stats(datapath, config, output, full_config, as_population, ignored_exceptions):
+@click.option(
+    '-C',
+    '--config',
+    type=click.Path(exists=True, dir_okay=False),
+    default=morph_stats.EXAMPLE_STATS_CONFIG,
+    show_default=True,
+    help='Configuration File',
+)
+@click.option(
+    '-o',
+    '--output',
+    type=click.Path(exists=False, dir_okay=False),
+    help='Path to output file, if it ends in .json, a json file is created,'
+    'otherwise a csv file is created',
+)
+@click.option(
+    '-f',
+    '--full-config',
+    is_flag=True,
+    default=False,
+    help='If passed then --config is ignored. Compute statistics for all neurite'
+    'types, all modes and all features',
+)
+@click.option(
+    '--as-population',
+    is_flag=True,
+    default=False,
+    help='If enabled the directory is treated as a population',
+)
+@click.option(
+    '-I',
+    '--ignored-exceptions',
+    help='Exception to ignore',
+    type=click.Choice(morph_stats.IGNORABLE_EXCEPTIONS.keys()),
+)
+@click.option(
+    '--use-subtrees',
+    is_flag=True,
+    show_default=True,
+    default=False,
+    help="Enable mixed subtree processing.",
+)
+def stats(datapath, config, output, full_config, as_population, ignored_exceptions, use_subtrees):
     """Cli for apps/morph_stats."""
-    morph_stats.main(datapath, config, output, full_config, as_population, ignored_exceptions)
+    morph_stats.main(
+        datapath, config, output, full_config, as_population, ignored_exceptions, use_subtrees
+    )
 
 
-@cli.command(short_help='Perform checks on morphologies, more details at'
-                        'https://neurom.readthedocs.io/en/latest/morph_check.html')
+@cli.command(
+    short_help='Perform checks on morphologies, more details at'
+    'https://neurom.readthedocs.io/en/latest/morph_check.html'
+)
 @click.argument('datapath')
-@click.option('-C', '--config', type=click.Path(exists=True, dir_okay=False),
-              default=EXAMPLE_CHECK_CONFIG, show_default=True,
-              help='Configuration File')
-@click.option('-o', '--output', type=click.Path(exists=False, dir_okay=False),
-              help='Path to output json summary file', required=True)
+@click.option(
+    '-C',
+    '--config',
+    type=click.Path(exists=True, dir_okay=False),
+    default=morph_check.EXAMPLE_CHECK_CONFIG,
+    show_default=True,
+    help='Configuration File',
+)
+@click.option(
+    '-o',
+    '--output',
+    type=click.Path(exists=False, dir_okay=False),
+    help='Path to output json summary file',
+    required=True,
+)
 def check(datapath, config, output):
     """Cli for apps/morph_check."""
     morph_check.main(datapath, config, output)
```

### Comparing `neurom-3.2.9/neurom/apps/config/morph_check.yaml` & `neurom-4.0.0/neurom/apps/config/morph_check.yaml`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/neurom/apps/morph_check.py` & `neurom-4.0.0/neurom/apps/morph_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Check on morphologies."""
 
 import json
-from neurom.apps import get_config, EXAMPLE_CHECK_CONFIG
+
+from neurom.apps import EXAMPLE_CHECK_CONFIG, get_config
 from neurom.check.runner import CheckRunner
 
 
 def main(datapath, config, output):
     """Main function that checks morphologies.
 
     Args:
```

### Comparing `neurom-3.2.9/neurom/apps/morph_stats.py` & `neurom-4.0.0/neurom/apps/morph_stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,36 +40,40 @@
 from functools import partial
 
 import numpy as np
 import pandas as pd
 from morphio import SomaError
 
 import neurom as nm
-from neurom.apps import get_config, EXAMPLE_STATS_CONFIG
+from neurom.apps import EXAMPLE_STATS_CONFIG, get_config
 from neurom.core.morphology import Morphology, Neurite
 from neurom.core.population import Population
 from neurom.exceptions import ConfigError
-from neurom.features import _NEURITE_FEATURES, _MORPHOLOGY_FEATURES, _POPULATION_FEATURES, \
-    _get_feature_value_and_func
+from neurom.features import (
+    _MORPHOLOGY_FEATURES,
+    _NEURITE_FEATURES,
+    _POPULATION_FEATURES,
+    _get_feature_value_and_func,
+)
 from neurom.io.utils import get_files_by_path
-from neurom.utils import flatten, NeuromJSON
+from neurom.utils import NeuromJSON, flatten
 
 L = logging.getLogger(__name__)
 
 IGNORABLE_EXCEPTIONS = {'SomaError': SomaError}
 
 
-def _run_extract_stats(morph, config):
+def _run_extract_stats(morph, config, process_subtrees):
     """The function to be called by multiprocessing.Pool.imap_unordered."""
     if not isinstance(morph, (Morphology, Population)):
-        morph = nm.load_morphologies(morph)
+        morph = nm.load_morphologies(morph, process_subtrees=process_subtrees)
     return morph.name, extract_stats(morph, config)
 
 
-def extract_dataframe(morphs, config, n_workers=1):
+def extract_dataframe(morphs, config, n_workers=1, process_subtrees=False):
     """Extract stats grouped by neurite type from morphs.
 
     Arguments:
         morphs: a morphology, population, neurite tree, list of populations or list of morphology
             paths
         config (dict): configuration dict. The keys are:
             - neurite_type: a list of neurite types for which features are extracted
@@ -92,42 +96,45 @@
 
     """
     if isinstance(morphs, Morphology):
         morphs = [morphs]
     elif isinstance(morphs, Population):
         morphs = morphs._files  # pylint: disable=protected-access
 
-    func = partial(_run_extract_stats, config=config)
+    func = partial(_run_extract_stats, config=config, process_subtrees=process_subtrees)
     if n_workers == 1:
         stats = list(map(func, morphs))
     else:
         if any(isinstance(i, Morphology) for i in morphs):
             raise ValueError("Can only process morphologies given as file paths when n_workers > 1")
         if n_workers > os.cpu_count():
             warnings.warn(f'n_workers ({n_workers}) > os.cpu_count() ({os.cpu_count()}))')
         with multiprocessing.Pool(n_workers) as pool:
             stats = list(pool.imap(func, morphs))
 
     columns = [('property', 'name')] + [
         (key1, key2) for key1, data in stats[0][1].items() for key2 in data
     ]
-    rows = [[name] + list(flatten(features.values() for features in data.values()))
-            for name, data in stats]
+    rows = [
+        [name] + list(flatten(features.values() for features in data.values()))
+        for name, data in stats
+    ]
     return pd.DataFrame(columns=pd.MultiIndex.from_tuples(columns), data=rows)
 
 
 extract_dataframe.__doc__ = extract_dataframe.__doc__.strip() + "\n\t" + str(EXAMPLE_STATS_CONFIG)
 
 
-def _get_feature_stats(feature_name, morphs, modes, kwargs):
+def _get_feature_stats(feature_name, morphs, modes, **kwargs):
     """Insert the stat data in the dict.
 
     If the feature is 2-dimensional, the feature is flattened on its last axis
     """
-    def stat_name_format(mode, feature_name, kwargs):
+
+    def stat_name_format(mode, feature_name, **kwargs):
         """Returns the key name for the data dictionary.
 
         The key is a combination of the mode, feature_name and an optional suffix of all the extra
         kwargs that are passed in the feature function (apart from neurite_type).
         """
         suffix = "__".join(
             [f"{key}:{value}" for key, value in kwargs.items() if key != "neurite_type"]
@@ -141,16 +148,15 @@
     data = {}
     value, func = _get_feature_value_and_func(feature_name, morphs, **kwargs)
     shape = func.shape
     if len(shape) > 2:
         raise ValueError(f'Len of "{feature_name}" feature shape must be <= 2')  # pragma: no cover
 
     for mode in modes:
-
-        stat_name = stat_name_format(mode, feature_name, kwargs)
+        stat_name = stat_name_format(mode, feature_name, **kwargs)
 
         stat = value
         if isinstance(value, Sized):
             if len(value) == 0 and mode not in {'raw', 'sum'}:
                 stat = None
             elif mode == 'raw':
                 stat = value
@@ -196,58 +202,56 @@
     config = _sanitize_config(config)
 
     neurite_types = [_NEURITE_MAP[t] for t in config.get('neurite_type', _NEURITE_MAP.keys())]
 
     stats = defaultdict(dict)
     for category in ("neurite", "morphology", "population"):
         for feature_name, opts in config[category].items():
-
             list_of_kwargs = opts["kwargs"]
             modes = opts["modes"]
 
             for feature_kwargs in list_of_kwargs:
-
                 if category == 'neurite':
-
                     # mutated below, need a copy
                     feature_kwargs = deepcopy(feature_kwargs)
 
                     types = (
                         neurite_types
                         if 'neurite_type' not in feature_kwargs and neurite_types
                         else [_NEURITE_MAP[feature_kwargs.get('neurite_type', 'ALL')]]
                     )
 
                     for neurite_type in types:
                         if not isinstance(morphs, Neurite):
                             feature_kwargs["neurite_type"] = neurite_type
                         stats[neurite_type.name].update(
-                            _get_feature_stats(feature_name, morphs, modes, feature_kwargs)
+                            _get_feature_stats(
+                                feature_name,
+                                morphs,
+                                modes,
+                                **feature_kwargs,
+                            )
                         )
 
                 else:
                     stats[category].update(
-                        _get_feature_stats(feature_name, morphs, modes, feature_kwargs)
+                        _get_feature_stats(feature_name, morphs, modes, **feature_kwargs)
                     )
 
     return dict(stats)
 
 
 extract_stats.__doc__ = extract_stats.__doc__.strip() + "\n\t" + str(EXAMPLE_STATS_CONFIG)
 
 
 def _get_header(results):
     """Extracts the headers, using the first value in the dict as the template."""
     values = next(iter(results.values()))
 
-    return ['name'] + [
-        f'{k}:{metric}'
-        for k, v in values.items()
-        for metric in v.keys()
-    ]
+    return ['name'] + [f'{k}:{metric}' for k, v in values.items() for metric in v.keys()]
 
 
 def _generate_flattened_dict(headers, results):
     """Extract from results the fields in the headers list."""
     for name, values in results.items():
         row = []
         for header in headers:
@@ -261,26 +265,26 @@
         yield row
 
 
 _NEURITE_MAP = {
     'AXON': nm.AXON,
     'BASAL_DENDRITE': nm.BASAL_DENDRITE,
     'APICAL_DENDRITE': nm.APICAL_DENDRITE,
-    'ALL': nm.ANY_NEURITE
+    'ALL': nm.ANY_NEURITE,
 }
 
 
 def full_config():
     """Returns a config with all features, all modes, all neurite types."""
     modes = ['min', 'max', 'median', 'mean', 'std']
 
     categories = {
         "neurite": _NEURITE_FEATURES,
         "morphology": _MORPHOLOGY_FEATURES,
-        "population": _POPULATION_FEATURES
+        "population": _POPULATION_FEATURES,
     }
 
     config = {
         category: {name: {"kwargs": [{}], "modes": modes} for name in features}
         for category, features in categories.items()
     }
 
@@ -314,14 +318,15 @@
                 kwargs:
                   - kwargs1
                   - kwargs2
                 modes:
                   - mode1
                   - mode2
     """
+
     def standardize_options(options):
         """Returns options as a dict with two keys: 'kwargs' and 'modes'."""
         # convert short format
         if isinstance(options, list):
             return {"kwargs": [{}], "modes": options}
 
         modes = options.get("modes", [])
@@ -349,38 +354,48 @@
 
     for category in ("neurite", "morphology", "population"):
         config[category] = _standardize_layout(config[category]) if category in config else {}
 
     return config
 
 
-def main(datapath, config, output_file, is_full_config, as_population, ignored_exceptions):
+def main(
+    datapath,
+    config,
+    output_file,
+    is_full_config,
+    as_population,
+    ignored_exceptions,
+    use_subtrees=False,
+):
     """Main function that get statistics for morphologies.
 
     Args:
         datapath (str|Path): path to a morphology file or folder
         config (str|Path): path to a statistics config file
         output_file (str|Path): path to output the resulted statistics file
         is_full_config (bool): should be statistics made over all possible features, modes, neurites
         as_population (bool): treat ``datapath`` as directory of morphologies population
         ignored_exceptions (list|tuple|None): exceptions to ignore when loading a morphology
+        use_subtrees (bool): Enable of heterogeneous subtree processing
     """
     config = full_config() if is_full_config else get_config(config, EXAMPLE_STATS_CONFIG)
 
     if 'neurite' in config and 'neurite_type' not in config:
         error = ConfigError('"neurite_type" missing from config, but "neurite" set')
         L.error(error)
         raise error
 
     if ignored_exceptions is None:
         ignored_exceptions = ()
 
     morphs = nm.load_morphologies(
         get_files_by_path(datapath),
-        ignored_exceptions=tuple(IGNORABLE_EXCEPTIONS[k] for k in ignored_exceptions)
+        ignored_exceptions=tuple(IGNORABLE_EXCEPTIONS[k] for k in ignored_exceptions),
+        process_subtrees=use_subtrees,
     )
 
     if as_population:
         results = {datapath: extract_stats(morphs, config)}
     else:
         results = {m.name: extract_stats(m, config) for m in morphs}
```

### Comparing `neurom-3.2.9/neurom/check/__init__.py` & `neurom-4.0.0/neurom/check/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,27 +29,29 @@
 """Basic tools to check morphologies."""
 
 from functools import wraps
 
 
 def check_wrapper(fun):
     """Decorate a checking function."""
+
     @wraps(fun)
     def _wrapper(*args, **kwargs):
         """Sets the title property of the result of running a checker."""
         title = fun.__name__.replace('_', ' ').capitalize()
         result = fun(*args, **kwargs)
         result.title = title
         return result
 
     return _wrapper
 
 
 class CheckResult:
     """Class representing a check result."""
+
     def __init__(self, status, info=None, title=None):
         """Initialize a CheckResult object."""
         self.status = bool(status)
         self.info = info
         self.title = title
 
     def __nonzero__(self):
```

### Comparing `neurom-3.2.9/neurom/check/morphology_checks.py` & `neurom-4.0.0/neurom/check/morphology_checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,20 @@
 """NeuroM morphology checking functions.
 
 Contains functions for checking validity of morphology neurites and somata.
 """
 from itertools import islice
 
 import numpy as np
+
 from neurom import NeuriteType
 from neurom.check import CheckResult
-from neurom.check.morphtree import get_flat_neurites, back_tracking_segments
-from neurom.core.morphology import Section, iter_neurites, iter_sections, iter_segments
+from neurom.check.morphtree import back_tracking_segments, get_flat_neurites, overlapping_points
 from neurom.core.dataformat import COLS
+from neurom.core.morphology import Section, iter_neurites, iter_sections, iter_segments
 from neurom.exceptions import NeuroMError
 from neurom.morphmath import section_length, segment_length
 from neurom.utils import flatten
 
 
 def _read_neurite_type(neurite):
     """Simply read the stored neurite type."""
@@ -133,16 +134,15 @@
     Arguments:
         morph(Morphology): the morphology to test
         threshold(float): value above which a section length is considered to be non-zero
 
     Returns:
         CheckResult with result including list of ids of bad sections
     """
-    bad_ids = [s.id for s in iter_sections(morph.neurites)
-               if section_length(s.points) <= threshold]
+    bad_ids = [s.id for s in iter_sections(morph.neurites) if section_length(s.points) <= threshold]
 
     return CheckResult(len(bad_ids) == 0, bad_ids)
 
 
 def has_all_nonzero_neurite_radii(morph, threshold=0.0):
     """Check presence of neurite points with radius not above threshold.
 
@@ -188,18 +188,23 @@
         considered a jump
         axis(str): one of x/y/z, which axis to check for jumps
 
     Returns:
         CheckResult with result list of ids of bad sections
     """
     bad_ids = []
-    axis = {'x': COLS.X, 'y': COLS.Y, 'z': COLS.Z, }[axis.lower()]
+    axis = {
+        'x': COLS.X,
+        'y': COLS.Y,
+        'z': COLS.Z,
+    }[axis.lower()]
     for neurite in iter_neurites(morph):
-        section_segment = ((sec, seg) for sec in iter_sections(neurite)
-                           for seg in iter_segments(sec))
+        section_segment = (
+            (sec, seg) for sec in iter_sections(neurite) for seg in iter_segments(sec)
+        )
         for sec, (p0, p1) in islice(section_segment, 1, None):  # Skip neurite root segment
             if max_distance < abs(p0[axis] - p1[axis]):
                 bad_ids.append((sec.id, [p0, p1]))
     return CheckResult(len(bad_ids) == 0, bad_ids)
 
 
 def has_no_root_node_jumps(morph, radius_multiplier=2):
@@ -250,17 +255,19 @@
     Arguments:
         morph(Morphology): the morphology to test
         frac(float): Ratio that the second point must be smaller than the first
 
     Returns:
         CheckResult with a list of all first segments of neurites with a narrow start
     """
-    bad_ids = [(neurite.root_node.id, neurite.root_node.points[np.newaxis, 1])
-               for neurite in morph.neurites
-               if neurite.root_node.points[0][COLS.R] < frac * neurite.root_node.points[1][COLS.R]]
+    bad_ids = [
+        (neurite.root_node.id, neurite.root_node.points[np.newaxis, 1])
+        for neurite in morph.neurites
+        if neurite.root_node.points[0][COLS.R] < frac * neurite.root_node.points[1][COLS.R]
+    ]
     return CheckResult(len(bad_ids) == 0, bad_ids)
 
 
 def has_no_dangling_branch(morph):
     """Check if the morphology has dangling neurites.
 
     Are considered dangling
@@ -278,70 +285,80 @@
     if len(morph.soma.points) == 0:
         raise NeuroMError("Can't check for dangling neurites if there is no soma")
     soma_center = morph.soma.points[:, COLS.XYZ].mean(axis=0)
     recentered_soma = morph.soma.points[:, COLS.XYZ] - soma_center
     radius = np.linalg.norm(recentered_soma, axis=1)
     soma_max_radius = radius.max()
 
-    dendritic_points = np.array(list(flatten(n.points
-                                             for n in iter_neurites(morph)
-                                             if n.type != NeuriteType.axon)))
+    dendritic_points = np.array(
+        list(flatten(n.points for n in iter_neurites(morph) if n.type != NeuriteType.axon))
+    )
 
     def is_dangling(neurite):
         """Is the neurite dangling?"""
         starting_point = neurite.points[0][COLS.XYZ]
 
-        if np.linalg.norm(starting_point - soma_center) - soma_max_radius <= 12.:
+        if np.linalg.norm(starting_point - soma_center) - soma_max_radius <= 12.0:
             return False
 
         if neurite.type != NeuriteType.axon:
             return True
 
-        distance_to_dendrites = np.linalg.norm(dendritic_points[:, COLS.XYZ] - starting_point,
-                                               axis=1)
+        distance_to_dendrites = np.linalg.norm(
+            dendritic_points[:, COLS.XYZ] - starting_point, axis=1
+        )
         return np.all(distance_to_dendrites >= 2 * dendritic_points[:, COLS.R] + 2)
 
-    bad_ids = [(n.root_node.id, [n.root_node.points[0]])
-               for n in iter_neurites(morph) if is_dangling(n)]
+    bad_ids = [
+        (n.root_node.id, [n.root_node.points[0]]) for n in iter_neurites(morph) if is_dangling(n)
+    ]
     return CheckResult(len(bad_ids) == 0, bad_ids)
 
 
-def has_no_narrow_neurite_section(morph,
-                                  neurite_filter,
-                                  radius_threshold=0.05,
-                                  considered_section_min_length=50):
+def has_no_narrow_neurite_section(
+    morph, neurite_filter, radius_threshold=0.05, considered_section_min_length=50
+):
     """Check if the morphology has dendrites with narrow sections.
 
     Arguments:
         morph(Morphology): the morphology to test
         neurite_filter(callable): filter the neurites by this callable
         radius_threshold(float): radii below this are considered narro
         considered_section_min_length(float): sections with length below
         this are not taken into account
 
     Returns:
         CheckResult with result. `result.info` contains the narrow section ids and their
         first point
     """
-    considered_sections = (sec for sec in iter_sections(morph, neurite_filter=neurite_filter)
-                           if sec.length > considered_section_min_length)
+    considered_sections = (
+        sec
+        for sec in iter_sections(morph, neurite_filter=neurite_filter)
+        if sec.length > considered_section_min_length
+    )
 
     def narrow_section(section):
         """Select narrow sections."""
         return section.points[:, COLS.R].mean() < radius_threshold
 
-    bad_ids = [(section.id, section.points[np.newaxis, 1])
-               for section in considered_sections if narrow_section(section)]
+    bad_ids = [
+        (section.id, section.points[np.newaxis, 1])
+        for section in considered_sections
+        if narrow_section(section)
+    ]
     return CheckResult(len(bad_ids) == 0, bad_ids)
 
 
 def has_multifurcation(morph):
     """Check if a section has more than 3 children."""
-    bad_ids = [(section.id, section.points[np.newaxis, -1]) for section in iter_sections(morph)
-               if len(section.children) > 3]
+    bad_ids = [
+        (section.id, section.points[np.newaxis, -1])
+        for section in iter_sections(morph)
+        if len(section.children) > 3
+    ]
     return CheckResult(len(bad_ids) == 0, bad_ids)
 
 
 def has_unifurcation(neuron):
     """Check if a section has 1 child."""
     bad_ids = [
         (section.id, section.points[np.newaxis, -1])
@@ -356,12 +373,27 @@
     bad_ids = [section.id for section in iter_sections(morph) if len(section.children) == 1]
     return CheckResult(len(bad_ids) == 0, bad_ids)
 
 
 def has_no_back_tracking(morph):
     """Check if the morphology has sections with back-tracks."""
     bad_ids = [
-        (i, morph.section(i[0]).points[np.newaxis, i[1]])
+        (i, morph.section(i[0]).points[:, COLS.XYZ][np.newaxis, i[1]])
         for neurite in iter_neurites(morph)
         for i in back_tracking_segments(neurite)
     ]
     return CheckResult(len(bad_ids) == 0, bad_ids)
+
+
+def has_no_overlapping_point(morph, tolerance=None):
+    """Check if the morphology has overlapping points.
+
+    Returns:
+        CheckResult with result. `result.info` contains a tuple with the two overlapping section ids
+        and a list containing only the first overlapping points.
+    """
+    bad_ids = [
+        (i[:2], np.atleast_2d(i[2]))
+        for neurite in iter_neurites(morph)
+        for i in overlapping_points(neurite, tolerance=tolerance)
+    ]
+    return CheckResult(len(bad_ids) == 0, bad_ids)
```

### Comparing `neurom-3.2.9/neurom/check/morphtree.py` & `neurom-4.0.0/neurom/check/morphtree.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,16 +25,19 @@
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Python module of NeuroM to check morphology trees."""
 
 import numpy as np
-from neurom.core.dataformat import COLS
+from scipy.spatial import KDTree
+
 from neurom import morphmath as mm
+from neurom.core.dataformat import COLS
+from neurom.core.morphology import iter_sections
 from neurom.morphmath import principal_direction_extent
 
 
 def is_monotonic(neurite, tol):
     """Check if neurite tree is monotonic.
 
     If each child has smaller or equal diameters from its parent
@@ -42,23 +45,22 @@
     Args:
         neurite(Neurite): neurite to operate on
         tol(float): tolerance
 
     Returns:
         True if neurite monotonic
     """
-    for node in neurite.iter_sections():
+    for node in iter_sections(neurite):
         # check that points in section satisfy monotonicity
         sec = node.points
         for point_id in range(len(sec) - 1):
             if sec[point_id + 1][COLS.R] > sec[point_id][COLS.R] + tol:
                 return False
         # Check that section boundary points satisfy monotonicity
-        if (node.parent is not None and
-           sec[0][COLS.R] > node.parent.points[-1][COLS.R] + tol):
+        if node.parent is not None and sec[0][COLS.R] > node.parent.points[-1][COLS.R] + tol:
             return False
 
     return True
 
 
 def is_flat(neurite, tol, method='tolerance'):
     """Check if neurite is flat using the given method.
@@ -80,30 +82,30 @@
     assert method in ('tolerance', 'ratio'), "Method must be one of 'tolerance', 'ratio'"
     if method == 'ratio':
         sorted_ext = np.sort(ext)
         return sorted_ext[0] / sorted_ext[1] < float(tol)
     return any(ext < float(tol))
 
 
-def back_tracking_segments(neurite):
+def back_tracking_segments(neurite):  # pylint: disable=too-many-locals
     """Check if a neurite process backtracks to a previous node.
 
     Back-tracking takes place
     when a daughter of a branching process goes back and either overlaps with a previous point, or
     lies inside the cylindrical volume of the latter.
 
     Args:
         neurite(Neurite): neurite to operate on
 
     Returns:
         A generator of tuples containing the section ID and the two segment indices in this section
         for which a back tracking is detected (so the first point of these segments can be
         retrieved with ``morph.section(section_id).points[segment_id]``.
     """
-    # pylint: disable=too-many-locals
+
     def pair(segs):
         """Pairs the input list into triplets."""
         return zip(segs, segs[1:])
 
     def coords(node):
         """Returns the first three values of the tree that correspond to the x, y, z coordinates."""
         return node[COLS.XYZ]
@@ -167,24 +169,24 @@
         Two conditions must be satisfied:
             1. The two segments are not facing the same direction  (seg2 comes back to seg1)
             2. seg2 is overlaping with seg1
         """
         return not is_in_the_same_verse(seg1, seg2) and is_seg1_overlapping_with_seg2(seg1, seg2)
 
     # filter out single segment sections
-    section_itr = (sec for sec in neurite.iter_sections() if sec.points.shape[0] > 2)
+    section_itr = (sec for sec in iter_sections(neurite) if sec.points.shape[0] > 2)
     for sec in section_itr:
         # group each section's points intro triplets
         segment_pairs = list(filter(is_not_zero_seg, pair(sec.points)))
 
         # filter out zero length segments
         for i, seg1 in enumerate(segment_pairs[1:]):
             # check if the end point of the segment lies within the previous
             # ones in the current section
-            for j, seg2 in enumerate(segment_pairs[0: i + 1]):
+            for j, seg2 in enumerate(segment_pairs[0 : i + 1]):
                 if is_inside_cylinder(seg1, seg2):
                     yield (sec.id, i, j)
 
 
 def is_back_tracking(neurite):
     """Check if a neurite process backtracks to a previous node.
 
@@ -200,14 +202,72 @@
     """
     for _i in back_tracking_segments(neurite):
         # If one segment is found then the neurite is back tracking
         return True
     return False
 
 
+def overlapping_points(neurite, tolerance=None):
+    """Return overlapping points of a neurite.
+
+    Args:
+        neurite(Neurite): neurite to operate on
+        tolerance(float): the tolerance used to find overlapping points
+
+    Returns:
+        A generator of tuples containing the IDs of the two intersecting sections and the
+        overlapping point.
+    """
+    # Create an array containing all the points of the neurite with 1st and last points of each
+    # section deduplicated. This array has 4 columns: the section ID of the point and the
+    # XYZ coordinates.
+    # Note: The section ID is cast to float in this operation and cast back to int later.
+    section_pts = np.vstack(
+        [
+            np.insert(neurite.root_node.points[0, :3], 0, neurite.root_node.id),
+            np.vstack(
+                [
+                    np.concatenate(
+                        [np.ones((len(sec.points) - 1, 1)) * sec.id, sec.points[1:, :3]],
+                        axis=1,
+                    )
+                    for sec in iter_sections(neurite)
+                ],
+            ),
+        ],
+    )
+    tree = KDTree(section_pts[:, 1:4])
+    if tolerance is None:
+        tolerance = 0
+    for pt_id1, pt_id2 in tree.query_pairs(tolerance):
+        yield (
+            int(section_pts[pt_id1, 0]),  # Cast the first section ID back to int
+            int(section_pts[pt_id2, 0]),  # Cast the second section ID back to int
+            section_pts[pt_id1, 1:4],  # The overlapping point of the first section
+        )
+
+
+def has_overlapping_points(neurite, tolerance=None):
+    """Check if a neurite has at least one overlapping point.
+
+    See overlapping_points() for more details.
+
+    Args:
+        neurite(Neurite): neurite to operate on
+        tolerance(float): the tolerance used to find overlapping points
+
+    Returns:
+        True if two points of the neurite are overlapping.
+    """
+    for _i in overlapping_points(neurite, tolerance=tolerance):
+        # If one overlapping point is found then the neurite is overlapping
+        return True
+    return False
+
+
 def get_flat_neurites(morph, tol=0.1, method='ratio'):
     """Check if a morphology has neurites that are flat within a tolerance.
 
     Args:
         morph(Morphology): morphology to operate on
         tol(float): the tolerance or the ratio
         method(string): 'tolerance' or 'ratio' described in :meth:`is_flat`
@@ -242,7 +302,19 @@
     Args:
         morph(Morphology): neurite to operate on
 
     Returns:
         List of morphologies with backtracks
     """
     return [n for n in morph.neurites if is_back_tracking(n)]
+
+
+def get_overlapping_point_neurites(morph, tolerance=0):
+    """Get neurites that have overlapping points.
+
+    Args:
+        morph(Morphology): neurite to operate on
+
+    Returns:
+        List of morphologies with backtracks
+    """
+    return [n for n in morph.neurites if has_overlapping_points(n, tolerance=tolerance)]
```

### Comparing `neurom-3.2.9/neurom/check/runner.py` & `neurom-4.0.0/neurom/check/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 
 import logging
 from collections import OrderedDict
 from importlib import import_module
 
 from neurom import load_morphology
 from neurom.check import check_wrapper
-from neurom.exceptions import ConfigError
+from neurom.exceptions import ConfigError, NeuroMError
 from neurom.io import utils
-from neurom.utils import warn_deprecated
 
 L = logging.getLogger(__name__)
 
 
 class CheckRunner:
     """Class managing checks, config and output."""
 
     def __init__(self, config):
         """Initialize a CheckRunner object."""
         self._config = CheckRunner._sanitize_config(config)
-        self._check_modules = dict((k, import_module('neurom.check.%s' % k))
-                                   for k in config['checks'])
+        self._check_modules = dict(
+            (k, import_module('neurom.check.%s' % k)) for k in config['checks']
+        )
 
     def run(self, path):
         """Test a bunch of files and return a summary JSON report."""
         SEPARATOR = '=' * 40
         summary = {}
         res = True
 
@@ -79,16 +79,15 @@
             else:
                 out = check_wrapper(getattr(check_module, check_str))(obj, fargs)
         else:
             out = check_wrapper(getattr(check_module, check_str))(obj)
 
         try:
             if out.info:
-                L.debug('%s: %d failing ids detected: %s',
-                        out.title, len(out.info), out.info)
+                L.debug('%s: %d failing ids detected: %s', out.title, len(out.info), out.info)
         except TypeError:  # pragma: no cover
             pass
 
         return out
 
     def _check_loop(self, obj, check_mod_str):
         """Run all the checks in a check_module."""
@@ -132,28 +131,27 @@
             CGREEN, CRED, CEND = '\033[92m', '\033[91m', '\033[0m'
         else:
             CGREEN = CRED = CEND = ''
 
         LOG_LEVELS = {False: logging.ERROR, True: logging.INFO}
 
         # pylint: disable=logging-not-lazy
-        L.log(LOG_LEVELS[ok],
-              '%35s %s' + CEND, msg, CGREEN + 'PASS' if ok else CRED + 'FAIL')
+        L.log(LOG_LEVELS[ok], '%35s %s' + CEND, msg, CGREEN + 'PASS' if ok else CRED + 'FAIL')
 
     @staticmethod
     def _sanitize_config(config):
         """Check that the config has the correct keys, add missing keys if necessary."""
         if 'checks' in config:
             checks = config['checks']
             if 'morphology_checks' not in checks:
                 checks['morphology_checks'] = []
-            if 'neuron_checks' in checks:
-                warn_deprecated('"neuron_checks" is deprecated, use "morphology_checks" instead '
-                                'for the config of `neurom.check`')  # pragma: no cover
-                checks['morphology_checks'] = config['neuron_checks']  # pragma: no cover
+            if 'neuron_checks' in checks:  # pragma: no cover
+                raise NeuroMError(
+                    "'neuron_checks' is not supported. Please rename it into 'morphology_checks'"
+                )
         else:
             raise ConfigError('Need to have "checks" in the config')
 
         if 'options' not in config:
             L.debug('Using default options')
             config['options'] = {}
```

### Comparing `neurom-3.2.9/neurom/core/__init__.py` & `neurom-4.0.0/neurom/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,11 +24,12 @@
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Core functionality and data types of NeuroM."""
 
+from neurom.core.morphology import Morphology, Neurite, Section
+from neurom.core.population import Population
+
 # those imports here for backward compatibility
 from neurom.core.soma import Soma
-from neurom.core.morphology import Section, Neurite, Morphology, Neuron
-from neurom.core.population import Population
```

### Comparing `neurom-3.2.9/neurom/core/dataformat.py` & `neurom-4.0.0/neurom/core/dataformat.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from collections import namedtuple
 
 _COL_COUNT = 4
 
 
 class COLS:
     """Column labels for internal data representation."""
+
     COL_COUNT = _COL_COUNT
     (X, Y, Z, R) = range(_COL_COUNT)
     XY = slice(0, 2)
     XZ = slice(0, 3, 2)
     YZ = slice(1, 3)
     XYZ = slice(0, 3)
     XYZR = slice(0, 4)
```

### Comparing `neurom-3.2.9/neurom/core/morphology.py` & `neurom-4.0.0/neurom/core/morphology.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,60 +24,59 @@
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Morphology classes and functions."""
 
-from collections import deque
 import warnings
+from collections import deque
 
 import morphio
 import numpy as np
+from cached_property import cached_property
+
 from neurom import morphmath
-from neurom.core.soma import make_soma
 from neurom.core.dataformat import COLS
-from neurom.core.types import NeuriteIter, NeuriteType
 from neurom.core.population import Population
-from neurom.utils import flatten, warn_deprecated
+from neurom.core.soma import make_soma
+from neurom.core.types import NeuriteIter, NeuriteType
+from neurom.exceptions import NeuroMError
+from neurom.utils import flatten
 
 
 class Section:
     """Simple recursive tree class."""
 
     def __init__(self, morphio_section):
         """The section constructor."""
-        self.morphio_section = morphio_section
+        self._morphio_section = morphio_section
+
+    def to_morphio(self):
+        """Returns the morphio section."""
+        return self._morphio_section
 
     @property
     def id(self):
         """Returns the section ID."""
-        return self.morphio_section.id
+        return self._morphio_section.id
 
     @property
     def parent(self):
         """Returns the parent section if non root section else None."""
-        if self.morphio_section.is_root:
-            return None
-        return Section(self.morphio_section.parent)
+        return None if self.is_root() else Section(self._morphio_section.parent)
 
     @property
     def children(self):
         """Returns a list of child section."""
-        return [Section(child) for child in self.morphio_section.children]
+        return [Section(child) for child in self._morphio_section.children]
 
-    def append_section(self, section):
-        """Appends a section to the current section object.
-
-        Args:
-            section (morphio.Section|morphio.mut.Section|Section|morphio.PointLevel): a section
-        """
-        if isinstance(section, Section):
-            return self.morphio_section.append_section(section.morphio_section)
-        return self.morphio_section.append_section(section)
+    def is_homogeneous_point(self):
+        """A section is homogeneous if it has the same type with its children."""
+        return all(c.type == self.type for c in self.children)
 
     def is_forking_point(self):
         """Is this section a forking point?"""
         return len(self.children) > 1
 
     def is_bifurcation_point(self):
         """Is tree a bifurcation point?"""
@@ -85,43 +84,60 @@
 
     def is_leaf(self):
         """Is tree a leaf?"""
         return len(self.children) == 0
 
     def is_root(self):
         """Is tree the root node?"""
-        return self.parent is None
+        return self._morphio_section.is_root
 
     def ipreorder(self):
         """Depth-first pre-order iteration of tree nodes."""
-        children = deque((self, ))
+        children = deque((self,))
         while children:
             cur_node = children.pop()
             children.extend(reversed(cur_node.children))
             yield cur_node
 
     def ipostorder(self):
         """Depth-first post-order iteration of tree nodes."""
-        children = [self, ]
+        children = [
+            self,
+        ]
         seen = set()
         while children:
             cur_node = children[-1]
             if cur_node not in seen:
                 seen.add(cur_node)
                 children.extend(reversed(cur_node.children))
             else:
                 children.pop()
                 yield cur_node
 
-    def iupstream(self):
-        """Iterate from a tree node to the root nodes."""
-        t = self
-        while t is not None:
-            yield t
-            t = t.parent
+    def iupstream(self, stop_node=None):
+        """Iterate from a tree node to the root nodes.
+
+        Args:
+            stop_node: Node to stop the upstream traversal. If None, it stops when parent is None.
+        """
+        if stop_node is None:
+
+            def stop_condition(section):
+                return section.is_root()
+
+        else:
+
+            def stop_condition(section):
+                return section.is_root() or section == stop_node
+
+        current_section = self
+        while not stop_condition(current_section):
+            yield current_section
+            current_section = current_section.parent
+        yield current_section
 
     def ileaf(self):
         """Iterator to all leaves of a tree."""
         return filter(Section.is_leaf, self.ipreorder())
 
     def iforking_point(self, iter_mode=ipreorder):
         """Iterator to forking points.
@@ -137,43 +153,37 @@
         Args:
             iter_mode: iteration mode. Default: ipreorder.
         """
         return filter(Section.is_bifurcation_point, iter_mode(self))
 
     def __eq__(self, other):
         """Equal when its morphio section is equal."""
-        return self.morphio_section == other.morphio_section
+        return self.to_morphio().has_same_shape(other.to_morphio())
 
     def __hash__(self):
         """Hash of its id."""
         return self.id
 
-    def __nonzero__(self):
-        """If has children."""
-        return self.morphio_section is not None
-
-    __bool__ = __nonzero__
+    @property
+    def segments(self):
+        """The array of all segments of the neurite."""
+        return list(iter_segments(self))
 
     @property
     def points(self):
         """Returns the section list of points the NeuroM way (points + radius)."""
-        return np.concatenate((self.morphio_section.points,
-                               self.morphio_section.diameters[:, np.newaxis] / 2.),
-                              axis=1)
-
-    @points.setter
-    def points(self, value):
-        """Set the points."""
-        self.morphio_section.points = np.copy(value[:, COLS.XYZ])
-        self.morphio_section.diameters = np.copy(value[:, COLS.R]) * 2
+        return np.concatenate(
+            (self._morphio_section.points, self._morphio_section.diameters[:, np.newaxis] / 2.0),
+            axis=1,
+        )
 
     @property
     def type(self):
         """Returns the section type."""
-        return NeuriteType(int(self.morphio_section.type))
+        return NeuriteType(int(self._morphio_section.type))
 
     @property
     def length(self):
         """Return the path length of this section."""
         return morphmath.section_length(self.points)
 
     @property
@@ -193,26 +203,30 @@
         section's points
         """
         return sum(morphmath.segment_volume(s) for s in iter_segments(self))
 
     def __repr__(self):
         """Text representation."""
         parent_id = None if self.parent is None else self.parent.id
-        return (f'Section(id={self.id}, type={self.type}, n_points={len(self.points)})'
-                f'<parent: Section(id={parent_id}), nchildren: {len(self.children)}>')
+        return (
+            f'Section(id={self.id}, type={self.type}, n_points={len(self.points)})'
+            f'<parent: Section(id={parent_id}), nchildren: {len(self.children)}>'
+        )
 
 
 # NRN simulator iteration order
 # See:
 # https://github.com/neuronsimulator/nrn/blob/2dbf2ebf95f1f8e5a9f0565272c18b1c87b2e54c/share/lib/hoc/import3d/import3d_gui.hoc#L874
-NRN_ORDER = {NeuriteType.soma: 0,
-             NeuriteType.axon: 1,
-             NeuriteType.basal_dendrite: 2,
-             NeuriteType.apical_dendrite: 3,
-             NeuriteType.undefined: 4}
+NRN_ORDER = {
+    NeuriteType.soma: 0,
+    NeuriteType.axon: 1,
+    NeuriteType.basal_dendrite: 2,
+    NeuriteType.apical_dendrite: 3,
+    NeuriteType.undefined: 4,
+}
 
 
 def iter_neurites(obj, mapfun=None, filt=None, neurite_order=NeuriteIter.FileOrder):
     """Iterator to a neurite, morphology or morphology population.
 
     Applies optional neurite filter and mapping functions.
 
@@ -225,42 +239,68 @@
             - NeuriteIter.NRN: NRN simulator order: soma -> axon -> basal -> apical
 
     Examples:
         Get the number of points in each neurite in a morphology population
 
         >>> from neurom.core.morphology import iter_neurites
         >>> from neurom import load_morphologies
-        >>> pop = load_morphologies('path/to/morphologies')
-        >>> n_points = [n for n in iter_neurites(pop, lambda x : len(x.points))]
+        >>> pop = load_morphologies("tests/data/valid_set")
+        >>> n_points = [n for n in iter_neurites(pop, lambda x, section_type: len(x.points))]
 
         Get the number of points in each axon in a morphology population
 
         >>> import neurom as nm
         >>> from neurom.core.morphology import iter_neurites
+        >>> from neurom import load_morphologies
+        >>> pop = load_morphologies("tests/data/valid_set")
         >>> filter = lambda n : n.type == nm.AXON
-        >>> mapping = lambda n : len(n.points)
+        >>> mapping = lambda n, section_type: len(n.points)
         >>> n_points = [n for n in iter_neurites(pop, mapping, filter)]
     """
-    neurites = ((obj,) if isinstance(obj, Neurite) else
-                obj.neurites if hasattr(obj, 'neurites') else obj)
+    if isinstance(obj, Neurite):
+        neurites = (obj,)
+    elif hasattr(obj, "neurites"):
+        neurites = obj.neurites
+    else:
+        neurites = obj
+
     if neurite_order == NeuriteIter.NRN:
         if isinstance(obj, Population):
-            warnings.warn('`iter_neurites` with `neurite_order` over Population orders neurites'
-                          'within the whole population, not within each morphology separately.')
+            warnings.warn(
+                '`iter_neurites` with `neurite_order` over Population orders neurites'
+                'within the whole population, not within each morphology separately.'
+            )
         last_position = max(NRN_ORDER.values()) + 1
         neurites = sorted(neurites, key=lambda neurite: NRN_ORDER.get(neurite.type, last_position))
 
     neurite_iter = iter(neurites) if filt is None else filter(filt, neurites)
-    return neurite_iter if mapfun is None else map(mapfun, neurite_iter)
+
+    if mapfun is None:
+        return neurite_iter
+
+    return (
+        (
+            mapfun(
+                neurite,
+                section_type=filt.type if filt is not None else None,
+            )
+            if neurite.process_subtrees
+            else mapfun(neurite, section_type=NeuriteType.all)
+        )
+        for neurite in neurite_iter
+    )
 
 
-def iter_sections(neurites,
-                  iterator_type=Section.ipreorder,
-                  neurite_filter=None,
-                  neurite_order=NeuriteIter.FileOrder):
+def iter_sections(
+    neurites,
+    iterator_type=Section.ipreorder,
+    neurite_filter=None,
+    neurite_order=NeuriteIter.FileOrder,
+    section_filter=None,
+):
     """Iterator to the sections in a neurite, morphology or morphology population.
 
     Arguments:
         neurites: morphology, population, neurite, or iterable containing neurite objects
         iterator_type: section iteration order within a given neurite. Must be one of:
             Section.ipreorder: Depth-first pre-order iteration of tree nodes
             Section.ipostorder: Depth-first post-order iteration of tree nodes
@@ -268,91 +308,170 @@
             Section.ibifurcation_point: Iterator to bifurcation points
             Section.ileaf: Iterator to all leaves of a tree
 
         neurite_filter: optional top level filter on properties of neurite neurite objects.
         neurite_order (NeuriteIter): order upon which neurites should be iterated
             - NeuriteIter.FileOrder: order of appearance in the file
             - NeuriteIter.NRN: NRN simulator order: soma -> axon -> basal -> apical
+        section_filter: optional section level filter. Please note that neurite_filter takes
+            precedence over the section_filter.
 
 
     Examples:
         Get the number of points in each section of all the axons in a morphology population
 
         >>> import neurom as nm
         >>> from neurom.core.morphology import iter_sections
         >>> filter = lambda n : n.type == nm.AXON
         >>> n_points = [len(s.points) for s in iter_sections(pop,  neurite_filter=filter)]
     """
-    return flatten(
-        iterator_type(neurite.root_node)
-        for neurite in iter_neurites(neurites, filt=neurite_filter, neurite_order=neurite_order)
-    )
+    neurites = iter_neurites(neurites, filt=neurite_filter, neurite_order=neurite_order)
+    sections = flatten(iterator_type(neurite.root_node) for neurite in neurites)
+    return sections if section_filter is None else filter(section_filter, sections)
 
 
-def iter_segments(obj, neurite_filter=None, neurite_order=NeuriteIter.FileOrder):
+def iter_segments(
+    obj,
+    neurite_filter=None,
+    neurite_order=NeuriteIter.FileOrder,
+    section_filter=None,
+    section_iterator=Section.ipreorder,
+):
     """Return an iterator to the segments in a collection of neurites.
 
     Arguments:
         obj: morphology, population, neurite, section, or iterable containing neurite objects
         neurite_filter: optional top level filter on properties of neurite neurite objects
         neurite_order: order upon which neurite should be iterated. Values:
             - NeuriteIter.FileOrder: order of appearance in the file
             - NeuriteIter.NRN: NRN simulator order: soma -> axon -> basal -> apical
+        section_filter: optional section level filter
+        section_iterator: section iteration order within a given neurite. Must be one of:
+            Section.ipreorder: Depth-first pre-order iteration of tree nodes
+            Section.ipostorder: Depth-first post-order iteration of tree nodes
+            Section.iupstream: Iterate from a tree node to the root nodes
+            Section.ibifurcation_point: Iterator to bifurcation points
+            Section.ileaf: Iterator to all leaves of a tree
 
     Note:
         This is a convenience function provided for generic access to
         morphology segments. It may have a performance overhead WRT custom-made
         segment analysis functions that leverage numpy and section-wise iteration.
     """
-    sections = iter((obj,) if isinstance(obj, Section) else
-                    iter_sections(obj,
-                                  neurite_filter=neurite_filter,
-                                  neurite_order=neurite_order))
-
-    return flatten(
-        zip(section.points[:-1], section.points[1:])
-        for section in sections
+    sections = iter(
+        (obj,)
+        if isinstance(obj, Section)
+        else iter_sections(
+            obj,
+            iterator_type=section_iterator,
+            neurite_filter=neurite_filter,
+            neurite_order=neurite_order,
+            section_filter=section_filter,
+        )
     )
 
+    return flatten(zip(section.points[:-1], section.points[1:]) for section in sections)
+
+
+def iter_points(obj, neurite_filter=None, neurite_order=NeuriteIter.FileOrder, section_filter=None):
+    """Return an iterator to the points in a population, morphology, neurites, or section.
+
+    Args:
+        obj: population, morphology, neurite, section or iterable containing
+        neurite_filter: optional top level filter on properties of neurite neurite objects
+        neurite_order: order upon which neurite should be iterated. Values:
+            - NeuriteIter.FileOrder: order of appearance in the file
+            - NeuriteIter.NRN: NRN simulator order: soma -> axon -> basal -> apical
+        section_filter: optional section level filter
+    """
+    sections = (
+        iter((obj,))
+        if isinstance(obj, Section)
+        else iter_sections(
+            obj,
+            neurite_filter=neurite_filter,
+            neurite_order=neurite_order,
+            section_filter=section_filter,
+        )
+    )
+
+    return flatten(s.points[:, COLS.XYZ] for s in sections)
+
 
 def graft_morphology(section):
     """Returns a morphology starting at section."""
     assert isinstance(section, Section)
     m = morphio.mut.Morphology()
-    m.append_root_section(section.morphio_section)
+    m.append_root_section(section.to_morphio())
     return Morphology(m)
 
 
-def graft_neuron(section):
-    """Deprecated in favor of ``graft_morphology``."""
-    warn_deprecated('`neurom.core.neuron.graft_neuron` is deprecated in favor of '
-                    '`neurom.core.morphology.graft_morphology`')  # pragma: no cover
-    return graft_morphology(section)  # pragma: no cover
-
-
 class Neurite:
     """Class representing a neurite tree."""
 
-    def __init__(self, root_node):
+    def __init__(self, root_node, *, process_subtrees=False):
         """Constructor.
 
         Args:
             root_node (morphio.Section): root section
+            process_subtrees (bool): enable mixed tree processing if set to True
         """
-        self.morphio_root_node = root_node
+        self._root_node = root_node
+        self._process_subtrees = process_subtrees
+
+    @property
+    def process_subtrees(self):
+        """Enable mixed tree processing if set to True."""
+        return self._process_subtrees
+
+    @process_subtrees.setter
+    def process_subtrees(self, value):
+        self._process_subtrees = value
+        if "type" in vars(self):
+            del vars(self)["type"]
+
+    @property
+    def morphio_root_node(self):
+        """Returns the morphio root section."""
+        return self._root_node
 
     @property
     def root_node(self):
         """The first section of the neurite."""
         return Section(self.morphio_root_node)
 
-    @property
+    @cached_property
     def type(self):
-        """The type of the root node."""
-        return self.root_node.type
+        """The type of the Neurite (which can be composite)."""
+        return NeuriteType(self.subtree_types)
+
+    @cached_property
+    def subtree_types(self):
+        """The types of the subtrees."""
+        if not self._process_subtrees:
+            return NeuriteType(self.morphio_root_node.type)
+
+        it = self.root_node.ipreorder()
+        subtree_types = [next(it).to_morphio().type]
+
+        for section in it:
+            if section.type != section.parent.type:
+                subtree_types.append(NeuriteType(section.to_morphio().type))
+
+        return subtree_types
+
+    @property
+    def sections(self):
+        """The array of all sections."""
+        return list(iter_sections(self))
+
+    @property
+    def segments(self):
+        """The array of all segments of the neurite."""
+        return list(iter_segments(self))
 
     @property
     def points(self):
         """Array with all the points in this neurite.
 
         Note: Duplicate points at section bifurcations are removed
         """
@@ -364,128 +483,147 @@
 
     @property
     def length(self):
         """Returns the total length of this neurite.
 
         The length is defined as the sum of lengths of the sections.
         """
-        return sum(s.length for s in self.iter_sections())
+        # pylint: disable=import-outside-toplevel
+        from neurom.features.neurite import total_length
+
+        return total_length(self)
 
     @property
     def area(self):
         """Return the surface area of this neurite.
 
         The area is defined as the sum of area of the sections.
         """
-        return sum(s.area for s in self.iter_sections())
+        # pylint: disable=import-outside-toplevel
+        from neurom.features.neurite import total_area
+
+        return total_area(self)
 
     @property
     def volume(self):
         """Return the volume of this neurite.
 
         The volume is defined as the sum of volumes of the sections.
         """
-        return sum(s.volume for s in self.iter_sections())
+        # pylint: disable=import-outside-toplevel
+        from neurom.features.neurite import total_volume
 
-    def iter_sections(self, order=Section.ipreorder, neurite_order=NeuriteIter.FileOrder):
-        """Iteration over section nodes.
+        return total_volume(self)
 
-        Arguments:
-            order: section iteration order within a given neurite. Must be one of:
-                Section.ipreorder: Depth-first pre-order iteration of tree nodes
-                Section.ipostorder: Depth-first post-order iteration of tree nodes
-                Section.iupstream: Iterate from a tree node to the root nodes
-                Section.ibifurcation_point: Iterator to bifurcation points
-                Section.ileaf: Iterator to all leaves of a tree
-
-            neurite_order: order upon which neurites should be iterated. Values:
-                - NeuriteIter.FileOrder: order of appearance in the file
-                - NeuriteIter.NRN: NRN simulator order: soma -> axon -> basal -> apical
-        """
-        return iter_sections(self, iterator_type=order, neurite_order=neurite_order)
-
-    def __nonzero__(self):
-        """If has root node."""
-        return bool(self.morphio_root_node)
+    def is_heterogeneous(self) -> bool:
+        """Returns true if the neurite consists of more that one section types."""
+        return self.morphio_root_node.is_heterogeneous()
 
     def __eq__(self, other):
         """If root node ids and types are equal."""
-        return self.type == other.type and self.morphio_root_node.id == other.morphio_root_node.id
+        return (
+            self.type == other.type
+            and self.morphio_root_node.id == other.morphio_root_node.id
+            and self.process_subtrees == other.process_subtrees
+        )
 
     def __hash__(self):
         """Hash is made of tuple of type and root_node."""
-        return hash((self.type, self.root_node))
-
-    __bool__ = __nonzero__
+        return hash((self.type, self.root_node, self.process_subtrees))
 
     def __repr__(self):
         """Return a string representation."""
         return 'Neurite <type: %s>' % self.type
 
 
-class Morphology(morphio.mut.Morphology):
+class Morphology:
     """Class representing a simple morphology."""
 
-    def __init__(self, filename, name=None):
+    def __init__(self, morphio_morph, name=None, *, process_subtrees=False):
         """Morphology constructor.
 
         Args:
-            filename (str|Path): a filename
-            name (str): a option morphology name
-        """
-        super().__init__(filename)
+            morphio_morph (morphio.Morphology|morphio.mut.Morphology): a morphio object
+            name (str): an optional morphology name
+            process_subtrees (bool): enable mixed tree processing if set to True
+        """
+        if not isinstance(morphio_morph, (morphio.Morphology, morphio.mut.Morphology)):
+            raise NeuroMError(
+                f"Expected morphio Morphology object but got: {morphio_morph}.\n"
+                f"Use neurom.load_morphology() to load from file."
+            )
+
+        self._morphio_morph = morphio_morph
+
         self.name = name if name else 'Morphology'
-        self.morphio_soma = super().soma
-        self.neurom_soma = make_soma(self.morphio_soma)
+        self.soma = make_soma(self._morphio_morph.soma)
 
-    @property
-    def soma(self):
-        """Corresponding soma."""
-        return self.neurom_soma
+        self.process_subtrees = process_subtrees
+
+    def to_morphio(self):
+        """Returns the morphio morphology object."""
+        return self._morphio_morph
+
+    def copy(self):
+        """Returns a shallow copy of the morphio morphology object."""
+        return Morphology(self.to_morphio(), name=self.name, process_subtrees=self.process_subtrees)
 
     @property
     def neurites(self):
         """The list of neurites."""
-        return [Neurite(root_section) for root_section in self.root_sections]
+        return [
+            Neurite(root_section, process_subtrees=self.process_subtrees)
+            for root_section in self._morphio_morph.root_sections
+        ]
+
+    def section(self, section_id):
+        """Returns the section with the given id."""
+        return Section(self._morphio_morph.section(section_id))
 
     @property
     def sections(self):
         """The array of all sections, excluding the soma."""
         return list(iter_sections(self))
 
     @property
+    def segments(self):
+        """The array of all segments of the sections."""
+        return list(iter_segments(self))
+
+    @property
     def points(self):
         """Returns the list of points."""
-        return np.concatenate(
-            [section.points for section in iter_sections(self)])
+        return np.concatenate([section.points for section in iter_sections(self)])
 
     def transform(self, trans):
         """Return a copy of this morphology with a 3D transformation applied."""
-        obj = Morphology(self)
-        obj.morphio_soma.points = trans(obj.morphio_soma.points)
+        morph = self._morphio_morph
+
+        is_immutable = hasattr(morph, 'as_mutable')
+
+        # make copy or convert to mutable if immutable
+        if is_immutable:
+            morph = morph.as_mutable()
+        else:
+            morph = morphio.mut.Morphology(morph)
 
-        for section in obj.sections:
-            section.morphio_section.points = trans(section.morphio_section.points)
-        return obj
+        morph.soma.points = trans(morph.soma.points)
+
+        for section in morph.iter():
+            section.points = trans(section.points)
+
+        if is_immutable:
+            return Morphology(morph.as_immutable())
+        return Morphology(morph)
 
     def __copy__(self):
         """Creates a deep copy of Morphology instance."""
-        return Morphology(self, self.name)
+        return Morphology(self.to_morphio(), self.name)
 
     def __deepcopy__(self, memodict={}):
         """Creates a deep copy of Morphology instance."""
         # pylint: disable=dangerous-default-value
-        return Morphology(self, self.name)
+        return Morphology(self.to_morphio(), self.name)
 
     def __repr__(self):
         """Return a string representation."""
-        return 'Morphology <soma: %s, n_neurites: %d>' % \
-            (self.soma, len(self.neurites))
-
-
-class Neuron(Morphology):
-    """Deprecated ``Neuron`` class. Use ``Morphology`` instead."""
-    def __init__(self, filename, name=None):
-        """Dont use me."""
-        super().__init__(filename, name)  # pragma: no cover
-        warn_deprecated('`neurom.core.neuron.Neuron` is deprecated in favor of '
-                        '`neurom.core.morphology.Morphology`')  # pragma: no cover
+        return 'Morphology <soma: %s, n_neurites: %d>' % (self.soma, len(self.neurites))
```

### Comparing `neurom-3.2.9/neurom/core/population.py` & `neurom-4.0.0/neurom/core/population.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,50 +24,87 @@
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Morphology Population Classes and Functions."""
 import logging
+import os
+from pathlib import Path
 
 from morphio import MorphioError
+
 import neurom
 from neurom.exceptions import NeuroMError
 
-
 L = logging.getLogger(__name__)
 
 
+def _resolve_if_morphology_paths(files_or_objects):
+    """Resolve the files in the list."""
+    return [Path(os.path.abspath(f)) if isinstance(f, (Path, str)) else f for f in files_or_objects]
+
+
 class Population:
     """Morphology Population Class.
 
     Offers an iterator over morphs within population, neurites of morphs, somas of morphs.
     It does not store the loaded morphology in memory unless the morphology has been already passed
     as loaded (instance of ``Morphology``).
     """
-    def __init__(self, files, name='Population', ignored_exceptions=(), cache=False):
+
+    def __init__(
+        self,
+        files,
+        name='Population',
+        ignored_exceptions=(),
+        *,
+        cache=False,
+        process_subtrees=False,
+    ):
         """Construct a morphology population.
 
         Arguments:
             files (collections.abc.Sequence[str|Path|Morphology]): collection of morphology files or
                 paths to them or instances of ``Morphology``.
             name (str): Optional name for this Population
             ignored_exceptions (tuple): NeuroM and MorphIO exceptions that you want to ignore when
                 loading morphs.
             cache (bool): whether to cache the loaded morphs in memory. If false then a morphology
                 will be loaded everytime it is accessed within the population. Which is good when
                 population is big. If true then all morphs will be loaded upon the construction
                 and kept in memory.
+            process_subtrees (bool): enable mixed tree processing if set to True
+
+        Notes:
+            symlinks in paths are not resolved.
         """
         self._ignored_exceptions = ignored_exceptions
         self.name = name
+
+        self._files = _resolve_if_morphology_paths(files)
+
+        self._process_subtrees = process_subtrees
+
         if cache:
-            self._files = [self._load_file(f) for f in files if f is not None]
-        else:
-            self._files = files
+            self._reset_cache()
+
+    def _reset_cache(self):
+        """Reset the internal cache."""
+        self._files = [self._load_file(f) for f in self._files if f is not None]
+
+    @property
+    def process_subtrees(self):
+        """Enable mixed tree processing if set to True."""
+        return self._process_subtrees
+
+    @process_subtrees.setter
+    def process_subtrees(self, value):
+        self._process_subtrees = value
+        self._reset_cache()
 
     @property
     def morphologies(self):
         """Iterator to populations's morphologies."""
         return (n for n in self)
 
     @property
@@ -78,17 +115,19 @@
     @property
     def neurites(self):
         """Iterator to populations's neurites."""
         return (neurite for n in self for neurite in n.neurites)
 
     def _load_file(self, f):
         if isinstance(f, neurom.core.morphology.Morphology):
-            return f
+            new_morph = f.copy()
+            new_morph.process_subtrees = self.process_subtrees
+            return new_morph
         try:
-            return neurom.load_morphology(f)
+            return neurom.load_morphology(f, process_subtrees=self.process_subtrees)
         except (NeuroMError, MorphioError) as e:
             if isinstance(e, self._ignored_exceptions):
                 L.info('Ignoring exception "%s" for file %s', e, f.name)
             else:
                 raise NeuroMError('`load_morphologies` failed') from e
         return None
 
@@ -104,13 +143,14 @@
         """Length of morphology collection."""
         return len(self._files)
 
     def __getitem__(self, idx):
         """Get morphology at index idx."""
         if idx > len(self):
             raise ValueError(
-                f'no {idx} index in "{self.name}" population, max possible index is {len(self)}')
+                f'no {idx} index in "{self.name}" population, max possible index is {len(self)}'
+            )
         return self._load_file(self._files[idx])
 
     def __str__(self):
         """Return a string representation."""
         return f'Population <name: {self.name}, n_morphologies: {len(self)}>'
```

### Comparing `neurom-3.2.9/neurom/exceptions.py` & `neurom-4.0.0/neurom/exceptions.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/neurom/features/__init__.py` & `neurom-4.0.0/neurom/features/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,52 +28,67 @@
 
 """NeuroM, lightweight and fast.
 
 Examples:
     Obtain some morphometrics
     >>> import neurom
     >>> from neurom import features
-    >>> m = neurom.load_morphology('path/to/morphology')
+    >>> m = neurom.load_morphology("tests/data/swc/Neuron.swc")
     >>> ap_seg_len = features.get('segment_lengths', m, neurite_type=neurom.APICAL_DENDRITE)
     >>> ax_sec_len = features.get('section_lengths', m, neurite_type=neurom.AXON)
 """
+
+import inspect
 import operator
 from enum import Enum
-from functools import reduce
+from functools import partial, reduce, wraps
+
+import numpy as np
 
-from neurom.core import Population, Morphology, Neurite
+from neurom.core import Morphology, Neurite, Population
 from neurom.core.morphology import iter_neurites
-from neurom.core.types import NeuriteType, tree_type_checker as is_type
+from neurom.core.types import NeuriteType
+from neurom.core.types import tree_type_checker as is_type
 from neurom.exceptions import NeuroMError
 
 _NEURITE_FEATURES = {}
 _MORPHOLOGY_FEATURES = {}
 _POPULATION_FEATURES = {}
 
 
 class NameSpace(Enum):
     """The level of morphology abstraction that feature applies to."""
+
     NEURITE = 'neurite'
     NEURON = 'morphology'
     POPULATION = 'population'
 
 
 def _flatten_feature(feature_shape, feature_value):
     """Flattens feature values. Applies for population features for backward compatibility."""
     if feature_shape == ():
         return feature_value
     return reduce(operator.concat, feature_value, [])
 
 
-def _get_neurites_feature_value(feature_, obj, neurite_filter, kwargs):
+def _get_neurites_feature_value(feature_, obj, neurite_filter, **kwargs):
     """Collects neurite feature values appropriately to feature's shape."""
     kwargs.pop('neurite_type', None)  # there is no 'neurite_type' arg in _NEURITE_FEATURES
-    return reduce(operator.add,
-                  (feature_(n, **kwargs) for n in iter_neurites(obj, filt=neurite_filter)),
-                  0 if feature_.shape == () else [])
+
+    return reduce(
+        operator.add,
+        (
+            iter_neurites(
+                obj,
+                mapfun=partial(feature_, **kwargs),
+                filt=neurite_filter,
+            )
+        ),
+        0 if feature_.shape == () else [],
+    )
 
 
 def _get_feature_value_and_func(feature_name, obj, **kwargs):
     """Obtain a feature from a set of morphology objects.
 
     Arguments:
         feature_name(string): feature to extract
@@ -83,55 +98,74 @@
     Returns:
         Tuple(List|Number, function): A tuple (feature, func) of the feature value and its function.
           Feature value can be a list or a number.
     """
     # pylint: disable=too-many-branches
     is_obj_list = isinstance(obj, (list, tuple))
     if not isinstance(obj, (Neurite, Morphology, Population)) and not is_obj_list:
-        raise NeuroMError('Only Neurite, Morphology, Population or list, tuple of Neurite,'
-                          ' Morphology can be used for feature calculation')
+        raise NeuroMError(
+            "Only Neurite, Morphology, Population or list, tuple of Neurite, Morphology"
+            f"can be used for feature calculation. Got: {obj}"
+        )
 
     neurite_filter = is_type(kwargs.get('neurite_type', NeuriteType.all))
     res, feature_ = None, None
 
     if isinstance(obj, Neurite) or (is_obj_list and isinstance(obj[0], Neurite)):
         # input is a neurite or a list of neurites
         if feature_name in _NEURITE_FEATURES:
-            assert 'neurite_type' not in kwargs, 'Cant apply "neurite_type" arg to a neurite with' \
-                                                 ' a neurite feature'
+            if 'neurite_type' in kwargs:
+                raise NeuroMError(
+                    'Can not apply "neurite_type" arg to a Neurite with a neurite feature'
+                )
+
             feature_ = _NEURITE_FEATURES[feature_name]
+
             if isinstance(obj, Neurite):
                 res = feature_(obj, **kwargs)
             else:
                 res = [feature_(s, **kwargs) for s in obj]
+
     elif isinstance(obj, Morphology):
         # input is a morphology
+        if 'section_type' in kwargs:
+            raise NeuroMError('Can not apply "section_type" arg to a Morphology')
         if feature_name in _MORPHOLOGY_FEATURES:
             feature_ = _MORPHOLOGY_FEATURES[feature_name]
+
             res = feature_(obj, **kwargs)
+
         elif feature_name in _NEURITE_FEATURES:
             feature_ = _NEURITE_FEATURES[feature_name]
-            res = _get_neurites_feature_value(feature_, obj, neurite_filter, kwargs)
+            res = _get_neurites_feature_value(feature_, obj, neurite_filter, **kwargs)
+
     elif isinstance(obj, Population) or (is_obj_list and isinstance(obj[0], Morphology)):
         # input is a morphology population or a list of morphs
+        if 'section_type' in kwargs:
+            raise NeuroMError('Can not apply "section_type" arg to a Population')
         if feature_name in _POPULATION_FEATURES:
             feature_ = _POPULATION_FEATURES[feature_name]
+
             res = feature_(obj, **kwargs)
         elif feature_name in _MORPHOLOGY_FEATURES:
             feature_ = _MORPHOLOGY_FEATURES[feature_name]
+
             res = _flatten_feature(feature_.shape, [feature_(n, **kwargs) for n in obj])
         elif feature_name in _NEURITE_FEATURES:
             feature_ = _NEURITE_FEATURES[feature_name]
             res = _flatten_feature(
                 feature_.shape,
-                [_get_neurites_feature_value(feature_, n, neurite_filter, kwargs) for n in obj])
+                [_get_neurites_feature_value(feature_, n, neurite_filter, **kwargs) for n in obj],
+            )
 
     if res is None or feature_ is None:
-        raise NeuroMError(f'Cant apply "{feature_name}" feature. Please check that it exists, '
-                          'and can be applied to your input. See the features documentation page.')
+        raise NeuroMError(
+            f'Cant apply "{feature_name}" feature. Please check that it exists, '
+            'and can be applied to your input. See the features documentation page.'
+        )
 
     return res, feature_
 
 
 def get(feature_name, obj, **kwargs):
     """Obtain a feature from a set of morphology objects.
 
@@ -159,41 +193,66 @@
     Arguments:
         namespace(string): a namespace, see :class:`NameSpace`
         name(string): name of the feature, used to access the feature via `neurom.features.get()`.
         func(callable): single parameter function of a neurite.
         shape(tuple): the expected shape of the feature values
     """
     setattr(func, 'shape', shape)
-    _map = {NameSpace.NEURITE: _NEURITE_FEATURES,
-            NameSpace.NEURON: _MORPHOLOGY_FEATURES,
-            NameSpace.POPULATION: _POPULATION_FEATURES}
+    _map = {
+        NameSpace.NEURITE: _NEURITE_FEATURES,
+        NameSpace.NEURON: _MORPHOLOGY_FEATURES,
+        NameSpace.POPULATION: _POPULATION_FEATURES,
+    }
     if name in _map[namespace]:
         raise NeuroMError(f'A feature is already registered under "{name}"')
     _map[namespace][name] = func
 
 
 def feature(shape, namespace: NameSpace, name=None):
     """Feature decorator to automatically register the feature in the appropriate namespace.
 
+    This decorator also ensures that the results of the features are casted to built-in types.
+
     Arguments:
         shape(tuple): the expected shape of the feature values
         namespace(string): a namespace, see :class:`NameSpace`
         name(string): name of the feature, used to access the feature via `neurom.features.get()`.
     """
 
     def inner(func):
-        _register_feature(namespace, name or func.__name__, func, shape)
-        return func
+        @wraps(func)
+        def scalar_wrapper(*args, **kwargs):
+            res = func(*args, **kwargs)
+            try:
+                return res.tolist()
+            except AttributeError:
+                return res
+
+        @wraps(func)
+        def matrix_wrapper(*args, **kwargs):
+            res = func(*args, **kwargs)
+            return np.array(res).tolist()
+
+        if shape == ():
+            decorated_func = scalar_wrapper
+        else:
+            decorated_func = matrix_wrapper
+
+        _register_feature(namespace, name or func.__name__, decorated_func, shape)
+        return decorated_func
 
     return inner
 
 
 # These imports are necessary in order to register the features
-from neurom.features import neurite, morphology, \
-    population  # noqa, pylint: disable=wrong-import-position
+# pylint: disable=wrong-import-position
+from neurom.features import neurite  # noqa, isort: skio
+
+from neurom.features import morphology  # noqa, isort: skip
+from neurom.features import population  # noqa, isort: skip
 
 
 def _features_catalogue():
     """Returns a string with all the available builtin features."""
     indentation = "\t"
     preamble = "\n    .. Builtin Features:\n"
```

### Comparing `neurom-3.2.9/neurom/features/bifurcation.py` & `neurom-4.0.0/neurom/features/bifurcation.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,68 +25,73 @@
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Bifurcation point functions."""
 
 import numpy as np
+
+import neurom.features.section
 from neurom import morphmath
-from neurom.exceptions import NeuroMError
 from neurom.core.dataformat import COLS
 from neurom.core.morphology import Section
-from neurom.features.section import section_mean_radius
+from neurom.exceptions import NeuroMError
 
 
 def _raise_if_not_bifurcation(section):
     n_children = len(section.children)
     if n_children != 2:
-        raise NeuroMError('A bifurcation point must have exactly 2 children, found {}'.format(
-            n_children))
+        raise NeuroMError(
+            'A bifurcation point must have exactly 2 children, found {}'.format(n_children)
+        )
 
 
 def local_bifurcation_angle(bif_point):
     """Return the opening angle between two out-going sections in a bifurcation point.
 
     We first ensure that the input point has only two children.
 
     The bifurcation angle is defined as the angle between the first non-zero
     length segments of a bifurcation point.
     """
+
     def skip_0_length(sec):
         """Return the first point with non-zero distance to first point."""
         p0 = sec[0]
         cur = sec[1]
         for i, p in enumerate(sec[1:]):
-            if not np.all(p[:COLS.R] == p0[:COLS.R]):
+            if not np.all(p[: COLS.R] == p0[: COLS.R]):
                 cur = sec[i + 1]
                 break
 
         return cur
 
     _raise_if_not_bifurcation(bif_point)
 
-    ch0, ch1 = (skip_0_length(bif_point.children[0].points),
-                skip_0_length(bif_point.children[1].points))
+    ch0, ch1 = (
+        skip_0_length(bif_point.children[0].points),
+        skip_0_length(bif_point.children[1].points),
+    )
 
     return morphmath.angle_3points(bif_point.points[-1], ch0, ch1)
 
 
 def remote_bifurcation_angle(bif_point):
     """Return the opening angle between two out-going sections in a bifurcation point.
 
     We first ensure that the input point has only two children.
 
     The angle is defined as between the bifurcation point and the
     last points in the out-going sections.
     """
     _raise_if_not_bifurcation(bif_point)
 
-    return morphmath.angle_3points(bif_point.points[-1],
-                                   bif_point.children[0].points[-1],
-                                   bif_point.children[1].points[-1])
+    return morphmath.angle_3points(
+        bif_point.points[-1], bif_point.children[0].points[-1], bif_point.children[1].points[-1]
+    )
 
 
 def bifurcation_partition(bif_point, iterator_type=Section.ipreorder):
     """Calculate the partition at a bifurcation point.
 
     We first ensure that the input point has only two children.
 
@@ -152,16 +157,16 @@
         raise ValueError('Please provide a valid method for sibling ratio, found %s' % method)
 
     if method == 'first':
         # the first point is the same as the parent last point
         n = bif_point.children[0].points[1, COLS.R]
         m = bif_point.children[1].points[1, COLS.R]
     if method == 'mean':
-        n = section_mean_radius(bif_point.children[0])
-        m = section_mean_radius(bif_point.children[1])
+        n = neurom.features.section.section_mean_radius(bif_point.children[0])
+        m = neurom.features.section.section_mean_radius(bif_point.children[1])
     return min(n, m) / max(n, m)
 
 
 def diameter_power_relation(bif_point, method='first'):
     """Calculate the diameter power relation at a bifurcation point.
 
     The diameter power relation is defined in https://www.ncbi.nlm.nih.gov/pubmed/18568015
@@ -178,11 +183,39 @@
 
     if method == 'first':
         # the first point is the same as the parent last point
         d_child = bif_point.points[-1, COLS.R]
         d_child1 = bif_point.children[0].points[1, COLS.R]
         d_child2 = bif_point.children[1].points[1, COLS.R]
     if method == 'mean':
-        d_child = section_mean_radius(bif_point)
-        d_child1 = section_mean_radius(bif_point.children[0])
-        d_child2 = section_mean_radius(bif_point.children[1])
-    return (d_child / d_child1)**(1.5) + (d_child / d_child2)**(1.5)
+        d_child = neurom.features.section.section_mean_radius(bif_point)
+        d_child1 = neurom.features.section.section_mean_radius(bif_point.children[0])
+        d_child2 = neurom.features.section.section_mean_radius(bif_point.children[1])
+    return (d_child / d_child1) ** (1.5) + (d_child / d_child2) ** (1.5)
+
+
+def downstream_pathlength_asymmetry(
+    bif_point, normalization_length=1.0, iterator_type=Section.ipreorder
+):
+    """Calculates the downstream pathlength asymmetry at a bifurcation point.
+
+    Args:
+        bif_point: Bifurcation section.
+        normalization_length: Constant to divide the result with.
+        iterator_type: Iterator type that specifies how the two subtrees are traversed.
+
+    Returns:
+        The absolute difference between the downstream path distances of the two children, divided
+        by the normalization length.
+    """
+    _raise_if_not_bifurcation(bif_point)
+    return (
+        abs(
+            neurom.features.section.downstream_pathlength(
+                bif_point.children[0], iterator_type=iterator_type
+            )
+            - neurom.features.section.downstream_pathlength(
+                bif_point.children[1], iterator_type=iterator_type
+            ),
+        )
+        / normalization_length
+    )
```

### Comparing `neurom-3.2.9/neurom/features/morphology.py` & `neurom-4.0.0/neurom/features/morphology.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,86 +31,195 @@
 Any public function from this namespace can be called via the features mechanism. If calling
 directly the function in this namespace can only accept a morphology as its input. If you want to
 apply it to a morphology population then you must use the features mechanism e.g. ``features.get``.
 The features mechanism does not allow you to apply these features to neurites.
 
 >>> import neurom
 >>> from neurom import features
->>> m = neurom.load_morphology('path/to/morphology')
->>> features.get('soma_surface_area', m)
->>> population = neurom.load_morphologies('path/to/morphs')
->>> features.get('sholl_crossings', population)
+>>> m = neurom.load_morphology("tests/data/swc/Neuron.swc")
+>>> result = features.get('soma_surface_area', m)
+>>> population = neurom.load_morphologies("tests/data/valid_set")
+>>> result = features.get('sholl_crossings', population)
 
 For more details see :ref:`features`.
 """
 
 import warnings
-
+from collections.abc import Iterable
 from functools import partial
-import math
+
 import numpy as np
 
+import neurom.core.soma
 from neurom import morphmath
-from neurom.core.morphology import iter_neurites, iter_segments, Morphology
-from neurom.core.types import tree_type_checker as is_type
 from neurom.core.dataformat import COLS
+from neurom.core.morphology import (
+    Morphology,
+    iter_neurites,
+    iter_points,
+    iter_sections,
+    iter_segments,
+)
 from neurom.core.types import NeuriteType
+from neurom.core.types import tree_type_checker as is_type
 from neurom.exceptions import NeuroMError
-from neurom.features import feature, NameSpace, neurite as nf, section as sf
-from neurom.utils import str_to_plane
+from neurom.features import NameSpace, feature
+from neurom.features import neurite as nf
+from neurom.features import section as sf
 from neurom.morphmath import convex_hull
-
+from neurom.utils import flatten, str_to_plane
 
 feature = partial(feature, namespace=NameSpace.NEURON)
 
 
 def _assert_soma_center(morph):
     if morph.soma.center is None:
         raise NeuroMError(
             f"The morphology named '{morph.name}' has no soma so the feature can not be computed."
         )
+    return morph
 
 
 def _map_neurites(function, morph, neurite_type):
     return list(
-        iter_neurites(morph, mapfun=function, filt=is_type(neurite_type))
+        iter_neurites(
+            obj=morph,
+            mapfun=function,
+            filt=is_type(neurite_type),
+        )
     )
 
 
+def _map_neurite_root_nodes(function, morph, neurite_type):
+    if neurite_type == NeuriteType.all:
+        filt = None
+    else:
+
+        def filt(neurite):
+            return neurite_type == neurite.type.root_type
+
+    return [function(trunk.root_node) for trunk in iter_neurites(obj=morph, filt=filt)]
+
+
+def _filter_mode(obj, neurite_type):
+    if obj.process_subtrees:
+        return {"section_filter": is_type(neurite_type)}
+    return {"neurite_filter": is_type(neurite_type)}
+
+
+def _get_sections(morph, neurite_type):
+    return list(iter_sections(morph, **_filter_mode(morph, neurite_type)))
+
+
+def _get_segments(morph, neurite_type):
+    return list(iter_segments(morph, **_filter_mode(morph, neurite_type)))
+
+
+def _get_points(morph, neurite_type):
+    return list(iter_points(morph, **_filter_mode(morph, neurite_type)))
+
+
 @feature(shape=())
 def soma_volume(morph):
     """Get the volume of a morphology's soma."""
-    return morph.soma.volume
+    return neurom.core.soma.get_volume(morph.soma)
 
 
 @feature(shape=())
 def soma_surface_area(morph):
     """Get the surface area of a morphology's soma.
 
     Note:
         The surface area is calculated by assuming the soma is spherical.
     """
-    return 4.0 * math.pi * morph.soma.radius ** 2
+    return neurom.core.soma.get_area(morph.soma)
 
 
 @feature(shape=())
 def soma_radius(morph):
     """Get the radius of a morphology's soma."""
-    return morph.soma.radius
+    return neurom.core.soma.get_radius(morph.soma)
 
 
 @feature(shape=())
-def max_radial_distance(morph, neurite_type=NeuriteType.all):
+def max_radial_distance(morph, origin=None, neurite_type=NeuriteType.all):
     """Get the maximum radial distances of the termination sections."""
-    term_radial_distances = _map_neurites(nf.max_radial_distance, morph, neurite_type)
+    origin = morph.soma.center if origin is None else origin
 
+    term_radial_distances = _map_neurites(
+        partial(nf.max_radial_distance, origin=origin), morph, neurite_type
+    )
     return max(term_radial_distances) if term_radial_distances else 0.0
 
 
 @feature(shape=(...,))
+def section_radial_distances(morph, origin=None, neurite_type=NeuriteType.all):
+    """Section radial distances."""
+    origin = morph.soma.center if origin is None else origin
+
+    return list(
+        flatten(
+            _map_neurites(
+                partial(nf.section_radial_distances, origin=origin),
+                morph=morph,
+                neurite_type=neurite_type,
+            )
+        )
+    )
+
+
+@feature(shape=(...,))
+def section_term_radial_distances(morph, origin=None, neurite_type=NeuriteType.all):
+    """Get the radial distances of the termination sections."""
+    origin = morph.soma.center if origin is None else origin
+
+    return list(
+        flatten(
+            _map_neurites(
+                partial(nf.section_term_radial_distances, origin=origin),
+                morph=morph,
+                neurite_type=neurite_type,
+            )
+        )
+    )
+
+
+@feature(shape=(...,))
+def section_bif_radial_distances(morph, origin=None, neurite_type=NeuriteType.all):
+    """Get the radial distances of the bifurcation sections."""
+    origin = morph.soma.center if origin is None else origin
+
+    return list(
+        flatten(
+            _map_neurites(
+                partial(nf.section_bif_radial_distances, origin=origin),
+                morph=morph,
+                neurite_type=neurite_type,
+            )
+        )
+    )
+
+
+@feature(shape=(...,))
+def segment_radial_distances(morph, origin=None, neurite_type=NeuriteType.all):
+    """Ger the radial distances of the segments."""
+    origin = morph.soma.center if origin is None else origin
+
+    return list(
+        flatten(
+            _map_neurites(
+                partial(nf.segment_radial_distances, origin=origin),
+                morph=morph,
+                neurite_type=neurite_type,
+            )
+        )
+    )
+
+
+@feature(shape=(...,))
 def number_of_sections_per_neurite(morph, neurite_type=NeuriteType.all):
     """List of numbers of sections per neurite."""
     return _map_neurites(nf.number_of_sections, morph, neurite_type)
 
 
 @feature(shape=(...,))
 def total_length_per_neurite(morph, neurite_type=NeuriteType.all):
@@ -137,53 +246,53 @@
     The azimuth is defined as Angle between x-axis and the vector
     defined by (initial tree point - soma center) on the x-z plane.
 
     The range of the azimuth angle [-pi, pi] radians
     """
     _assert_soma_center(morph)
 
-    def azimuth(neurite):
+    def azimuth(root_node):
         """Azimuth of a neurite trunk."""
         return morphmath.azimuth_from_vector(
-            morphmath.vector(neurite.root_node.points[0], morph.soma.center)
+            morphmath.vector(root_node.points[0], morph.soma.center)
         )
 
-    return _map_neurites(azimuth, morph, neurite_type)
+    return _map_neurite_root_nodes(azimuth, morph, neurite_type)
 
 
 @feature(shape=(...,))
 def trunk_origin_elevations(morph, neurite_type=NeuriteType.all):
     """Get a list of all the trunk origin elevations of a morph.
 
     The elevation is defined as the angle between x-axis and the
     vector defined by (initial tree point - soma center)
     on the x-y half-plane.
 
     The range of the elevation angle [-pi/2, pi/2] radians
     """
     _assert_soma_center(morph)
 
-    def elevation(neurite):
+    def elevation(root_node):
         """Elevation of a section."""
         return morphmath.elevation_from_vector(
-            morphmath.vector(neurite.root_node.points[0], morph.soma.center)
+            morphmath.vector(root_node.points[0], morph.soma.center)
         )
 
-    return _map_neurites(elevation, morph, neurite_type)
+    return _map_neurite_root_nodes(elevation, morph, neurite_type)
 
 
 @feature(shape=(...,))
 def trunk_vectors(morph, neurite_type=NeuriteType.all):
     """Calculate the vectors between all the trunks of the morphology and the soma center."""
     _assert_soma_center(morph)
 
-    def vector_to_root_node(neurite):
-        return morphmath.vector(neurite.root_node.points[0], morph.soma.center)
+    def vector_from_soma_to_root(root_node):
+        return morphmath.vector(root_node.points[0], morph.soma.center)
 
-    return _map_neurites(vector_to_root_node, morph, neurite_type)
+    return _map_neurite_root_nodes(vector_from_soma_to_root, morph, neurite_type)
 
 
 @feature(shape=(...,))
 def trunk_angles(
     morph,
     neurite_type=NeuriteType.all,
     coords_only="xy",
@@ -222,31 +331,35 @@
         sort_coords = str_to_plane(sort_along)
         order = np.argsort(
             np.fromiter(
                 (
                     morphmath.angle_between_projections(i / np.linalg.norm(i), [0, 1])
                     for i in vectors[:, sort_coords]
                 ),
-                dtype=float)
+                dtype=float,
+            )
         )
         vectors = vectors[order]
 
     # Select coordinates to consider
     if coords_only:
         coords = str_to_plane(coords_only)
         vectors = vectors[:, coords]
 
     # Compute angles between each trunk and the next ones
     n_vectors = len(vectors)
     cycling_vectors = np.vstack([vectors, vectors])
     angles = [
-        (num_i, [
-            morphmath.angle_between_vectors(i, j)
-            for j in cycling_vectors[num_i: num_i + n_vectors]
-        ])
+        (
+            num_i,
+            [
+                morphmath.angle_between_vectors(i, j)
+                for j in cycling_vectors[num_i : num_i + n_vectors]
+            ],
+        )
         for num_i, i in enumerate(vectors)
     ]
 
     if consecutive_only:
         angles = [i[1][-1] for i in angles if i[1]]
     else:
         angles = [i[1] for i in angles]
@@ -295,28 +408,27 @@
         return []
 
     angles = np.empty((len(source_vectors), len(target_vectors), 3), dtype=float)
 
     for i, source in enumerate(source_vectors):
         for j, target in enumerate(target_vectors):
             angles[i, j, 0] = morphmath.angle_between_vectors(source, target)
-            angles[i, j, [1, 2]] = (
-                morphmath.spherical_from_vector(target) - morphmath.spherical_from_vector(source)
-            )
+            angles[i, j, [1, 2]] = morphmath.spherical_from_vector(
+                target
+            ) - morphmath.spherical_from_vector(source)
 
     # Ensure elevation differences are in [-pi, pi]
     angles[:, :, 1] = morphmath.angles_to_pi_interval(angles[:, :, 1])
 
     # Ensure azimuth differences are in [-2pi, 2pi]
     angles[:, :, 2] = morphmath.angles_to_pi_interval(angles[:, :, 2], scale=2.0)
 
     if closest_component is not None:
         angles = angles[
-            np.arange(len(angles)),
-            np.argmin(np.abs(angles[:, :, closest_component]), axis=1)
+            np.arange(len(angles)), np.argmin(np.abs(angles[:, :, closest_component]), axis=1)
         ][:, np.newaxis, :]
 
     return angles.tolist()
 
 
 @feature(shape=(...,))
 def trunk_angles_from_vector(
@@ -347,17 +459,17 @@
     # In order to avoid the failure of the process in case the neurite_type does not exist
     if len(vectors) == 0:
         return []
 
     angles = np.empty((len(vectors), 3), dtype=float)
     for i, i_vec in enumerate(vectors):
         angles[i, 0] = morphmath.angle_between_vectors(vector, i_vec)
-        angles[i, (1, 2)] = (
-            morphmath.spherical_from_vector(i_vec) - morphmath.spherical_from_vector(vector)
-        )
+        angles[i, (1, 2)] = morphmath.spherical_from_vector(
+            i_vec
+        ) - morphmath.spherical_from_vector(vector)
 
     # Ensure elevation difference are in [-pi, pi]
     angles[:, 1] = morphmath.angles_to_pi_interval(angles[:, 1])
 
     # Ensure azimuth difference are in [-2pi, 2pi]
     angles[:, 2] = morphmath.angles_to_pi_interval(angles[:, 2], scale=2)
 
@@ -388,18 +500,14 @@
     Returns:
         list[float]:
             * if ``min_length_filter`` and ``max_length_filter`` are ``None``, the radii of the
               first point of each neurite are returned.
             * else the mean radius of the points between the given ``min_length_filter`` and
               ``max_length_filter`` are returned.
     """
-    if max_length_filter is None and min_length_filter is None:
-        return [n.root_node.points[0][COLS.R]
-                for n in iter_neurites(morph, filt=is_type(neurite_type))]
-
     if min_length_filter is not None and min_length_filter <= 0:
         raise NeuroMError(
             "In 'trunk_origin_radii': the 'min_length_filter' value must be strictly greater "
             "than 0."
         )
 
     if max_length_filter is not None and max_length_filter <= 0:
@@ -414,57 +522,67 @@
         and min_length_filter >= max_length_filter
     ):
         raise NeuroMError(
             "In 'trunk_origin_radii': the 'min_length_filter' value must be strictly less than the "
             "'max_length_filter' value."
         )
 
-    def _mean_radius(neurite):
-        points = neurite.root_node.points
+    def trunk_first_radius(root_node):
+        return root_node.points[0][COLS.R]
+
+    def trunk_mean_radius(root_node):
+        points = root_node.points
+
         interval_lengths = morphmath.interval_lengths(points)
         path_lengths = np.insert(np.cumsum(interval_lengths), 0, 0)
         valid_pts = np.ones(len(path_lengths), dtype=bool)
+
         if min_length_filter is not None:
             valid_pts = valid_pts & (path_lengths >= min_length_filter)
             if not valid_pts.any():
                 warnings.warn(
                     "In 'trunk_origin_radii': the 'min_length_filter' value is greater than the "
                     "path distance of the last point of the last section so the radius of this "
                     "point is returned."
                 )
                 return points[-1, COLS.R]
+
         if max_length_filter is not None:
             valid_max = path_lengths <= max_length_filter
             valid_pts = valid_pts & valid_max
             if not valid_pts.any():
                 warnings.warn(
                     "In 'trunk_origin_radii': the 'min_length_filter' and 'max_length_filter' "
                     "values excluded all the points of the section so the radius of the first "
                     "point after the 'min_length_filter' path distance is returned."
                 )
                 # pylint: disable=invalid-unary-operand-type
                 return points[~valid_max, COLS.R][0]
+
         return points[valid_pts, COLS.R].mean()
 
-    return _map_neurites(_mean_radius, morph, neurite_type)
+    function = (
+        trunk_first_radius
+        if max_length_filter is None and min_length_filter is None
+        else trunk_mean_radius
+    )
+
+    return _map_neurite_root_nodes(function, morph, neurite_type)
 
 
 @feature(shape=(...,))
 def trunk_section_lengths(morph, neurite_type=NeuriteType.all):
     """List of lengths of trunk sections of neurites in a morph."""
-    def trunk_section_length(neurite):
-        return morphmath.section_length(neurite.root_node.points)
-
-    return _map_neurites(trunk_section_length, morph, neurite_type)
+    return _map_neurite_root_nodes(sf.section_length, morph, neurite_type)
 
 
 @feature(shape=())
 def number_of_neurites(morph, neurite_type=NeuriteType.all):
     """Number of neurites in a morph."""
-    return len(_map_neurites(lambda n: n, morph, neurite_type))
+    return len(_map_neurites(lambda x, section_type: 1, morph, neurite_type))
 
 
 @feature(shape=(...,))
 def neurite_volume_density(morph, neurite_type=NeuriteType.all):
     """Get volume density per neurite."""
     return _map_neurites(nf.volume_density, morph, neurite_type)
 
@@ -487,39 +605,53 @@
     This function can also be used with a list of sections, as follow::
 
         secs = (sec for sec in nm.iter_sections(morph) if complex_filter(sec))
         sholl = nm.features.neuritefunc.sholl_crossings(secs,
                                                         center=morph.soma.center,
                                                         radii=np.arange(0, 1000, 100))
     """
-    def _count_crossings(neurite, radius):
-        """Used to count_crossings of segments in neurite with radius."""
-        r2 = radius ** 2
+
+    def count_crossings(section, radius):
+        """Used to count crossings of segments in neurite with radius."""
+        r2 = radius**2
         count = 0
-        for start, end in iter_segments(neurite):
-            start_dist2, end_dist2 = (morphmath.point_dist2(center, start),
-                                      morphmath.point_dist2(center, end))
+        for start, end in iter_segments(section):
+            start_dist2, end_dist2 = (
+                morphmath.point_dist2(center, start),
+                morphmath.point_dist2(center, end),
+            )
 
-            count += int(start_dist2 <= r2 <= end_dist2 or
-                         end_dist2 <= r2 <= start_dist2)
+            if start_dist2 <= r2 <= end_dist2 or end_dist2 <= r2 <= start_dist2:
+                count += 1
 
         return count
 
     if center is None or radii is None:
-        assert isinstance(morph, Morphology) and morph.soma, \
-            '`sholl_crossings` input error. If `center` or `radii` is not set then `morph` is ' \
+        assert isinstance(morph, Morphology) and morph.soma, (
+            '`sholl_crossings` input error. If `center` or `radii` is not set then `morph` is '
             'expected to be an instance of Morphology and have a soma.'
+        )
         if center is None:
             _assert_soma_center(morph)
             center = morph.soma.center
         if radii is None:
             radii = [morph.soma.radius]
-    return [sum(_count_crossings(neurite, r)
-                for neurite in iter_neurites(morph, filt=is_type(neurite_type)))
-            for r in radii]
+
+    if isinstance(morph, Iterable):
+        sections = filter(is_type(neurite_type), morph)
+    else:
+        sections = _get_sections(morph, neurite_type)
+
+    counts_per_radius = [0 for _ in range(len(radii))]
+
+    for section in sections:
+        for i, radius in enumerate(radii):
+            counts_per_radius[i] += count_crossings(section, radius)
+
+    return counts_per_radius
 
 
 @feature(shape=(...,))
 def sholl_frequency(morph, neurite_type=NeuriteType.all, step_size=10, bins=None):
     """Perform Sholl frequency calculations on a morph.
 
     Args:
@@ -536,115 +668,103 @@
         bends back on itself, and crosses the same Sholl radius will get counted as
         having crossed multiple times.
 
         If a `neurite_type` is specified and there are no trees corresponding to it, an empty
         list will be returned.
     """
     _assert_soma_center(morph)
-    neurite_filter = is_type(neurite_type)
 
     if bins is None:
         min_soma_edge = morph.soma.radius
 
-        max_radius_per_neurite = [
-            np.max(np.linalg.norm(n.points[:, COLS.XYZ] - morph.soma.center, axis=1))
-            for n in morph.neurites if neurite_filter(n)
+        sections = _get_sections(morph, neurite_type)
+
+        max_radius_per_section = [
+            np.max(np.linalg.norm(section.points[:, COLS.XYZ] - morph.soma.center, axis=1))
+            for section in sections
         ]
 
-        if not max_radius_per_neurite:
+        if not max_radius_per_section:
             return []
 
-        bins = np.arange(min_soma_edge, min_soma_edge + max(max_radius_per_neurite), step_size)
+        bins = np.arange(min_soma_edge, min_soma_edge + max(max_radius_per_section), step_size)
 
     return sholl_crossings(morph, neurite_type, morph.soma.center, bins)
 
 
 def _extent_along_axis(morph, axis, neurite_type):
     """Returns the total extent of the morpholog neurites.
 
     The morphology is filtered by neurite type and the extent is calculated
     along the coordinate axis direction (e.g. COLS.X).
     """
-    it_points = (
-            p
-            for n in iter_neurites(morph, filt=is_type(neurite_type))
-            for p in n.points[:, axis]
-    )
-    try:
-        return abs(np.ptp(np.fromiter(it_points, dtype=np.float32)))
-    except ValueError:
-        # a ValueError is thrown when there are no points passed to ptp
+    points = _get_points(morph, neurite_type)
+
+    if not points:
         return 0.0
 
+    return abs(np.ptp(np.asarray(points)[:, axis]))
+
 
 @feature(shape=())
 def total_width(morph, neurite_type=NeuriteType.all):
     """Extent of morphology along axis x."""
-    return _extent_along_axis(morph, axis=COLS.X, neurite_type=neurite_type)
+    return _extent_along_axis(morph, COLS.X, neurite_type)
 
 
 @feature(shape=())
 def total_height(morph, neurite_type=NeuriteType.all):
     """Extent of morphology along axis y."""
-    return _extent_along_axis(morph, axis=COLS.Y, neurite_type=neurite_type)
+    return _extent_along_axis(morph, COLS.Y, neurite_type)
 
 
 @feature(shape=())
 def total_depth(morph, neurite_type=NeuriteType.all):
     """Extent of morphology along axis z."""
-    return _extent_along_axis(morph, axis=COLS.Z, neurite_type=neurite_type)
+    return _extent_along_axis(morph, COLS.Z, neurite_type)
 
 
 @feature(shape=())
 def volume_density(morph, neurite_type=NeuriteType.all):
     """Get the volume density.
 
     The volume density is defined as the ratio of the neurite volume and
     the volume of the morphology's enclosing convex hull
 
     .. note:: Returns `np.nan` if the convex hull computation fails or there are not points
               available due to neurite type filtering.
     """
-    # note: duplicate points are present but do not affect convex hull calculation
-    points = [
-        point
-        for point_list in iter_neurites(morph, mapfun=sf.section_points, filt=is_type(neurite_type))
-        for point in point_list
-    ]
+    points = _get_points(morph, neurite_type)
 
     if not points:
         return np.nan
 
     morph_hull = convex_hull(points)
 
     if morph_hull is None:
         return np.nan
 
-    total_volume = sum(iter_neurites(morph, mapfun=nf.total_volume, filt=is_type(neurite_type)))
+    total_volume = sum(total_volume_per_neurite(morph, neurite_type=neurite_type))
 
     return total_volume / morph_hull.volume
 
 
-def _unique_projected_points(morph, projection_plane,  neurite_type):
-
+def _unique_projected_points(morph, projection_plane, neurite_type):
     key = "".join(sorted(projection_plane.lower()))
 
     try:
         axes = {"xy": COLS.XY, "xz": COLS.XZ, "yz": COLS.YZ}[key]
 
     except KeyError as e:
-
         raise NeuroMError(
             f"Invalid 'projection_plane' argument {projection_plane}. "
             f"Please select 'xy', 'xz', or 'yz'."
         ) from e
 
-    points = list(
-        iter_neurites(morph, mapfun=sf.section_points, filt=is_type(neurite_type))
-    )
+    points = _get_points(morph, neurite_type)
 
     if len(points) == 0:
         return np.empty(shape=(0, 3), dtype=np.float32)
 
     return np.unique(np.vstack(points), axis=0)[:, axes]
 
 
@@ -719,15 +839,16 @@
     _assert_soma_center(morph)
     axis = up.upper()
 
     if axis not in {"X", "Y", "Z"}:
         raise NeuroMError(f"Unknown axis {axis}. Please choose 'X', 'Y', or 'Z'.")
 
     col = getattr(COLS, axis)
-    segments = list(iter_segments(morph, neurite_filter=is_type(neurite_type)))
+
+    segments = _get_segments(morph, neurite_type)
 
     if not segments:
         return np.nan
 
     # (Segment 1, Segment 2) x (X, Y, Z, R) X N
     segments = np.dstack(segments)
```

### Comparing `neurom-3.2.9/neurom/features/population.py` & `neurom-4.0.0/neurom/features/population.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,58 +29,72 @@
 """Population features.
 
 Any public function from this namespace can be called via features mechanism. Functions in this
 namespace can only accept a morphology population as its input no matter how called.
 
 >>> import neurom
 >>> from neurom import features
->>> pop = neurom.load_morphologies('path/to/morphs')
->>> features.get('sholl_frequency', pop)
+>>> pop = neurom.load_morphologies("tests/data/valid_set")
+>>> frequencies = features.get('sholl_frequency', pop)
 
 For more details see :ref:`features`.
 """
 
 
 from functools import partial
+
 import numpy as np
 
 from neurom.core.dataformat import COLS
+from neurom.core.morphology import iter_sections
 from neurom.core.types import NeuriteType
 from neurom.core.types import tree_type_checker as is_type
-from neurom.features import feature, NameSpace
+from neurom.features import NameSpace, feature
+from neurom.features import morphology as mf
 from neurom.features.morphology import _assert_soma_center
-from neurom.features.morphology import sholl_crossings
 
 feature = partial(feature, namespace=NameSpace.POPULATION)
 
 
 @feature(shape=(...,))
 def sholl_frequency(morphs, neurite_type=NeuriteType.all, step_size=10, bins=None):
     """Perform Sholl frequency calculations on a population of morphs.
 
     Args:
         morphs(list|Population): list of morphologies or morphology population
         neurite_type(NeuriteType): which neurites to operate on
         step_size(float): step size between Sholl radii
         bins(iterable of floats): custom binning to use for the Sholl radii. If None, it uses
         intervals of step_size between min and max radii of ``morphs``.
+        use_subtrees (bool): Enable mixed subtree processing.
 
     Note:
         Given a population, the concentric circles range from the smallest soma radius to the
         largest radial neurite distance in steps of `step_size`. Each segment of the morphology is
         tested, so a neurite that bends back on itself, and crosses the same Sholl radius will
         get counted as having crossed multiple times.
     """
     neurite_filter = is_type(neurite_type)
 
     if bins is None:
+        section_iterator = partial(
+            iter_sections, neurite_filter=neurite_filter, section_filter=neurite_filter
+        )
+
+        max_radius_per_section = [
+            np.max(np.linalg.norm(section.points[:, COLS.XYZ] - morph.soma.center, axis=1))
+            for morph in map(_assert_soma_center, morphs)
+            for section in section_iterator(morph)
+        ]
+
+        if not max_radius_per_section:
+            return []
+
         min_soma_edge = min(n.soma.radius for n in morphs)
-        max_radii = max(np.max(np.linalg.norm(n.points[:, COLS.XYZ], axis=1))
-                        for m in morphs
-                        for n in m.neurites if neurite_filter(n))
-        bins = np.arange(min_soma_edge, min_soma_edge + max_radii, step_size)
+
+        bins = np.arange(min_soma_edge, min_soma_edge + max(max_radius_per_section), step_size)
 
     def _sholl_crossings(morph):
         _assert_soma_center(morph)
-        return sholl_crossings(morph, neurite_type, morph.soma.center, bins)
+        return mf.sholl_crossings(morph, neurite_type, morph.soma.center, bins)
 
-    return np.array([_sholl_crossings(m) for m in morphs]).sum(axis=0)
+    return np.array([_sholl_crossings(m) for m in morphs]).sum(axis=0).tolist()
```

### Comparing `neurom-3.2.9/neurom/features/section.py` & `neurom-4.0.0/neurom/features/section.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,26 +28,31 @@
 
 """Section functions and functional tools."""
 
 import numpy as np
 
 from neurom import morphmath as mm
 from neurom.core.dataformat import COLS
-from neurom.core.morphology import iter_segments
+from neurom.core.morphology import Section, iter_segments
 from neurom.morphmath import interval_lengths
 
 
 def section_points(section):
     """Returns the points in the section."""
     return section.points[:, COLS.XYZ]
 
 
-def section_path_length(section):
-    """Path length from section to root."""
-    return sum(s.length for s in section.iupstream())
+def section_path_length(section, stop_node=None):
+    """Path length from section to root.
+
+    Args:
+        section: Section object.
+        stop_node: Node to stop the upstream traversal. If None, it stops when no parent is found.
+    """
+    return sum(map(section_length, section.iupstream(stop_node=stop_node)))
 
 
 def section_length(section):
     """Length of a section."""
     return section.length
 
 
@@ -133,14 +138,21 @@
 
 def segment_midpoints(section):
     """Returns the list of segment midpoints within the section."""
     pts = section.points[:, COLS.XYZ]
     return np.divide(np.add(pts[:-1], pts[1:]), 2.0).tolist()
 
 
+def segment_midpoint_radial_distances(section, origin=None):
+    """Returns the list of segment midpoint radial distances to the origin."""
+    origin = np.zeros(3, dtype=float) if origin is None else origin
+    midpoints = np.array(segment_midpoints(section))
+    return np.linalg.norm(midpoints - origin, axis=1).tolist()
+
+
 def segment_taper_rates(section):
     """Returns the list of segment taper rates within the section."""
     pts = section.points[:, COLS.XYZR]
     diff = np.diff(pts, axis=0)
     distance = np.linalg.norm(diff[:, COLS.XYZ], axis=1)
     return np.divide(2.0 * diff[:, COLS.R], distance).tolist()
 
@@ -158,16 +170,15 @@
     """
     return mm.point_dist(section.points[-1], origin)
 
 
 def section_meander_angles(section):
     """Inter-segment opening angles in a section."""
     p = section.points
-    return [mm.angle_3points(p[i - 1], p[i - 2], p[i])
-            for i in range(2, len(p))]
+    return [mm.angle_3points(p[i - 1], p[i - 2], p[i]) for i in range(2, len(p))]
 
 
 def strahler_order(section):
     """Branching order of a tree section.
 
     The strahler order is the inverse of the branch order,
     since this is computed from the tips of the tree
@@ -209,10 +220,10 @@
     radii = section.points[:, COLS.R]
     points = section.points[:, COLS.XYZ]
     lengths = np.linalg.norm(points[1:] - points[:-1], axis=1)
     mean_radii = 0.5 * (radii[1:] + radii[:-1])
     return np.sum(mean_radii * lengths) / np.sum(lengths)
 
 
-def downstream_pathlength(section):
+def downstream_pathlength(section, iterator_type=Section.ipreorder):
     """Compute the total downstream length starting from a section."""
-    return sum(sec.length for sec in section.ipreorder())
+    return sum(sec.length for sec in iterator_type(section))
```

### Comparing `neurom-3.2.9/neurom/geom/__init__.py` & `neurom-4.0.0/neurom/geom/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,27 +30,28 @@
 
 import logging
 
 import numpy as np
 
 import neurom.morphmath
 from neurom.core.dataformat import COLS
-from neurom.geom.transform import translate, rotate
+from neurom.geom.transform import rotate, translate
 
 L = logging.getLogger(__name__)
 
 
 def bounding_box(obj):
     """Get the (x, y, z) bounding box of an object containing points.
 
     Returns:
         2D numpy array of [[min_x, min_y, min_z], [max_x, max_y, max_z]]
     """
-    return np.array([np.min(obj.points[:, COLS.XYZ], axis=0),
-                     np.max(obj.points[:, COLS.XYZ], axis=0)])
+    return np.array(
+        [np.min(obj.points[:, COLS.XYZ], axis=0), np.max(obj.points[:, COLS.XYZ], axis=0)]
+    )
 
 
 def convex_hull(obj):
     """Get the convex hull from object containing points.
 
     Returns:
         scipy.spatial.ConvexHull object if successful, otherwise None
```

### Comparing `neurom-3.2.9/neurom/geom/transform.py` & `neurom-4.0.0/neurom/geom/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,23 +42,25 @@
     Returns:
         2D numpy array of transformed points
 """
 
 
 class Transform3D:
     """Class representing a generic 3D transformation."""
+
     __doc__ += _TRANSFDOC
 
     def __call__(self, points):
         """Apply a 3D transformation to a set of points."""
         raise NotImplementedError
 
 
 class Translation(Transform3D):
     """Class representing a 3D translation."""
+
     __doc__ += _TRANSFDOC
 
     def __init__(self, translation):
         """Initialize a 3D translation.
 
         Arguments:
             translation: 3-vector of x, y, z
@@ -68,14 +70,15 @@
     def __call__(self, points):
         """Apply a 3D translation to a set of points."""
         return points + self._trans
 
 
 class Rotation(Transform3D):
     """Class representing a 3D rotation."""
+
     __doc__ += _TRANSFDOC
 
     def __init__(self, dcm):
         """Initialize a 3D rotation.
 
         Arguments:
             dcm: a 3x3 direction cosine matrix
@@ -85,14 +88,15 @@
     def __call__(self, points):
         """Apply a 3D rotation to a set of points."""
         return np.dot(self._dcm, np.array(points).T).T
 
 
 class PivotRotation(Rotation):
     """Class representing a 3D rotation about a pivot point."""
+
     __doc__ += _TRANSFDOC
 
     def __init__(self, dcm, pivot=None):
         """Initialize a 3D rotation about a pivot point.
 
         Arguments:
             dcm: a 3x3 direction cosine matrix
@@ -144,15 +148,15 @@
         return obj.transform(PivotRotation(R, origin))
     except AttributeError as e:
         raise NotImplementedError from e
 
 
 def _sin(x):
     """Sine with case for pi multiples."""
-    return 0. if np.isclose(np.mod(x, np.pi), 0.) else np.sin(x)
+    return 0.0 if np.isclose(np.mod(x, np.pi), 0.0) else np.sin(x)
 
 
 def _rodrigues_to_dcm(axis, angle):
     """Generates transformation matrix from unit vector and rotation angle.
 
     The rotation is applied in the direction
     of the axis which is a unit vector following the right hand rule.
@@ -170,16 +174,16 @@
     uyy = uy * uy
     uzz = uz * uz
     uxy = ux * uy
     uxz = ux * uz
     uyz = uy * uz
 
     sn = _sin(angle)
-    cs = _sin(np.pi / 2. - angle)
-    cs1 = 1. - cs
+    cs = _sin(np.pi / 2.0 - angle)
+    cs1 = 1.0 - cs
 
     R = np.zeros([3, 3])
 
     R[0, 0] = cs + uxx * cs1
     R[0, 1] = uxy * cs1 - uz * sn
     R[0, 2] = uxz * cs1 + uy * sn
```

### Comparing `neurom-3.2.9/neurom/io/__init__.py` & `neurom-4.0.0/neurom/io/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.9/neurom/io/utils.py` & `neurom-4.0.0/neurom/io/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 import tempfile
 import uuid
 from functools import lru_cache
 from io import StringIO, open
 from pathlib import Path
 
 import morphio
+
 from neurom.core.morphology import Morphology
 from neurom.core.population import Population
 from neurom.exceptions import NeuroMError
-from neurom.utils import warn_deprecated
 
 L = logging.getLogger(__name__)
 
 
 def _is_morphology_file(filepath):
     """Check if `filepath` is a file with one of morphology file extensions."""
     return filepath.is_file() and filepath.suffix.lower() in {'.swc', '.h5', '.asc'}
@@ -116,28 +116,32 @@
     os.close(fd)
     with open(temp_file, 'w') as fd:
         stream.seek(0)
         shutil.copyfileobj(stream, fd)
     return temp_file
 
 
-def load_morphology(morph, reader=None):
+def load_morphology(morph, reader=None, *, mutable=None, process_subtrees=False):
     """Build section trees from a morphology or a h5, swc or asc file.
 
     Args:
         morph (str|Path|Morphology|morphio.Morphology|morphio.mut.Morphology): a morphology
             representation. It can be:
 
             - a filename with the h5, swc or asc extension
             - a NeuroM Neuron object
             - a morphio mutable or immutable Morphology object
             - a stream that can be put into a io.StreamIO object. In this case, the READER argument
               must be passed with the corresponding file format (asc, swc and h5)
         reader (str): Optional, must be provided if morphology is a stream to
                       specify the file format (asc, swc, h5)
+        mutable (bool|None): Whether to enforce mutability. If None and a morphio/neurom object is
+                             passed, the initial mutability will be maintained. If None and the
+                             morphology is loaded, then it will be immutable by default.
+        process_subtrees (bool): enable mixed tree processing if set to True
 
     Returns:
         A Morphology object
 
     Examples::
 
             morphology = neurom.load_morphology('my_morphology_file.h5')
@@ -152,57 +156,57 @@
                                                      (-3 -10 0 2)
                                                      |
                                                      (6 -10 0 2)
                                                      (9 -10 0 2)
                                                    )
                                                    )'''), reader='asc')
     """
-    if isinstance(morph, (Morphology, morphio.Morphology, morphio.mut.Morphology)):
-        return Morphology(morph)
-
-    if reader:
-        return Morphology(_get_file(morph, reader))
-
-    return Morphology(morph, Path(morph).name)
-
-
-def load_neuron(morph, reader=None):
-    """Deprecated in favor of ``load_morphology``."""
-    warn_deprecated('`neurom.io.utils.load_neuron` is deprecated in favor of '
-                    '`neurom.io.utils.load_morphology`')  # pragma: no cover
-    return load_morphology(morph, reader)  # pragma: no cover
-
-
-def load_morphologies(morphs,
-                      name=None,
-                      ignored_exceptions=(),
-                      cache=False):
+    if isinstance(morph, Morphology):
+        name = morph.name
+        morphio_morph = morph.to_morphio()
+    elif isinstance(morph, (morphio.Morphology, morphio.mut.Morphology)):
+        name = "Morphology"
+        morphio_morph = morph
+    else:
+        filepath = _get_file(morph, reader) if reader else morph
+        name = os.path.basename(filepath)
+        morphio_morph = morphio.Morphology(filepath)
+
+    # None does not modify existing mutability
+    if mutable is not None:
+        if mutable and isinstance(morphio_morph, morphio.Morphology):
+            morphio_morph = morphio_morph.as_mutable()
+        elif not mutable and isinstance(morphio_morph, morphio.mut.Morphology):
+            morphio_morph = morphio_morph.as_immutable()
+
+    return Morphology(morphio_morph, name=name, process_subtrees=process_subtrees)
+
+
+def load_morphologies(
+    morphs, name=None, ignored_exceptions=(), *, cache=False, process_subtrees=False
+):
     """Create a population object.
 
     From all morphologies in a directory of from morphologies in a list of file names.
 
     Arguments:
         morphs(str|Path|Iterable[Path]): path to a folder or list of paths to morphology files
         name (str): optional name of population. By default 'Population' or\
             filepath basename depending on whether morphologies is list or\
             directory path respectively.
         ignored_exceptions (tuple): NeuroM and MorphIO exceptions that you want to ignore when
             loading morphologies
         cache (bool): whether to cache the loaded morphologies in memory
+        process_subtrees (bool): enable mixed tree processing if set to True
 
     Returns:
         Population: population object
     """
     if isinstance(morphs, (str, Path)):
         files = get_files_by_path(morphs)
         name = name or Path(morphs).name
     else:
         files = morphs
         name = name or 'Population'
-    return Population(files, name, ignored_exceptions, cache)
-
-
-def load_neurons(morphs, name=None, ignored_exceptions=(), cache=False):
-    """Deprecated in favor of ``load_morphologies``."""
-    warn_deprecated('`neurom.io.utils.load_neurons` is deprecated in favor of '
-                    '`neurom.io.utils.load_morphologies`')  # pragma: no cover
-    return load_morphologies(morphs, name, ignored_exceptions, cache)  # pragma: no cover
+    return Population(
+        files, name, ignored_exceptions, cache=cache, process_subtrees=process_subtrees
+    )
```

### Comparing `neurom-3.2.9/neurom/morphmath.py` & `neurom-4.0.0/neurom/morphmath.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,31 +23,30 @@
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Mathematical and geometrical functions used to compute morphometrics."""
-import math
 import logging
+import math
 from itertools import combinations
 
 import numpy as np
 from scipy.spatial import ConvexHull
 from scipy.spatial.distance import cdist
 
 try:
     # The QhulError was moved in scipy >= 1.8 so if the import fails the old location is imported
     from scipy.spatial import QhullError
 except ImportError:  # pragma: no cover
     from scipy.spatial.qhull import QhullError
 
 from neurom.core.dataformat import COLS
 
-
 L = logging.getLogger(__name__)
 
 
 def vector(p1, p2):
     """Compute vector between two 3D points.
 
     Args:
@@ -58,17 +57,21 @@
         3-vector from p1 - p2
     """
     return np.subtract(p1[COLS.XYZ], p2[COLS.XYZ])
 
 
 def linear_interpolate(p1, p2, fraction):
     """Returns the point p satisfying: p1 + fraction * (p2 - p1)."""
-    return np.array((p1[0] + fraction * (p2[0] - p1[0]),
-                     p1[1] + fraction * (p2[1] - p1[1]),
-                     p1[2] + fraction * (p2[2] - p1[2])))
+    return np.array(
+        (
+            p1[0] + fraction * (p2[0] - p1[0]),
+            p1[1] + fraction * (p2[1] - p1[1]),
+            p1[2] + fraction * (p2[2] - p1[2]),
+        )
+    )
 
 
 def interpolate_radius(r1, r2, fraction):
     """Interpolate the radius between two values.
 
     Calculate the radius that corresponds to a point P that lies at a fraction of the length
     of a cut cone P1P2 where P1, P2 are the centers of the circles that bound the shape with radii
@@ -83,18 +86,20 @@
             The fraction at which the interpolated radius is calculated.
 
     Returns: float
         The interpolated radius.
 
     Note: The fraction is assumed from point P1, not from point P2.
     """
+
     def f(a, b, c):
         """Returns the length of the interpolated radius calculated using similar triangles."""
         return a + c * (b - a)
-    return f(r2, r1, 1. - fraction) if r1 > r2 else f(r1, r2, fraction)
+
+    return f(r2, r1, 1.0 - fraction) if r1 > r2 else f(r1, r2, fraction)
 
 
 def interval_lengths(points, prepend_zero=False):
     """Returns the list of distances between consecutive points.
 
     Args:
         points: a list of np.array of 3D points
@@ -118,15 +123,15 @@
         0, 1, 2 correspoding to 3D cartesian coordinates
         fraction: path length fraction (0.0 <= fraction <= 1.0)
         relative_offset: return absolute or relative segment distance
 
     Returns:
         (segment ID, segment offset) pair.
     """
-    if not 0. <= fraction <= 1.0:
+    if not 0.0 <= fraction <= 1.0:
         raise ValueError("Invalid fraction: %.3f" % fraction)
     lengths = interval_lengths(points)
     cum_lengths = np.cumsum(lengths)
     offset = cum_lengths[-1] * fraction
     seg_id = np.argmin(cum_lengths < offset)
     if seg_id > 0:
         offset -= cum_lengths[seg_id - 1]
@@ -235,30 +240,22 @@
 
     Returns:
         Angle in radians between (p1-p0) and (p2-p0).
         0.0 if p0==p1 or p0==p2.
     """
     vec1 = vector(p1, p0)
     vec2 = vector(p2, p0)
-    return math.atan2(np.linalg.norm(np.cross(vec1, vec2)),
-                      np.dot(vec1, vec2))
+    return math.atan2(np.linalg.norm(np.cross(vec1, vec2)), np.dot(vec1, vec2))
 
 
 def angle_between_vectors(p1, p2):
     """Computes the angle in radians between vectors 'p1' and 'p2'.
 
     Normalizes the input vectors and computes the relative angle
     between them.
-
-        >>> angle_between((1, 0), (0, 1))
-        1.5707963267948966
-        >>> angle_between((1, 0), (1, 0))
-        0.0
-        >>> angle_between((1, 0), (-1, 0))
-        3.141592653589793
     """
     if np.equal(p1, p2).all():
         return 0.0
     v1 = p1 / np.linalg.norm(p1)
     v2 = p2 / np.linalg.norm(p2)
     return np.arccos(np.clip(np.dot(v1, v2), -1.0, 1.0))
 
@@ -356,39 +353,39 @@
 
 
 def segment_radius(seg):
     """Return the mean radius of a segment.
 
     Returns: arithmetic mean of the radii of the points in seg
     """
-    return (seg[0][COLS.R] + seg[1][COLS.R]) / 2.
+    return (seg[0][COLS.R] + seg[1][COLS.R]) / 2.0
 
 
 def segment_x_coordinate(seg):
     """Return the mean x coordinate of a segment.
 
     Returns: arithmetic mean of the x coordinates of the points in seg
     """
-    return (seg[0][COLS.X] + seg[1][COLS.X]) / 2.
+    return (seg[0][COLS.X] + seg[1][COLS.X]) / 2.0
 
 
 def segment_y_coordinate(seg):
     """Return the mean y coordinate of a segment.
 
     Returns: arithmetic mean of the y coordinates of the points in seg
     """
-    return (seg[0][COLS.Y] + seg[1][COLS.Y]) / 2.
+    return (seg[0][COLS.Y] + seg[1][COLS.Y]) / 2.0
 
 
 def segment_z_coordinate(seg):
     """Return the mean z coordinate of a segment.
 
     Returns: arithmetic mean of the z coordinates of the points in seg
     """
-    return (seg[0][COLS.Z] + seg[1][COLS.Z]) / 2.
+    return (seg[0][COLS.Z] + seg[1][COLS.Z]) / 2.0
 
 
 def segment_radial_dist(seg, pos):
     """Return the radial distance of a tree segment to a given point.
 
     The radial distance is the euclidian distance between the mid-point of
     the segment and the point in question.
@@ -460,15 +457,15 @@
         Eigenvalues and respective eigenvectors
     """
     return np.linalg.eig(np.cov(points.transpose()))
 
 
 def sphere_area(r):
     """Compute the area of a sphere with radius r."""
-    return 4. * math.pi * r ** 2
+    return 4.0 * math.pi * r**2
 
 
 # Useful alias for path_distance
 section_length = path_distance
 
 
 def principal_direction_extent(points):
@@ -509,25 +506,21 @@
 def convex_hull(points):
     """Get the convex hull from an array of points.
 
     Returns:
         scipy.spatial.ConvexHull object if successful, otherwise None
     """
     if len(points) == 0:
-        L.exception(
-            "Failure to compute convex hull because there are no points"
-        )
+        L.exception("Failure to compute convex hull because there are no points")
         return None
 
     try:
         return ConvexHull(points)
     except QhullError:
-        L.exception(
-            "Failure to compute convex hull because of geometrical degeneracy."
-        )
+        L.exception("Failure to compute convex hull because of geometrical degeneracy.")
         return None
 
 
 def aspect_ratio(points):
     """Computes the min/max ratio of the principal direction extents."""
     extents = principal_direction_extent(points)
     return float(extents.min() / extents.max())
```

### Comparing `neurom-3.2.9/neurom/stats.py` & `neurom-4.0.0/neurom/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,26 +27,27 @@
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Statistical analysis helper functions.
 
 Nothing fancy. Just commonly used functions using scipy functionality.
 """
 
-from collections import namedtuple, OrderedDict
+from collections import OrderedDict, namedtuple
 from enum import Enum, unique
 
 import numpy as np
 from scipy import stats as _st
 
 FitResults = namedtuple('FitResults', ['params', 'errs', 'type'])
 
 
 @unique
 class StatTests(Enum):
     """Enum representing valid statistical tests of scipy."""
+
     ks = 1
     wilcoxon = 2
     ttest = 3
 
 
 def get_test(stest):
     """Returns the correct stat test."""
@@ -72,17 +73,19 @@
     Returns:
         JSON-compatible dictionary with fit results
 
     Note:
         Supported fit types: 'norm', 'expon', 'uniform'
     """
     type_map = {'norm': 'normal', 'expon': 'exponential', 'uniform': 'uniform'}
-    param_map = {'uniform': lambda p: [('min', p[0]), ('max', p[0] + p[1])],
-                 'norm': lambda p: [('mu', p[0]), ('sigma', p[1])],
-                 'expon': lambda p: [('lambda', 1.0 / p[1])]}
+    param_map = {
+        'uniform': lambda p: [('min', p[0]), ('max', p[0] + p[1])],
+        'norm': lambda p: [('mu', p[0]), ('sigma', p[1])],
+        'expon': lambda p: [('lambda', 1.0 / p[1])],
+    }
 
     d = OrderedDict({'type': type_map[fit_results.type]})
     d.update(param_map[fit_results.type](fit_results.params))
 
     if min_bound is not None and 'min' not in d:
         d['min'] = min_bound
     if max_bound is not None and 'max' not in d:
@@ -141,15 +144,14 @@
 
     Returns:
         Dictionary with the name of the function as key and the result
         as the respective value
     """
     stats = {}
     for func in functions:
-
         stats[func] = getattr(np, func)(data)
 
     return stats
 
 
 def compare_two(data1, data2, test=StatTests.ks):
     """Compares two distributions of data.
```

### Comparing `neurom-3.2.9/neurom/utils.py` & `neurom-4.0.0/neurom/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,16 +42,18 @@
 def warn_deprecated(msg):
     """Issue a deprecation warning."""
     warnings.warn(msg, category=NeuroMDeprecationWarning, stacklevel=3)
 
 
 def deprecated(fun_name=None, msg=""):
     """Issue a deprecation warning for a function."""
+
     def _deprecated(fun):
         """Issue a deprecation warning for a function."""
+
         @wraps(fun)
         def _wrapper(*args, **kwargs):
             """Issue deprecation warning and forward arguments to fun."""
             name = fun_name if fun_name is not None else fun.__name__
             warn_deprecated('Call to deprecated function %s. %s' % (name, msg))
             return fun(*args, **kwargs)
 
@@ -132,7 +134,17 @@
         coords = COLS.XYZ
     return coords
 
 
 def flatten(list_of_lists):
     """Flatten one level of nesting."""
     return chain.from_iterable(list_of_lists)
+
+
+def filtered_iterator(predicate, iterator_type):
+    """Returns an iterator function that is filtered by the predicate."""
+
+    @wraps(iterator_type)
+    def composed(*args, **kwargs):
+        return filter(predicate, iterator_type(*args, **kwargs))
+
+    return composed
```

### Comparing `neurom-3.2.9/neurom/view/__init__.py` & `neurom-4.0.0/neurom/view/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,11 +23,8 @@
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """View tools to visualize morphologies."""
-from neurom.view.matplotlib_impl import (plot_morph, plot_morph3d,
-                                         plot_tree, plot_tree3d,
-                                         plot_soma, plot_soma3d,
-                                         plot_dendrogram)
+from neurom.view.matplotlib_impl import plot_dendrogram, plot_morph, plot_morph3d
```

### Comparing `neurom-3.2.9/neurom/view/dendrogram.py` & `neurom-4.0.0/neurom/view/dendrogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Dendrogram helper functions and class."""
 
 import numpy as np
+
 from neurom import NeuriteType
-from neurom.core.morphology import Neurite, Morphology
 from neurom.core.dataformat import COLS
+from neurom.core.morphology import Morphology, Neurite
 from neurom.morphmath import interval_lengths
 
 
 class Dendrogram:
     """Dendrogram."""
 
     def __init__(self, neurom_section):
@@ -45,15 +46,16 @@
             neurom_section (Neurite|Morphology|Section): tree to build dendrogram for.
         """
         if isinstance(neurom_section, Morphology):
             self.neurite_type = NeuriteType.soma
             self.height = 1
             self.width = 1
             self.coords = self.get_coords(
-                np.array([0, self.height]), np.array([.5 * self.width, .5 * self.width]))
+                np.array([0, self.height]), np.array([0.5 * self.width, 0.5 * self.width])
+            )
             self.children = [Dendrogram(neurite.root_node) for neurite in neurom_section.neurites]
         else:
             if isinstance(neurom_section, Neurite):
                 neurom_section = neurom_section.root_node
             lengths = interval_lengths(neurom_section.points, prepend_zero=True)
             radii = neurom_section.points[:, COLS.R]
 
@@ -101,14 +103,15 @@
         The layout happens only in X coordinates. Children's Y coordinate is just a parent's Y
          + parent's height. Algorithm is that we calculate bounding rectangle width of each
          dendrogram's subtree. This width is a sum of all children widths calculated recursively
          in `total_width`. If no children then the width is the dendrogram's width. After the
          calculation we start to lay out. Each child gets its X coordinate as:
          parent's X + previous sibling children widths + half of this child's width.
         """
+
         HORIZONTAL_PADDING = 2
 
         def __init__(self, dendrogram):
             self.dendrogram = dendrogram
             self.children = [_PositionedDendrogram(child) for child in dendrogram.children]
             self.total_width = self.dendrogram.width
             if self.children:
@@ -116,18 +119,18 @@
                 children_width += self.HORIZONTAL_PADDING * (len(self.children) - 1)
                 self.total_width = max(self.total_width, children_width)
 
         def position_at(self, origin):  # pylint: disable=missing-docstring
             positions = {self.dendrogram: origin}
             if self.children:
                 end_point = origin + [0, self.dendrogram.height]
-                left_bottom_offset = [-.5 * self.total_width, 0]
+                left_bottom_offset = [-0.5 * self.total_width, 0]
                 children_origin = end_point + left_bottom_offset
                 for child in self.children:
-                    child_origin = children_origin + [.5 * child.total_width, 0]
+                    child_origin = children_origin + [0.5 * child.total_width, 0]
                     positions.update(child.position_at(child_origin))
                     children_origin += [child.total_width + self.HORIZONTAL_PADDING, 0]
             return positions
 
     return _PositionedDendrogram(dendrogram).position_at(origin)
```

### Comparing `neurom-3.2.9/neurom/view/matplotlib_impl.py` & `neurom-4.0.0/neurom/view/matplotlib_impl.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,43 +25,46 @@
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Morphology draw functions using matplotlib."""
 
 from functools import wraps
+
 import numpy as np
 from matplotlib.collections import LineCollection, PatchCollection
 from matplotlib.lines import Line2D
 from matplotlib.patches import Circle, FancyArrowPatch, Polygon, Rectangle
 from mpl_toolkits.mplot3d.art3d import Line3DCollection
+
 from neurom import NeuriteType, geom
+from neurom.core.dataformat import COLS
 from neurom.core.morphology import iter_neurites, iter_sections, iter_segments
 from neurom.core.soma import SomaCylinders
-from neurom.core.dataformat import COLS
 from neurom.core.types import tree_type_checker
 from neurom.morphmath import segment_radius
-from neurom.view.dendrogram import Dendrogram, get_size, layout_dendrogram, move_positions
-
 from neurom.view import matplotlib_utils
+from neurom.view.dendrogram import Dendrogram, get_size, layout_dendrogram, move_positions
 
 _LINEWIDTH = 1.2
 _ALPHA = 0.8
 _DIAMETER_SCALE = 1.0
-TREE_COLOR = {NeuriteType.basal_dendrite: 'red',
-              NeuriteType.apical_dendrite: 'purple',
-              NeuriteType.axon: 'blue',
-              NeuriteType.soma: 'black',
-              NeuriteType.undefined: 'green',
-              NeuriteType.custom5: 'orange',
-              NeuriteType.custom6: 'orange',
-              NeuriteType.custom7: 'orange',
-              NeuriteType.custom8: 'orange',
-              NeuriteType.custom9: 'orange',
-              NeuriteType.custom10: 'orange'}
+TREE_COLOR = {
+    NeuriteType.basal_dendrite: 'red',
+    NeuriteType.apical_dendrite: 'purple',
+    NeuriteType.axon: 'blue',
+    NeuriteType.soma: 'black',
+    NeuriteType.undefined: 'green',
+    NeuriteType.custom5: 'orange',
+    NeuriteType.custom6: 'orange',
+    NeuriteType.custom7: 'orange',
+    NeuriteType.custom8: 'orange',
+    NeuriteType.custom9: 'orange',
+    NeuriteType.custom10: 'orange',
+}
 
 
 def _implicit_ax(plot_func, params=None):
     """Sets ``ax`` arg for plot functions if ``ax`` is not set originally."""
 
     @wraps(plot_func)
     def wrapper(*args, **kwargs):
@@ -82,42 +85,50 @@
     return _implicit_ax(plot_func, {'projection': '3d'})
 
 
 def _plane2col(plane):
     """Take a string like 'xy', and return the indices from COLS.*."""
     planes = ('xy', 'yx', 'xz', 'zx', 'yz', 'zy')
     assert plane in planes, 'No such plane found! Please select one of: ' + str(planes)
-    return (getattr(COLS, plane[0].capitalize()),
-            getattr(COLS, plane[1].capitalize()), )
+    return (
+        getattr(COLS, plane[0].capitalize()),
+        getattr(COLS, plane[1].capitalize()),
+    )
 
 
 def _get_linewidth(tree, linewidth, diameter_scale):
     """Calculate the desired linewidth based on tree contents.
 
     If diameter_scale exists, it is used to scale the diameter of each of the segments
     in the tree
     If diameter_scale is None, the linewidth is used.
     """
     if diameter_scale is not None and tree:
-        linewidth = [2 * segment_radius(s) * diameter_scale
-                     for s in iter_segments(tree)]
+        linewidth = [2 * segment_radius(s) * diameter_scale for s in iter_segments(tree)]
     return linewidth
 
 
 def _get_color(treecolor, tree_type):
     """If treecolor set, it's returned, otherwise tree_type is used to return set colors."""
     if treecolor is not None:
         return treecolor
     return TREE_COLOR.get(tree_type, 'green')
 
 
 @_implicit_ax
-def plot_tree(tree, ax=None, plane='xy',
-              diameter_scale=_DIAMETER_SCALE, linewidth=_LINEWIDTH,
-              color=None, alpha=_ALPHA, realistic_diameters=False):
+def plot_tree(
+    tree,
+    ax=None,
+    plane='xy',
+    diameter_scale=_DIAMETER_SCALE,
+    linewidth=_LINEWIDTH,
+    color=None,
+    alpha=_ALPHA,
+    realistic_diameters=False,
+):
     """Plots a 2d figure of the tree's segments.
 
     Args:
         tree(neurom.core.Section or neurom.core.Neurite): plotted tree
         ax(matplotlib axes): on what to plot
         plane(str): Any pair of 'xyz'
         diameter_scale(float): Scale factor multiplied with segment diameters before plotting
@@ -128,57 +139,64 @@
 
     Note:
         If the tree contains one single point the plot will be empty
         since no segments can be constructed.
     """
     plane0, plane1 = _plane2col(plane)
 
-    section_segment_list = [(section, segment)
-                            for section in iter_sections(tree)
-                            for segment in iter_segments(section)]
+    section_segment_list = [
+        (section, segment) for section in iter_sections(tree) for segment in iter_segments(section)
+    ]
     colors = [_get_color(color, section.type) for section, _ in section_segment_list]
 
     if realistic_diameters:
+
         def _get_rectangle(x, y, linewidth):
             """Draw  a rectangle to represent a secgment."""
             x, y = np.array(x), np.array(y)
             diff = y - x
             angle = np.arctan2(diff[1], diff[0]) % (2 * np.pi)
-            return Rectangle(x - linewidth / 2. * np.array([-np.sin(angle), np.cos(angle)]),
-                             np.linalg.norm(diff),
-                             linewidth,
-                             angle=np.rad2deg(angle))
-
-        segs = [_get_rectangle((seg[0][plane0], seg[0][plane1]),
-                               (seg[1][plane0], seg[1][plane1]),
-                               2 * segment_radius(seg) * diameter_scale)
-                for _, seg in section_segment_list]
+            return Rectangle(
+                x - linewidth / 2.0 * np.array([-np.sin(angle), np.cos(angle)]),
+                np.linalg.norm(diff),
+                linewidth,
+                angle=np.rad2deg(angle),
+            )
+
+        segs = [
+            _get_rectangle(
+                (seg[0][plane0], seg[0][plane1]),
+                (seg[1][plane0], seg[1][plane1]),
+                2 * segment_radius(seg) * diameter_scale,
+            )
+            for _, seg in section_segment_list
+        ]
 
         collection = PatchCollection(segs, alpha=alpha, facecolors=colors)
 
     else:
-        segs = [((seg[0][plane0], seg[0][plane1]),
-                 (seg[1][plane0], seg[1][plane1]))
-                for _, seg in section_segment_list]
+        segs = [
+            ((seg[0][plane0], seg[0][plane1]), (seg[1][plane0], seg[1][plane1]))
+            for _, seg in section_segment_list
+        ]
 
         linewidth = _get_linewidth(
             tree,
             diameter_scale=diameter_scale,
             linewidth=linewidth,
         )
         collection = LineCollection(segs, colors=colors, linewidth=linewidth, alpha=alpha)
 
     ax.add_collection(collection)
 
 
 @_implicit_ax
-def plot_soma(soma, ax=None, plane='xy',
-              soma_outline=True,
-              linewidth=_LINEWIDTH,
-              color=None, alpha=_ALPHA):
+def plot_soma(
+    soma, ax=None, plane='xy', soma_outline=True, linewidth=_LINEWIDTH, color=None, alpha=_ALPHA
+):
     """Generates a 2d figure of the soma.
 
     Args:
         soma(neurom.core.Soma): plotted soma
         ax(matplotlib axes): on what to plot
         plane(str): Any pair of 'xyz'
         soma_outline(bool): should the soma be drawn as an outline
@@ -188,105 +206,140 @@
     """
     plane0, plane1 = _plane2col(plane)
     color = _get_color(color, tree_type=NeuriteType.soma)
 
     if isinstance(soma, SomaCylinders):
         for start, end in zip(soma.points, soma.points[1:]):
             matplotlib_utils.project_cylinder_onto_2d(
-                ax, (plane0, plane1),
-                start=start[COLS.XYZ], end=end[COLS.XYZ],
-                start_radius=start[COLS.R], end_radius=end[COLS.R],
-                color=color, alpha=alpha)
+                ax,
+                (plane0, plane1),
+                start=start[COLS.XYZ],
+                end=end[COLS.XYZ],
+                start_radius=start[COLS.R],
+                end_radius=end[COLS.R],
+                color=color,
+                alpha=alpha,
+            )
     else:
         if soma_outline:
-            ax.add_artist(Circle(soma.center[[plane0, plane1]], soma.radius,
-                                 color=color, alpha=alpha))
+            ax.add_artist(
+                Circle(soma.center[[plane0, plane1]], soma.radius, color=color, alpha=alpha)
+            )
         else:
             points = [[p[plane0], p[plane1]] for p in soma.iter()]
             if points:
                 points.append(points[0])  # close the loop
                 x, y = tuple(np.array(points).T)
                 ax.plot(x, y, color=color, alpha=alpha, linewidth=linewidth)
 
     ax.set_xlabel(plane[0])
     ax.set_ylabel(plane[1])
 
     bounding_box = geom.bounding_box(soma)
-    ax.dataLim.update_from_data_xy(np.vstack(([bounding_box[0][plane0], bounding_box[0][plane1]],
-                                              [bounding_box[1][plane0], bounding_box[1][plane1]])),
-                                   ignore=False)
+    ax.dataLim.update_from_data_xy(
+        np.vstack(
+            (
+                [bounding_box[0][plane0], bounding_box[0][plane1]],
+                [bounding_box[1][plane0], bounding_box[1][plane1]],
+            )
+        ),
+        ignore=False,
+    )
 
 
 # pylint: disable=too-many-arguments
 @_implicit_ax
-def plot_morph(morph, ax=None,
-               neurite_type=NeuriteType.all,
-               plane='xy',
-               soma_outline=True,
-               diameter_scale=_DIAMETER_SCALE, linewidth=_LINEWIDTH,
-               color=None, alpha=_ALPHA, realistic_diameters=False):
+def plot_morph(
+    morph,
+    ax=None,
+    neurite_type=NeuriteType.all,
+    plane='xy',
+    soma_outline=True,
+    diameter_scale=_DIAMETER_SCALE,
+    linewidth=_LINEWIDTH,
+    color=None,
+    alpha=_ALPHA,
+    realistic_diameters=False,
+):
     """Plots a 2D figure of the morphology, that contains a soma and the neurites.
 
     Args:
         neurite_type(NeuriteType|tuple): an optional filter on the neurite type
         ax(matplotlib axes): on what to plot
         morph(Morphology): morphology to be plotted
         soma_outline(bool): should the soma be drawn as an outline
         plane(str): Any pair of 'xyz'
         diameter_scale(float): Scale factor multiplied with segment diameters before plotting
         linewidth(float): all segments are plotted with this width, but only if diameter_scale=None
         color(str or None): Color of plotted values, None corresponds to default choice
         alpha(float): Transparency of plotted values
         realistic_diameters(bool): scale linewidths with axis data coordinates
     """
-    plot_soma(morph.soma, ax, plane=plane, soma_outline=soma_outline, linewidth=linewidth,
-              color=color, alpha=alpha)
+    plot_soma(
+        morph.soma,
+        ax,
+        plane=plane,
+        soma_outline=soma_outline,
+        linewidth=linewidth,
+        color=color,
+        alpha=alpha,
+    )
 
     for neurite in iter_neurites(morph, filt=tree_type_checker(neurite_type)):
-        plot_tree(neurite, ax, plane=plane,
-                  diameter_scale=diameter_scale, linewidth=linewidth,
-                  color=color, alpha=alpha, realistic_diameters=realistic_diameters)
+        plot_tree(
+            neurite,
+            ax,
+            plane=plane,
+            diameter_scale=diameter_scale,
+            linewidth=linewidth,
+            color=color,
+            alpha=alpha,
+            realistic_diameters=realistic_diameters,
+        )
 
     ax.set_title(morph.name)
     ax.set_xlabel(plane[0])
     ax.set_ylabel(plane[1])
 
 
 def _update_3d_datalim(ax, obj):
     """Unlike w/ 2d Axes, the dataLim isn't set by collections, so it has to be updated manually."""
     min_bounding_box, max_bounding_box = geom.bounding_box(obj)
-    xy_bounds = np.vstack((min_bounding_box[:COLS.Z],
-                           max_bounding_box[:COLS.Z]))
+    xy_bounds = np.vstack((min_bounding_box[: COLS.Z], max_bounding_box[: COLS.Z]))
     ax.xy_dataLim.update_from_data_xy(xy_bounds, ignore=False)
 
-    z_bounds = np.vstack(((min_bounding_box[COLS.Z], min_bounding_box[COLS.Z]),
-                          (max_bounding_box[COLS.Z], max_bounding_box[COLS.Z])))
+    z_bounds = np.vstack(
+        (
+            (min_bounding_box[COLS.Z], min_bounding_box[COLS.Z]),
+            (max_bounding_box[COLS.Z], max_bounding_box[COLS.Z]),
+        )
+    )
     ax.zz_dataLim.update_from_data_xy(z_bounds, ignore=False)
 
 
 @_implicit_ax3d
-def plot_tree3d(tree, ax=None,
-                diameter_scale=_DIAMETER_SCALE, linewidth=_LINEWIDTH,
-                color=None, alpha=_ALPHA):
+def plot_tree3d(
+    tree, ax=None, diameter_scale=_DIAMETER_SCALE, linewidth=_LINEWIDTH, color=None, alpha=_ALPHA
+):
     """Generates a figure of the tree in 3d.
 
     If the tree contains one single point the plot will be empty \
     since no segments can be constructed.
 
     Args:
         tree(neurom.core.Section or neurom.core.Neurite): plotted tree
         ax(matplotlib axes): on what to plot
         diameter_scale(float): Scale factor multiplied with segment diameters before plotting
         linewidth(float): all segments are plotted with this width, but only if diameter_scale=None
         color(str or None): Color of plotted values, None corresponds to default choice
         alpha(float): Transparency of plotted values
     """
-    section_segment_list = [(section, segment)
-                            for section in iter_sections(tree)
-                            for segment in iter_segments(section)]
+    section_segment_list = [
+        (section, segment) for section in iter_sections(tree) for segment in iter_segments(section)
+    ]
     segs = [(seg[0][COLS.XYZ], seg[1][COLS.XYZ]) for _, seg in section_segment_list]
     colors = [_get_color(color, section.type) for section, _ in section_segment_list]
 
     linewidth = _get_linewidth(tree, diameter_scale=diameter_scale, linewidth=linewidth)
 
     collection = Line3DCollection(segs, colors=colors, linewidth=linewidth, alpha=alpha)
     ax.add_collection3d(collection)
@@ -304,67 +357,87 @@
         color(str or None): Color of plotted values, None corresponds to default choice
         alpha(float): Transparency of plotted values
     """
     color = _get_color(color, tree_type=NeuriteType.soma)
 
     if isinstance(soma, SomaCylinders):
         for start, end in zip(soma.points, soma.points[1:]):
-            matplotlib_utils.plot_cylinder(ax,
-                                           start=start[COLS.XYZ], end=end[COLS.XYZ],
-                                           start_radius=start[COLS.R], end_radius=end[COLS.R],
-                                           color=color, alpha=alpha)
+            matplotlib_utils.plot_cylinder(
+                ax,
+                start=start[COLS.XYZ],
+                end=end[COLS.XYZ],
+                start_radius=start[COLS.R],
+                end_radius=end[COLS.R],
+                color=color,
+                alpha=alpha,
+            )
     else:
-        matplotlib_utils.plot_sphere(ax, center=soma.center[COLS.XYZ], radius=soma.radius,
-                                     color=color, alpha=alpha)
+        matplotlib_utils.plot_sphere(
+            ax, center=soma.center[COLS.XYZ], radius=soma.radius, color=color, alpha=alpha
+        )
 
     # unlike w/ 2d Axes, the dataLim isn't set by collections, so it has to be updated manually
     _update_3d_datalim(ax, soma)
 
 
 @_implicit_ax3d
-def plot_morph3d(morph, ax=None, neurite_type=NeuriteType.all,
-                 diameter_scale=_DIAMETER_SCALE, linewidth=_LINEWIDTH,
-                 color=None, alpha=_ALPHA):
+def plot_morph3d(
+    morph,
+    ax=None,
+    neurite_type=NeuriteType.all,
+    diameter_scale=_DIAMETER_SCALE,
+    linewidth=_LINEWIDTH,
+    color=None,
+    alpha=_ALPHA,
+):
     """Generates a figure of the morphology, that contains a soma and a list of trees.
 
     Args:
         morph(Morphology): morphology to be plotted
         ax(matplotlib axes): on what to plot
         neurite_type(NeuriteType): an optional filter on the neurite type
         diameter_scale(float): Scale factor multiplied with segment diameters before plotting
         linewidth(float): all segments are plotted with this width, but only if diameter_scale=None
         color(str or None): Color of plotted values, None corresponds to default choice
         alpha(float): Transparency of plotted values
     """
     plot_soma3d(morph.soma, ax, color=color, alpha=alpha)
 
     for neurite in iter_neurites(morph, filt=tree_type_checker(neurite_type)):
-        plot_tree3d(neurite, ax,
-                    diameter_scale=diameter_scale, linewidth=linewidth,
-                    color=color, alpha=alpha)
+        plot_tree3d(
+            neurite,
+            ax,
+            diameter_scale=diameter_scale,
+            linewidth=linewidth,
+            color=color,
+            alpha=alpha,
+        )
 
     ax.set_title(morph.name)
 
 
 def _get_dendrogram_legend(dendrogram):
     """Generates labels legend for dendrogram.
 
     Because dendrogram is rendered as patches, we need to manually label it.
     Args:
         dendrogram (Dendrogram): dendrogram
 
     Returns:
         List of legend handles.
     """
+
     def neurite_legend(neurite_type):
         return Line2D([0], [0], color=TREE_COLOR[neurite_type], lw=2, label=neurite_type.name)
 
     if dendrogram.neurite_type == NeuriteType.soma:
-        handles = {d.neurite_type: neurite_legend(d.neurite_type)
-                   for d in [dendrogram] + dendrogram.children}
+        handles = {
+            d.neurite_type: neurite_legend(d.neurite_type)
+            for d in [dendrogram] + dendrogram.children
+        }
         return handles.values()
     return [neurite_legend(dendrogram.neurite_type)]
 
 
 def _as_dendrogram_polygon(coords, color):
     return Polygon(coords, color=color, fill=True)
 
@@ -405,17 +478,17 @@
         obj (neurom.Morphology, neurom.Section): morphology or section
         ax: matplotlib axes
         show_diameters (bool): whether to show node diameters or not
     """
     dendrogram = Dendrogram(obj)
     positions = layout_dendrogram(dendrogram, np.array([0, 0]))
     w, h = get_size(positions)
-    positions = move_positions(positions, np.array([.5 * w, 0]))
-    ax.set_xlim([-.05 * w, 1.05 * w])
-    ax.set_ylim([-.05 * h, 1.05 * h])
+    positions = move_positions(positions, np.array([0.5 * w, 0]))
+    ax.set_xlim([-0.05 * w, 1.05 * w])
+    ax.set_ylim([-0.05 * h, 1.05 * h])
     ax.set_title('Morphology Dendrogram')
     ax.set_xlabel('micrometers (um)')
     ax.set_ylabel('micrometers (um)')
     shapes = _get_dendrogram_shapes(dendrogram, positions, show_diameters)
     ax.add_collection(PatchCollection(shapes, match_original=True))
 
     ax.set_aspect('auto')
```

### Comparing `neurom-3.2.9/neurom/view/matplotlib_utils.py` & `neurom-4.0.0/neurom/view/matplotlib_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,28 @@
 
 """Functionality for styling plots."""
 
 from pathlib import Path
 
 import numpy as np
 from matplotlib.patches import Polygon
+
 # needed so that projection='3d' works with fig.add_subplot
 from mpl_toolkits.mplot3d import Axes3D  # pylint: disable=unused-import
 from scipy.linalg import norm
 from scipy.spatial import ConvexHull
 
-
 plt = None  # refer to _get_plt()
 
 
 def _get_plt():
     """Wrapper to avoid loading matplotlib.pyplot before someone has a chance to set the backend."""
     global plt  # pylint: disable=global-statement
     import matplotlib.pyplot  # pylint: disable=import-outside-toplevel
+
     plt = matplotlib.pyplot
 
 
 def dict_if_none(arg):
     """Return an empty dict if arg is None."""
     return arg if arg is not None else {}
 
@@ -107,16 +108,25 @@
         ax = fig.add_subplot(*subplot, **params)
     else:
         ax = fig.add_subplot(subplot, **params)
 
     return fig, ax
 
 
-def save_plot(fig, prefile='', postfile='', output_path='./', output_name='Figure',
-              output_format='png', dpi=300, transparent=False, **_):
+def save_plot(
+    fig,
+    prefile='',
+    postfile='',
+    output_path='./',
+    output_name='Figure',
+    output_format='png',
+    dpi=300,
+    transparent=False,
+    **_,
+):
     """Generates a figure file in the selected directory.
 
     Args:
         fig: matplotlib figure
         prefile(str): Include before the general filename of the figure
         postfile(str): Included after the general filename of the figure
         output_path(str): Define the path to the output directory
@@ -124,51 +134,57 @@
         output_format(str): String to define the format of the output figure
         dpi(int): Define the DPI (Dots per Inch) of the figure
         transparent(bool): If True the saved figure will have a transparent background
     """
     output_path = Path(output_path)
     output_path.mkdir(parents=True, exist_ok=True)
 
-    fig.savefig(Path(output_path, prefile + output_name + postfile + "." + output_format),
-                dpi=dpi, transparent=transparent)
-
-
-def plot_style(fig, ax,  # pylint: disable=too-many-arguments, too-many-locals
-               # plot_title
-               pretitle='',
-               title='Figure',
-               posttitle='',
-               title_fontsize=14,
-               title_arg=None,
-               # plot_labels
-               label_fontsize=14,
-               xlabel=None,
-               xlabel_arg=None,
-               ylabel=None,
-               ylabel_arg=None,
-               zlabel=None,
-               zlabel_arg=None,
-               # plot_ticks
-               tick_fontsize=12,
-               xticks=None,
-               xticks_args=None,
-               yticks=None,
-               yticks_args=None,
-               zticks=None,
-               zticks_args=None,
-               # update_plot_limits
-               white_space=30,
-               # plot_legend
-               no_legend=True,
-               legend_arg=None,
-               # internal
-               no_axes=False,
-               aspect_ratio='equal',
-               tight=False,
-               **_):
+    fig.savefig(
+        Path(output_path, prefile + output_name + postfile + "." + output_format),
+        dpi=dpi,
+        transparent=transparent,
+    )
+
+
+def plot_style(
+    fig,
+    ax,
+    # plot_title
+    pretitle='',
+    title='Figure',
+    posttitle='',
+    title_fontsize=14,
+    title_arg=None,
+    # plot_labels
+    label_fontsize=14,
+    xlabel=None,
+    xlabel_arg=None,
+    ylabel=None,
+    ylabel_arg=None,
+    zlabel=None,
+    zlabel_arg=None,
+    # plot_ticks
+    tick_fontsize=12,
+    xticks=None,
+    xticks_args=None,
+    yticks=None,
+    yticks_args=None,
+    zticks=None,
+    zticks_args=None,
+    # update_plot_limits
+    white_space=30,
+    # plot_legend
+    no_legend=True,
+    legend_arg=None,
+    # internal
+    no_axes=False,
+    aspect_ratio='equal',
+    tight=False,
+    **_,
+):  # pylint: disable=too-many-arguments, too-many-locals
     """Set the basic options of a matplotlib figure, to be used by viewing - plotting functions.
 
     Args:
         fig(matplotlib figure): figure
         ax(matplotlib axes, belonging to `fig`): axes
 
         pretitle(str): String to include before the general title of the figure
@@ -240,18 +256,24 @@
         current_title = pretitle + title + posttitle
 
     title_arg = dict_if_none(title_arg)
 
     ax.set_title(current_title, fontsize=title_fontsize, **title_arg)
 
 
-def plot_labels(ax, label_fontsize=14,
-                xlabel=None, xlabel_arg=None,
-                ylabel=None, ylabel_arg=None,
-                zlabel=None, zlabel_arg=None):
+def plot_labels(
+    ax,
+    label_fontsize=14,
+    xlabel=None,
+    xlabel_arg=None,
+    ylabel=None,
+    ylabel_arg=None,
+    zlabel=None,
+    zlabel_arg=None,
+):
     """Sets the labels options of a matplotlib plot.
 
     Args:
         ax: matplotlib axes
         label_fontsize(int): Size of the labels' font
         xlabel(str): The xlabel for the figure
         xlabel_arg(dict):  Passsed into matplotlib as xlabel arguments
@@ -271,18 +293,24 @@
 
     if hasattr(ax, 'zaxis'):
         zlabel = zlabel if zlabel is not None else ax.get_zlabel() or 'Z'
         zlabel_arg = dict_if_none(zlabel_arg)
         ax.set_zlabel(zlabel, fontsize=label_fontsize, **zlabel_arg)
 
 
-def plot_ticks(ax, tick_fontsize=12,
-               xticks=None, xticks_args=None,
-               yticks=None, yticks_args=None,
-               zticks=None, zticks_args=None):
+def plot_ticks(
+    ax,
+    tick_fontsize=12,
+    xticks=None,
+    xticks_args=None,
+    yticks=None,
+    yticks_args=None,
+    zticks=None,
+    zticks_args=None,
+):
     """Function that defines the labels options of a matplotlib plot.
 
     Args:
         ax: matplotlib axes
         tick_fontsize (int): Defines the size of the ticks' font
         xticks([list of ticks]): Defines the values of x ticks in the figure
         xticks_args(dict):  Passsed into matplotlib as xticks arguments
@@ -357,42 +385,41 @@
         not_v = np.array([0, 1, 0])
     n1 = np.cross(v, not_v)
     n1 /= norm(n1)
     n2 = np.cross(v, n1)
     return n1, n2
 
 
-def generate_cylindrical_points(start, end, start_radius, end_radius,
-                                linspace_count=_LINSPACE_COUNT):
+def generate_cylindrical_points(
+    start, end, start_radius, end_radius, linspace_count=_LINSPACE_COUNT
+):
     """Generate a 3d mesh of a cylinder with start and end points, and varying radius.
 
     Based on: http://stackoverflow.com/a/32383775
     """
     v = end - start
     length = norm(v)
     v = v / length
     n1, n2 = _get_normals(v)
 
     # pylint: disable=unbalanced-tuple-unpacking
-    l, theta = np.meshgrid(np.linspace(0, length, linspace_count),
-                           np.linspace(0, 2 * np.pi, linspace_count))
+    l, theta = np.meshgrid(
+        np.linspace(0, length, linspace_count), np.linspace(0, 2 * np.pi, linspace_count)
+    )
 
     radii = np.linspace(start_radius, end_radius, linspace_count)
     rsin = np.multiply(radii, np.sin(theta))
     rcos = np.multiply(radii, np.cos(theta))
 
-    return np.array([start[i] +
-                     v[i] * l +
-                     n1[i] * rsin + n2[i] * rcos
-                     for i in range(3)])
+    return np.array([start[i] + v[i] * l + n1[i] * rsin + n2[i] * rcos for i in range(3)])
 
 
-def project_cylinder_onto_2d(ax, plane,
-                             start, end, start_radius, end_radius,
-                             color='black', alpha=1.):
+def project_cylinder_onto_2d(
+    ax, plane, start, end, start_radius, end_radius, color='black', alpha=1.0
+):
     """Take cylinder defined by start/end, and project it onto the plane.
 
     Args:
         ax: matplotlib axes
         plane(tuple of int): where x, y, z = 0, 1, 2, so (0, 1) is the xy axis
         start(np.array): start coordinates
         end(np.array): end coordinates
@@ -402,31 +429,39 @@
         alpha(float): alpha value
 
     Note: There are probably more efficient ways of doing this: here the
     3d outline is calculated, the non-used plane coordinates are dropped, a
     tight convex hull is found, and that is used for a filled polygon
     """
     points = generate_cylindrical_points(start, end, start_radius, end_radius, 10)
-    points = np.vstack([points[plane[0]].ravel(),
-                        points[plane[1]].ravel()])
+    points = np.vstack([points[plane[0]].ravel(), points[plane[1]].ravel()])
     points = points.T
     hull = ConvexHull(points)
     ax.add_patch(Polygon(points[hull.vertices], fill=True, color=color, alpha=alpha))
 
 
-def plot_cylinder(ax, start, end, start_radius, end_radius,
-                  color='black', alpha=1., linspace_count=_LINSPACE_COUNT):
+def plot_cylinder(
+    ax,
+    start,
+    end,
+    start_radius,
+    end_radius,
+    color='black',
+    alpha=1.0,
+    linspace_count=_LINSPACE_COUNT,
+):
     """Plot a 3d cylinder."""
     assert not np.all(start == end), 'Cylinder must have length'
-    x, y, z = generate_cylindrical_points(start, end, start_radius, end_radius,
-                                          linspace_count=linspace_count)
+    x, y, z = generate_cylindrical_points(
+        start, end, start_radius, end_radius, linspace_count=linspace_count
+    )
     ax.plot_surface(x, y, z, color=color, alpha=alpha)
 
 
-def plot_sphere(ax, center, radius, color='black', alpha=1., linspace_count=_LINSPACE_COUNT):
+def plot_sphere(ax, center, radius, color='black', alpha=1.0, linspace_count=_LINSPACE_COUNT):
     """Plots a 3d sphere, given the center and the radius."""
     u = np.linspace(0, 2 * np.pi, linspace_count)
     v = np.linspace(0, np.pi, linspace_count)
     sin_v = np.sin(v)
     x = center[0] + radius * np.outer(np.cos(u), sin_v)
     y = center[1] + radius * np.outer(np.sin(u), sin_v)
     z = center[2] + radius * np.outer(np.ones_like(u), np.cos(v))
```

### Comparing `neurom-3.2.9/neurom/view/plotly_impl.py` & `neurom-4.0.0/neurom/view/plotly_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,27 +26,26 @@
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Morphology draw functions using plotly."""
 
 import numpy as np
 
-
 try:
     import plotly.graph_objs as go
-    from plotly.offline import plot, iplot, init_notebook_mode
+    from plotly.offline import init_notebook_mode, iplot, plot
 except ImportError as e:
     raise ImportError(
         'neurom[plotly] is not installed. Please install it by doing: pip install neurom[plotly]'
     ) from e
 
-from neurom import COLS, iter_segments, iter_neurites
+from neurom import COLS, iter_neurites, iter_segments
 from neurom.core.morphology import Morphology
-from neurom.view.matplotlib_impl import TREE_COLOR
 from neurom.utils import flatten
+from neurom.view.matplotlib_impl import TREE_COLOR
 
 
 def plot_morph(morph, plane='xy', inline=False, **kwargs):
     """Draw morphology in 2D.
 
     Args:
         morph(Morphology|Section): morphology or section
@@ -71,34 +70,27 @@
 def _make_trace(morph, plane):
     """Create the trace to be plotted."""
     for neurite in iter_neurites(morph):
         segments = list(iter_segments(neurite))
 
         segs = [(s[0][COLS.XYZ], s[1][COLS.XYZ]) for s in segments]
 
-        coords = {'x': list(flatten((p1[0], p2[0], None) for p1, p2 in segs)),
-                  'y': list(flatten((p1[1], p2[1], None) for p1, p2 in segs)),
-                  'z': list(flatten((p1[2], p2[2], None) for p1, p2 in segs)),
-                  }
+        coords = {
+            "x": list(flatten((p1[0], p2[0], None) for p1, p2 in segs)),
+            "y": list(flatten((p1[1], p2[1], None) for p1, p2 in segs)),
+            "z": list(flatten((p1[2], p2[2], None) for p1, p2 in segs)),
+        }
 
         color = TREE_COLOR.get(neurite.root_node.type, 'black')
         if plane.lower() == '3d':
             plot_fun = go.Scatter3d
         else:
             plot_fun = go.Scatter
-            coords = {'x': coords[plane[0]],
-                      'y': coords[plane[1]],
-                      }
-        yield plot_fun(
-            line={'color': color,
-                  'width': 2,
-                  },
-            mode='lines',
-            **coords
-        )
+            coords = {"x": coords[plane[0]], "y": coords[plane[1]]}
+        yield plot_fun(line={"color": color, "width": 2}, mode='lines', **coords)
 
 
 def _fill_soma_data(morph, data, plane):
     """Fill soma data if 3D plot and returns soma_2d in all cases."""
     if not isinstance(morph, Morphology):
         return []
 
@@ -110,15 +102,14 @@
                 'xref': 'x',
                 'yref': 'y',
                 'fillcolor': 'rgba(50, 171, 96, 0.7)',
                 'x0': morph.soma.center[0] - morph.soma.radius,
                 'y0': morph.soma.center[1] - morph.soma.radius,
                 'x1': morph.soma.center[0] + morph.soma.radius,
                 'y1': morph.soma.center[1] + morph.soma.radius,
-
                 'line': {
                     'color': 'rgba(50, 171, 96, 1)',
                 },
             },
         ]
 
     else:
@@ -140,42 +131,41 @@
     return soma_2d
 
 
 def get_figure(morph, plane, title):
     """Returns the plotly figure containing the morphology."""
     data = list(_make_trace(morph, plane))
     axis = {
-        'gridcolor': 'rgb(255, 255, 255)',
-        'zerolinecolor': 'rgb(255, 255, 255)',
-        'showbackground': True,
-        'backgroundcolor': 'rgb(230, 230,230)',
+        "gridcolor": "rgb(255, 255, 255)",
+        "zerolinecolor": "rgb(255, 255, 255)",
+        "showbackground": True,
+        "backgroundcolor": "rgb(230, 230,230)",
     }
 
     soma_2d = _fill_soma_data(morph, data, plane)
 
     layout = {
-        'autosize': True,
-        'title': title,
-        'scene': {
-            'xaxis': axis,
-            'yaxis': axis,
-            'zaxis': axis,
-            'camera': {'up': {'x': 0,
-                              'y': 0,
-                              'z': 1,
-                              },
-                       'eye': {'x': -1.7428,
-                               'y': 1.0707,
-                               'z': 0.7100,
-                               },
-                       },
-            'aspectmode': 'data',
+        "autosize": True,
+        "title": title,
+        "scene": {  # This is used for 3D plots
+            "xaxis": axis,
+            "yaxis": axis,
+            "zaxis": axis,
+            "camera": {
+                "up": {"x": 0, "y": 0, "z": 1},
+                "eye": {
+                    "x": -1.7428,
+                    "y": 1.0707,
+                    "z": 0.7100,
+                },
+            },
+            "aspectmode": "data",
         },
-        'yaxis': {'scaleanchor': "x"},  # This is used for 2D plots
-        'shapes': soma_2d,
+        "yaxis": {"scaleanchor": "x"},  # This is used for 2D plots
+        "shapes": soma_2d,
     }
 
     res = {"data": data, "layout": layout}
     return res
 
 
 def _plotly(morph, plane, title, inline, **kwargs):
```

### Comparing `neurom-3.2.9/neurom.egg-info/PKG-INFO` & `neurom-4.0.0/neurom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurom
-Version: 3.2.9
+Version: 4.0.0
 Summary: NeuroM: a light-weight neuron morphology analysis package
 Author: Blue Brain Project, EPFL
 License: Copyright (c) 2015-2022 Blue Brain Project/EPFL 
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -50,14 +50,15 @@
 Requires-Dist: matplotlib>=3.2.1
 Requires-Dist: morphio>=3.3.6
 Requires-Dist: numpy>=1.8.0
 Requires-Dist: pandas>=1.0.5
 Requires-Dist: pyyaml>=3.10
 Requires-Dist: scipy>=1.2.0
 Requires-Dist: tqdm>=4.8.4
+Requires-Dist: cached_property>=1.5.1
 Requires-Dist: importlib_resources>=1.3; python_version < "3.9"
 Provides-Extra: plotly
 Requires-Dist: plotly>=3.6.0; extra == "plotly"
 Requires-Dist: psutil>=5.5.1; extra == "plotly"
 Provides-Extra: docs
 Requires-Dist: sphinx-bluebrain-theme; extra == "docs"
 Requires-Dist: sphinx-autorun; extra == "docs"
```

### Comparing `neurom-3.2.9/neurom.egg-info/SOURCES.txt` & `neurom-4.0.0/neurom.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -16,36 +16,36 @@
 setup.py
 tox.ini
 .binder/postBuild
 .binder/runtime.txt
 .github/workflows/mirror-ebrains.yml
 .github/workflows/publish-sdist.yml
 .github/workflows/run-tox.yml
-doc/Makefile
-doc/clean.sh
-doc/make.bat
 doc/source/api.rst
 doc/source/changelog.rst
 doc/source/cli.rst
 doc/source/conf.py
 doc/source/definitions.rst
 doc/source/developer.rst
 doc/source/documentation.rst
 doc/source/examples.rst
 doc/source/features.rst
+doc/source/heterogeneous.rst
 doc/source/index.rst
 doc/source/install.rst
 doc/source/license.rst
 doc/source/migration.rst
 doc/source/morph_check.rst
 doc/source/morph_stats.rst
 doc/source/quickstart.rst
 doc/source/spherical_coordinates.rst
 doc/source/tutorial.rst
 doc/source/validation.rst
+doc/source/images/heterogeneous_neurite.png
+doc/source/images/heterogeneous_neuron.png
 doc/source/images/spherical_coordinates.svg
 doc/source/images/spherical_coordinates.tex
 doc/source/logo/NeuroM.jpg
 examples/boxplot.py
 examples/density_plot.py
 examples/end_to_end_distance.py
 examples/extract_distribution.py
@@ -59,15 +59,14 @@
 examples/section_ids.py
 examples/soma_radius_fit.py
 neurom/__init__.py
 neurom/exceptions.py
 neurom/morphmath.py
 neurom/stats.py
 neurom/utils.py
-neurom/viewer.py
 neurom.egg-info/PKG-INFO
 neurom.egg-info/SOURCES.txt
 neurom.egg-info/dependency_links.txt
 neurom.egg-info/entry_points.txt
 neurom.egg-info/requires.txt
 neurom.egg-info/top_level.txt
 neurom/apps/__init__.py
@@ -76,31 +75,27 @@
 neurom/apps/morph_check.py
 neurom/apps/morph_stats.py
 neurom/apps/config/morph_check.yaml
 neurom/apps/config/morph_stats.yaml
 neurom/check/__init__.py
 neurom/check/morphology_checks.py
 neurom/check/morphtree.py
-neurom/check/neuron_checks.py
 neurom/check/runner.py
 neurom/core/__init__.py
 neurom/core/dataformat.py
 neurom/core/morphology.py
-neurom/core/neuron.py
 neurom/core/population.py
 neurom/core/soma.py
 neurom/core/types.py
 neurom/features/__init__.py
 neurom/features/bifurcation.py
-neurom/features/bifurcationfunc.py
 neurom/features/morphology.py
 neurom/features/neurite.py
 neurom/features/population.py
 neurom/features/section.py
-neurom/features/sectionfunc.py
 neurom/geom/__init__.py
 neurom/geom/transform.py
 neurom/io/__init__.py
 neurom/io/utils.py
 neurom/view/__init__.py
 neurom/view/dendrogram.py
 neurom/view/matplotlib_impl.py
```

### Comparing `neurom-3.2.9/pylintrc` & `neurom-4.0.0/pylintrc`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## look at http://docutils.sourceforge.net/sandbox/py-rest-doc/utils/pylintrc
+# look at http://docutils.sourceforge.net/sandbox/py-rest-doc/utils/pylintrc
 # for some of the options that are available
 
 [MESSAGES CONTROL]
 #C0103 -  Invalid name "%s" (should match %s) - matches too many things, like variables w/ single char names
 #R0903 - Too Few public methods
 #W0511 - TODO in code
 #R0401 - cyclic-import
@@ -52,8 +52,8 @@
 # (useful for classes with attributes dynamically set).
 #ignored-classes=foo.bar
 
 # List of module names for which member attributes should not be checked
 # (useful for modules/projects where namespaces are manipulated during runtime
 # and thus existing member attributes cannot be deduced by static analysis. It
 # supports qualified module names, as well as Unix pattern matching.
-ignored-modules=numpy,numpy.*,scipy.stats,scipy.spatial
+ignored-modules=numpy,numpy.*,scipy,scipy.spatial,scipy.stats,scipy.spatial.qhull
```

### Comparing `neurom-3.2.9/pyproject.toml` & `neurom-4.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     'matplotlib>=3.2.1',
     'morphio>=3.3.6',
     'numpy>=1.8.0',
     'pandas>=1.0.5',
     'pyyaml>=3.10',
     'scipy>=1.2.0',
     'tqdm>=4.8.4',
+    'cached_property>=1.5.1',
     'importlib_resources>=1.3; python_version < "3.9"',
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 plotly = [
     'plotly>=3.6.0',
@@ -63,7 +64,27 @@
 namespaces = false
 
 [tool.setuptools.package-data]
 "*" = ["morph_check.yaml", "morph_stats.yaml"]
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
+
+[tool.pytest.ini_options]
+testpaths = [
+    "tests",
+]
+
+[tool.black]
+line-length = 100
+target-version = [
+    'py38',
+    'py39',
+    'py310',
+    'py311',
+]
+skip-string-normalization = true
+include = 'neurom\/.*\.py$|tests\/.*\.py$|doc\/source\/conf\.py$|setup\.py$|examples\/.*\.py$'
+
+[tool.isort]
+profile = "black"
+line_length = 100
```

### Comparing `neurom-3.2.9/tox.ini` & `neurom-4.0.0/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -12,46 +12,64 @@
     check-packaging
     py{38,39,310,311,312}
 
 [testenv]
 deps =
     {[base]testdeps}
     pytest-cov
+    coverage[toml]>=6.3
 extras = plotly
-commands = pytest \
-                --cov={envsitepackagesdir}/{[base]name} \
+commands = python -m pytest \
+                --cov={[base]name} \
                 --cov-report term-missing \
                 --cov-fail-under=100 \
                 --cov-report=xml \
                 --no-cov-on-fail \
                 {posargs}
 
 [testenv:lint]
-basepython=python3.8
 deps =
+    isort
+    black
     pycodestyle
     pydocstyle
     astroid
     pylint
 commands =
+    isort --check-only --diff {[base]name}
+    black --check .
     pycodestyle --exclude=tests neurom
     pydocstyle --match-dir='(?!test).*' {toxinidir}/neurom
     pylint --rcfile=pylintrc --extension-pkg-whitelist=numpy --ignore=tests neurom
 
+[testenv:format]
+skip_install = true
+deps =
+    isort
+    black
+commands =
+    isort {[base]name}
+    black .
+
 [testenv:docs]
-basepython=python3.9
-changedir = doc
 extras = docs
 commands =
-    # remove autosummary output
-    rm -rf {toxinidir}/doc/source/_neurom_build
-    make clean
-    make html SPHINXOPTS=-W
+    # remove autosummary output and cleanup
+    rm -rf {toxinidir}/doc/source/_neurom_build {toxinidir}/doc/build/*
+    sphinx-build -b doctest \
+        {toxinidir}/doc/source \
+        {toxinidir}/doc/build/doctest \
+        -d {toxinidir}/doc/build/doctrees \
+        -W
+    sphinx-build -b html \
+        {toxinidir}/doc/source \
+        {toxinidir}/doc/build/html \
+        -d {toxinidir}/doc/build/doctrees \
+        -W
 allowlist_externals =
-    make
     rm
 
 [testenv:tutorial]
 changedir = {toxinidir}/tutorial
 extras = plotly
 deps =
     {[base]testdeps}
@@ -67,14 +85,16 @@
     twine
 commands =
     python -m build -o {envtmpdir}/dist
     twine check {envtmpdir}/dist/*
 
 [pycodestyle]
 max-line-length=100
+# E203,W503 needed for black
+ignore = E203,W503
 
 [pydocstyle]
 convention = google
 
 [gh-actions]
 python =
   3.8: py38, lint
```

