# Comparing `tmp/morph-tool-2.9.0.tar.gz` & `tmp/morph-tool-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/morph-tool-2.9.0.tar", last modified: Mon Aug 30 10:40:39 2021, max compression
+gzip compressed data, was "morph-tool-2.9.1.tar", last modified: Mon Jun 20 13:52:30 2022, max compression
```

## Comparing `morph-tool-2.9.0.tar` & `morph-tool-2.9.1.tar`

### file list

```diff
@@ -1,145 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2021-08-30 10:40:10.000000 morph-tool-2.9.0/examples/draw_morphology.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-08-30 10:40:10.000000 morph-tool-2.9.0/examples/dendrogram_plain_example.swc
--rw-r--r--   0 runner    (1001) docker     (121)     3418 2021-08-30 10:40:10.000000 morph-tool-2.9.0/examples/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-08-30 10:40:10.000000 morph-tool-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/functional_tests/
--rw-r--r--   0 runner    (1001) docker     (121)    10180 2021-08-30 10:40:10.000000 morph-tool-2.9.0/functional_tests/circle_contour.asc
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-08-30 10:40:10.000000 morph-tool-2.9.0/functional_tests/test_nrnhines_mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    13568 2021-08-30 10:40:10.000000 morph-tool-2.9.0/functional_tests/circle_contour.h5
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-08-30 10:40:10.000000 morph-tool-2.9.0/functional_tests/soma_three_points_cylinder.swc
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-08-30 10:40:10.000000 morph-tool-2.9.0/functional_tests/morphio.swc
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-08-30 10:40:10.000000 morph-tool-2.9.0/functional_tests/single-point-soma.swc
--rw-r--r--   0 runner    (1001) docker     (121)    58421 2021-08-30 10:40:10.000000 morph-tool-2.9.0/functional_tests/Neuron.swc
--rw-r--r--   0 runner    (1001) docker     (121)   216477 2021-08-30 10:40:10.000000 morph-tool-2.9.0/functional_tests/real_neuron.asc
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-08-30 10:40:10.000000 morph-tool-2.9.0/functional_tests/simple.asc
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2021-08-30 10:40:10.000000 morph-tool-2.9.0/functional_tests/circle_contour.swc
--rw-r--r--   0 runner    (1001) docker     (121)    20070 2021-08-30 10:40:10.000000 morph-tool-2.9.0/functional_tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)   219780 2021-08-30 10:40:10.000000 morph-tool-2.9.0/functional_tests/real_neuron2.asc
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-08-30 10:40:10.000000 morph-tool-2.9.0/ACKNOWLEDGMENT.md
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-08-30 10:40:10.000000 morph-tool-2.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2021-08-30 10:40:10.000000 morph-tool-2.9.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2021-08-30 10:40:10.000000 morph-tool-2.9.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12376 2021-08-30 10:40:39.000000 morph-tool-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2021-08-30 10:40:10.000000 morph-tool-2.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-08-30 10:40:10.000000 morph-tool-2.9.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/morph_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-08-30 10:40:39.000000 morph-tool-2.9.0/morph_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-08-30 10:40:39.000000 morph-tool-2.9.0/morph_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-08-30 10:40:39.000000 morph-tool-2.9.0/morph_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12376 2021-08-30 10:40:39.000000 morph-tool-2.9.0/morph_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-30 10:40:39.000000 morph-tool-2.9.0/morph_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3583 2021-08-30 10:40:39.000000 morph-tool-2.9.0/morph_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-08-30 10:40:10.000000 morph-tool-2.9.0/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/morph_tool/
--rw-r--r--   0 runner    (1001) docker     (121)     2744 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/axon_point.py
--rw-r--r--   0 runner    (1001) docker     (121)     3779 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/morphio_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)    11772 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/nrnhines.py
--rw-r--r--   0 runner    (1001) docker     (121)    16497 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/morphdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     7524 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/resampling.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2651 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5569 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/graft.py
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     9820 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/morph_tool/plot/
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/plot/consts.py
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7448 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/plot/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     4910 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/plot/morphology.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6299 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/neuron_surface.py
--rw-r--r--   0 runner    (1001) docker     (121)     8225 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     3366 2021-08-30 10:40:10.000000 morph-tool-2.9.0/morph_tool/apical_point.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2021-08-30 10:40:10.000000 morph-tool-2.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-08-30 10:40:10.000000 morph-tool-2.9.0/COPYING.LESSER
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      537 2021-08-30 10:40:10.000000 morph-tool-2.9.0/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-08-30 10:40:10.000000 morph-tool-2.9.0/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-08-30 10:40:10.000000 morph-tool-2.9.0/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (121)     9209 2021-08-30 10:40:10.000000 morph-tool-2.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2021-08-30 10:40:10.000000 morph-tool-2.9.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/doc/source/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-08-30 10:40:10.000000 morph-tool-2.9.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-08-30 10:40:10.000000 morph-tool-2.9.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      259 2021-08-30 10:40:10.000000 morph-tool-2.9.0/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4082 2021-08-30 10:40:10.000000 morph-tool-2.9.0/doc/source/morphdb.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4251 2021-08-30 10:40:10.000000 morph-tool-2.9.0/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    10079 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_resampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     3454 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     7456 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_morphdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     4549 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_graft.py
--rw-r--r--   0 runner    (1001) docker     (121)     6686 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     6454 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2781 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_nrnhines.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_spatial.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_axon_point.py
--rw-r--r--   0 runner    (1001) docker     (121)     2360 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/test_apical_point.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/tests/data/folder/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/folder/a.h5
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/folder/d
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/folder/b.swc
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/folder/c.blah
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/tests/data/folder/subfolder/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/folder/subfolder/g.SWC
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/folder/subfolder/e.h5
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/folder/subfolder/f.bla
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/tests/data/morphdb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/tests/data/morphdb/from_neurondb/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_neurondb/neurondb-msubtype.xml
--rw-r--r--   0 runner    (1001) docker     (121)      871 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_neurondb/expected.csv
--rw-r--r--   0 runner    (1001) docker     (121)   212416 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_neurondb/tkb061126a4_ch0_cc2_h_zk_60x_1.h5
--rw-r--r--   0 runner    (1001) docker     (121)     3237 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_neurondb/neurondb.xml
--rw-r--r--   0 runner    (1001) docker     (121)      859 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_neurondb/features.csv
--rw-r--r--   0 runner    (1001) docker     (121)      550 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_neurondb/single-axon-input.neurondb
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_neurondb/simple3.asc
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_neurondb/neurondb-only-dat-info.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/tests/data/morphdb/from_folder_duplicates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_folder_duplicates/a.h5
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_folder_duplicates/a.swc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/tests/data/morphdb/from_folder/
--rw-r--r--   0 runner    (1001) docker     (121)      410 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_folder/expected.csv
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_folder/simple2.swc
--rw-r--r--   0 runner    (1001) docker     (121)    10336 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/morphdb/from_folder/simple.h5
--rw-r--r--   0 runner    (1001) docker     (121)   727793 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/tkb061126a4_ch0_cc2_h_zk_60x_1.asc
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/not_single_child.asc
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/simple2.asc
--rw-r--r--   0 runner    (1001) docker     (121)    10336 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/apical_test.h5
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/apical_test.swc
--rw-r--r--   0 runner    (1001) docker     (121)   212416 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/tkb061126a4_ch0_cc2_h_zk_60x_1.h5
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/synthesized_cell.asc
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/simple2.swc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/tests/data/input-convert/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/input-convert/simple2.asc
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/input-convert/simple3.asc
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/neurondb.dat
--rw-r--r--   0 runner    (1001) docker     (121)     3237 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/neurondb.xml
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/single_child.asc
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/simple3.asc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:39.000000 morph-tool-2.9.0/tests/data/test-neurondb-with-path/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/test-neurondb-with-path/C270106C.wrongext
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/test-neurondb-with-path/C270106A.h5
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/test-neurondb-with-path/a_neuron.ASC
--rw-r--r--   0 runner    (1001) docker     (121)      805 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/neurondb-no-repair.xml
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/simple.swc
--rw-r--r--   0 runner    (1001) docker     (121)      548 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/simple.asc
--rw-r--r--   0 runner    (1001) docker     (121)   727750 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/neuron.asc
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/no_axon.swc
--rw-r--r--   0 runner    (1001) docker     (121)      591 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/two_axons.asc
--rw-r--r--   0 runner    (1001) docker     (121)    10336 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/simple.h5
--rw-r--r--   0 runner    (1001) docker     (121)   589072 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/astrocyte.h5
--rw-r--r--   0 runner    (1001) docker     (121)      703 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/neurondb-empty-morph-tag.xml
--rw-r--r--   0 runner    (1001) docker     (121)  1019250 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tests/data/tkb061126a4_ch0_cc2_h_zk_60x_1.swc
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-30 10:40:39.000000 morph-tool-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2021-08-30 10:40:10.000000 morph-tool-2.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.505176 morph-tool-2.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.489176 morph-tool-2.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-06-20 13:52:25.000000 morph-tool-2.9.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.489176 morph-tool-2.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-20 13:52:25.000000 morph-tool-2.9.1/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2022-06-20 13:52:25.000000 morph-tool-2.9.1/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-06-20 13:52:25.000000 morph-tool-2.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2022-06-20 13:52:25.000000 morph-tool-2.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-06-20 13:52:25.000000 morph-tool-2.9.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-06-20 13:52:25.000000 morph-tool-2.9.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-06-20 13:52:25.000000 morph-tool-2.9.1/ACKNOWLEDGMENT.md
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-06-20 13:52:25.000000 morph-tool-2.9.1/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-06-20 13:52:25.000000 morph-tool-2.9.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-06-20 13:52:25.000000 morph-tool-2.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-20 13:52:25.000000 morph-tool-2.9.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-06-20 13:52:25.000000 morph-tool-2.9.1/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-06-20 13:52:25.000000 morph-tool-2.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    12539 2022-06-20 13:52:30.505176 morph-tool-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9256 2022-06-20 13:52:25.000000 morph-tool-2.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.489176 morph-tool-2.9.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-06-20 13:52:25.000000 morph-tool-2.9.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.489176 morph-tool-2.9.1/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-06-20 13:52:25.000000 morph-tool-2.9.1/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-20 13:52:25.000000 morph-tool-2.9.1/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4599 2022-06-20 13:52:25.000000 morph-tool-2.9.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-06-20 13:52:25.000000 morph-tool-2.9.1/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.489176 morph-tool-2.9.1/doc/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (121)   172811 2022-06-20 13:52:25.000000 morph-tool-2.9.1/doc/source/logo/BBP-Morph-Tool.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)     4082 2022-06-20 13:52:25.000000 morph-tool-2.9.1/doc/source/morphdb.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.489176 morph-tool-2.9.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-06-20 13:52:25.000000 morph-tool-2.9.1/examples/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-06-20 13:52:25.000000 morph-tool-2.9.1/examples/dendrogram_plain_example.swc
+-rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-06-20 13:52:25.000000 morph-tool-2.9.1/examples/draw_morphology.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.493176 morph-tool-2.9.1/functional_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)    58421 2022-06-20 13:52:25.000000 morph-tool-2.9.1/functional_tests/Neuron.swc
+-rw-r--r--   0 runner    (1001) docker     (121)    10180 2022-06-20 13:52:25.000000 morph-tool-2.9.1/functional_tests/circle_contour.asc
+-rw-r--r--   0 runner    (1001) docker     (121)    13568 2022-06-20 13:52:25.000000 morph-tool-2.9.1/functional_tests/circle_contour.h5
+-rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-06-20 13:52:25.000000 morph-tool-2.9.1/functional_tests/circle_contour.swc
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-20 13:52:25.000000 morph-tool-2.9.1/functional_tests/morphio.swc
+-rw-r--r--   0 runner    (1001) docker     (121)   216477 2022-06-20 13:52:25.000000 morph-tool-2.9.1/functional_tests/real_neuron.asc
+-rw-r--r--   0 runner    (1001) docker     (121)   219780 2022-06-20 13:52:25.000000 morph-tool-2.9.1/functional_tests/real_neuron2.asc
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-06-20 13:52:25.000000 morph-tool-2.9.1/functional_tests/simple.asc
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-06-20 13:52:25.000000 morph-tool-2.9.1/functional_tests/single-point-soma.swc
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-06-20 13:52:25.000000 morph-tool-2.9.1/functional_tests/soma_three_points_cylinder.swc
+-rw-r--r--   0 runner    (1001) docker     (121)    20070 2022-06-20 13:52:25.000000 morph-tool-2.9.1/functional_tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-06-20 13:52:25.000000 morph-tool-2.9.1/functional_tests/test_nrnhines_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.493176 morph-tool-2.9.1/morph_tool/
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3531 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/apical_point.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/axon_point.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6297 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10499 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5573 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/graft.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16728 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/morphdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/morphio_diff.py
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/neuron_surface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11998 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/nrnhines.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.493176 morph-tool-2.9.1/morph_tool/plot/
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/plot/consts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7520 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/plot/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4911 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/plot/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7570 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/resampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8254 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2681 2022-06-20 13:52:25.000000 morph-tool-2.9.1/morph_tool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.493176 morph-tool-2.9.1/morph_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12539 2022-06-20 13:52:30.000000 morph-tool-2.9.1/morph_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-06-20 13:52:30.000000 morph-tool-2.9.1/morph_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-20 13:52:30.000000 morph-tool-2.9.1/morph_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-20 13:52:30.000000 morph-tool-2.9.1/morph_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2022-06-20 13:52:30.000000 morph-tool-2.9.1/morph_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-20 13:52:30.000000 morph-tool-2.9.1/morph_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-20 13:52:30.505176 morph-tool-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-06-20 13:52:25.000000 morph-tool-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.497176 morph-tool-2.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.501176 morph-tool-2.9.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)    10336 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/apical_test.h5
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/apical_test.swc
+-rw-r--r--   0 runner    (1001) docker     (121)   589072 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/astrocyte.h5
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.501176 morph-tool-2.9.1/tests/data/folder/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/folder/a.h5
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/folder/b.swc
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/folder/c.blah
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/folder/d
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.501176 morph-tool-2.9.1/tests/data/folder/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/folder/subfolder/e.h5
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/folder/subfolder/f.bla
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/folder/subfolder/g.SWC
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.501176 morph-tool-2.9.1/tests/data/input-convert/
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/input-convert/simple2.asc
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/input-convert/simple3.asc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.485176 morph-tool-2.9.1/tests/data/morphdb/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.501176 morph-tool-2.9.1/tests/data/morphdb/from_folder/
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_folder/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    10336 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_folder/simple.h5
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_folder/simple2.swc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.501176 morph-tool-2.9.1/tests/data/morphdb/from_folder_duplicates/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_folder_duplicates/a.h5
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_folder_duplicates/a.swc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.505176 morph-tool-2.9.1/tests/data/morphdb/from_neurondb/
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_neurondb/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_neurondb/features.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_neurondb/neurondb-msubtype.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_neurondb/neurondb-only-dat-info.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_neurondb/neurondb.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_neurondb/simple3.asc
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_neurondb/single-axon-input.neurondb
+-rw-r--r--   0 runner    (1001) docker     (121)   212416 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/morphdb/from_neurondb/tkb061126a4_ch0_cc2_h_zk_60x_1.h5
+-rw-r--r--   0 runner    (1001) docker     (121)   727750 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/neuron.asc
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/neurondb-empty-morph-tag.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/neurondb-no-repair.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/neurondb.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/neurondb.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/no_axon.swc
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/not_single_child.asc
+-rw-r--r--   0 runner    (1001) docker     (121)      548 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/simple.asc
+-rw-r--r--   0 runner    (1001) docker     (121)    10336 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/simple.h5
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/simple.swc
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/simple2.asc
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/simple2.swc
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/simple3.asc
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/single_child.asc
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/synthesized_cell.asc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:30.505176 morph-tool-2.9.1/tests/data/test-neurondb-with-path/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/test-neurondb-with-path/C270106A.h5
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/test-neurondb-with-path/C270106C.wrongext
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/test-neurondb-with-path/a_neuron.ASC
+-rw-r--r--   0 runner    (1001) docker     (121)   727793 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/tkb061126a4_ch0_cc2_h_zk_60x_1.asc
+-rw-r--r--   0 runner    (1001) docker     (121)   212416 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/tkb061126a4_ch0_cc2_h_zk_60x_1.h5
+-rw-r--r--   0 runner    (1001) docker     (121)  1019250 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/tkb061126a4_ch0_cc2_h_zk_60x_1.swc
+-rw-r--r--   0 runner    (1001) docker     (121)      591 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/data/two_axons.asc
+-rw-r--r--   0 runner    (1001) docker     (121)      946 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_apical_point.py
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_axon_point.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3454 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4549 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_graft.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7456 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_morphdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2781 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_nrnhines.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10079 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7237 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6454 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-06-20 13:52:25.000000 morph-tool-2.9.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `morph-tool-2.9.0/examples/draw_morphology.py` & `morph-tool-2.9.1/examples/draw_morphology.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/examples/dendrogram.py` & `morph-tool-2.9.1/examples/dendrogram.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/setup.py` & `morph-tool-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,18 +39,20 @@
     extras_require={
         'nrn': nrn_extras,
         'parallel': parallel_extras,
         'plot': plot_extras,
         'all': plot_extras + parallel_extras + nrn_extras,
         'docs': ['sphinx', 'sphinx-bluebrain-theme'],
     },
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     use_scm_version=True,
     setup_requires=['setuptools_scm'],
 )
```

### Comparing `morph-tool-2.9.0/functional_tests/circle_contour.asc` & `morph-tool-2.9.1/functional_tests/circle_contour.asc`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/functional_tests/test_nrnhines_mapper.py` & `morph-tool-2.9.1/functional_tests/test_nrnhines_mapper.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/functional_tests/circle_contour.h5` & `morph-tool-2.9.1/functional_tests/circle_contour.h5`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/functional_tests/Neuron.swc` & `morph-tool-2.9.1/functional_tests/Neuron.swc`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/functional_tests/real_neuron.asc` & `morph-tool-2.9.1/functional_tests/real_neuron.asc`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/functional_tests/circle_contour.swc` & `morph-tool-2.9.1/functional_tests/circle_contour.swc`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/functional_tests/test_converter.py` & `morph-tool-2.9.1/functional_tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/functional_tests/real_neuron2.asc` & `morph-tool-2.9.1/functional_tests/real_neuron2.asc`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/.pylintrc` & `morph-tool-2.9.1/.pylintrc`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [MESSAGES CONTROL]
-disable=bad-continuation,fixme,invalid-name,len-as-condition,no-else-return,useless-object-inheritance
+disable=fixme,invalid-name,len-as-condition,no-else-return,useless-object-inheritance
 
 [FORMAT]
 # Maximum number of characters on a single line.
 max-line-length=100
 
 [DESIGN]
 # Maximum number of arguments for function / method
@@ -12,15 +12,15 @@
 # with leading underscore
 ignored-argument-names=_.*
 # Maximum number of locals for function / method body
 max-locals=15
 # Maximum number of return / yield for function / method body
 max-returns=6
 # Maximum number of branch for function / method body
-max-branchs=12
+max-branches=12
 # Maximum number of statements in function / method body
 max-statements=50
 # Maximum number of parents for a class (see R0901).
 max-parents=7
 # Maximum number of attributes for a class (see R0902).
 max-attributes=40
 # Minimum number of public methods for a class (see R0903).
```

### Comparing `morph-tool-2.9.0/CHANGELOG.rst` & `morph-tool-2.9.1/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Changelog
 =========
 
-Version 2.8.1
+Version 2.9.0
 -------------
 - use NeuroM dependency of version >= 3.0
 - use pytest instead of nosetests
 
 Version 2.8.0
 -------------
 - Use numpy.isclose in spatial ``point_to_section_segment``. Add new keyword arguments ``rtol``,``atol`` to ``point_to_section_segment``.  (#84)
@@ -45,9 +45,9 @@
 - Fix NestedPool for py38 and CI (#60)
 
 Version 2.4.0
 -------------
 - Make MorphDB.df hashable (#53)
 - Improve feature (#55)
 - Fix resampling issue from numerical imprecision (#58)
-- automatic morphology alignement (#51)
+- automatic morphology alignment (#51)
 - Introduce installation extras to lighten the package as dependency by default (#57)
```

### Comparing `morph-tool-2.9.0/PKG-INFO` & `morph-tool-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: morph-tool
-Version: 2.9.0
+Version: 2.9.1
 Summary: A collection of CLIs and python function related to morphology handling
 Home-page: https://github.com/bluebrain/morph-tool
 Author: Blue Brain Project, EPFL
 License: LGPLv3
-Description: |docs|
+Description: .. image:: doc/source/logo/BBP-Morph-Tool.jpg
+        
+        |docs|
         
         MorphTool
         =========
         
         A toolbox for morphology editing. It aims to provide small helper programs that perform simple tasks.
         
         Currently MorphTool provides:
@@ -102,15 +104,15 @@
         - sections point array
         - sections diameter array
         - sections perimeter array
         - sections number of children
         
         The soma are *not* taken into consideration
         
-        The same functionality is also avalaible through the python API:
+        The same functionality is also available through the python API:
         
         .. code:: python
         
            from morph_tool import diff
         
            # The result can be used as a boolean:
            if diff(filename1, filename2):
@@ -313,25 +315,27 @@
         
         License
         -------
         
         morph-tool is licensed under the terms of the GNU Lesser General Public License version 3.
         Refer to COPYING.LESSER and COPYING for details.
         
-        Copyright (c) 2018-2021 Blue Brain Project/EPFL
+        Copyright (c) 2018-2022 Blue Brain Project/EPFL
         
         .. |docs| image:: https://readthedocs.org/projects/morph-tool/badge/?version=latest
                      :target: https://morph-tool.readthedocs.io/
                      :alt: documentation status
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: nrn
+Provides-Extra: parallel
 Provides-Extra: plot
 Provides-Extra: all
-Provides-Extra: parallel
 Provides-Extra: docs
-Provides-Extra: nrn
```

### Comparing `morph-tool-2.9.0/CONTRIBUTING.md` & `morph-tool-2.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/morph_tool.egg-info/PKG-INFO` & `morph-tool-2.9.1/morph_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: morph-tool
-Version: 2.9.0
+Version: 2.9.1
 Summary: A collection of CLIs and python function related to morphology handling
 Home-page: https://github.com/bluebrain/morph-tool
 Author: Blue Brain Project, EPFL
 License: LGPLv3
-Description: |docs|
+Description: .. image:: doc/source/logo/BBP-Morph-Tool.jpg
+        
+        |docs|
         
         MorphTool
         =========
         
         A toolbox for morphology editing. It aims to provide small helper programs that perform simple tasks.
         
         Currently MorphTool provides:
@@ -102,15 +104,15 @@
         - sections point array
         - sections diameter array
         - sections perimeter array
         - sections number of children
         
         The soma are *not* taken into consideration
         
-        The same functionality is also avalaible through the python API:
+        The same functionality is also available through the python API:
         
         .. code:: python
         
            from morph_tool import diff
         
            # The result can be used as a boolean:
            if diff(filename1, filename2):
@@ -313,25 +315,27 @@
         
         License
         -------
         
         morph-tool is licensed under the terms of the GNU Lesser General Public License version 3.
         Refer to COPYING.LESSER and COPYING for details.
         
-        Copyright (c) 2018-2021 Blue Brain Project/EPFL
+        Copyright (c) 2018-2022 Blue Brain Project/EPFL
         
         .. |docs| image:: https://readthedocs.org/projects/morph-tool/badge/?version=latest
                      :target: https://morph-tool.readthedocs.io/
                      :alt: documentation status
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: nrn
+Provides-Extra: parallel
 Provides-Extra: plot
 Provides-Extra: all
-Provides-Extra: parallel
 Provides-Extra: docs
-Provides-Extra: nrn
```

### Comparing `morph-tool-2.9.0/morph_tool.egg-info/SOURCES.txt` & `morph-tool-2.9.1/morph_tool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 .gitignore
+.pre-commit-config.yaml
 .pylintrc
 .readthedocs.yml
 ACKNOWLEDGMENT.md
+AUTHORS.txt
 CHANGELOG.rst
 CONTRIBUTING.md
 COPYING
 COPYING.LESSER
 MANIFEST.in
 README.rst
 setup.py
@@ -15,14 +17,15 @@
 .github/workflows/run-tox.yml
 doc/Makefile
 doc/source/api.rst
 doc/source/changelog.rst
 doc/source/conf.py
 doc/source/index.rst
 doc/source/morphdb.rst
+doc/source/logo/BBP-Morph-Tool.jpg
 examples/dendrogram.py
 examples/dendrogram_plain_example.swc
 examples/draw_morphology.py
 functional_tests/Neuron.swc
 functional_tests/circle_contour.asc
 functional_tests/circle_contour.h5
 functional_tests/circle_contour.swc
```

### Comparing `morph-tool-2.9.0/COPYING` & `morph-tool-2.9.1/COPYING`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/morph_tool/axon_point.py` & `morph-tool-2.9.1/morph_tool/axon_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module to detect the terminal point of the main axon/"""
+"""Module to detect the terminal point of the main axon."""
 import logging
 import numpy as np
 
 from neurom import COLS
 from morphio import SectionType, IterType
 
 L = logging.getLogger(__name__)
@@ -16,15 +16,15 @@
 
 
 def axon_point_section(morph, direction=None, bbox=None, ignore_axis=2):
     """Estimate axon point as the terminal point of the main axon.
 
     This point is defined as the point for which the sum of the angles with the direction vector
     is minimal. This corresponds to a main axon being a branch that follows best a straight line
-    in the given direction. More constraints can be added with bbox argument, if incorect axon is
+    in the given direction. More constraints can be added with bbox argument, if incorrect axon is
     detected.
 
     Args:
         morph (morphio.Morphology): morphology
         direction (ndarray): estimated direction of main axon, if None [0, -1, 0] is used
         bbox (dict): bbox of the form {'x': [-100, 100], 'y': [-500, -400]}
         ignore_axis (int): axis to ignore in the angle computation, if None, 3d directions are used
```

### Comparing `morph-tool-2.9.0/morph_tool/morphio_diff.py` & `morph-tool-2.9.1/morph_tool/morphio_diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,87 @@
-'''This module provides the MorphIO diff functionality that can be used
-to see if two morphologies are the same or not'''
+"""Functionality that can be used to see if two morphologies are the same or not."""
 import numpy as np
 from morphio import Morphology
 
 
 class DiffResult:
-    '''
-    An object that, when casted as a boolean, is equivalent to True when morphologies differ
-    Additional information about why they differ is stored in DiffResult.info
-    '''
+    """An object that, when casted as a boolean, is equivalent to True when morphologies differ.
+
+    Additional information about why they differ is stored in DiffResult.info.
+    """
 
     def __init__(self, is_different, info=None):
-        '''The DiffResult ctor
+        """The DiffResult constructor.
 
         Args:
             is_different (bool): are the morphologies different
             info (str): Additional information about how morphologies differ
-        '''
+        """
         self._is_different = is_different
         self.info = info
 
     def __bool__(self):
-        '''Returns True if morphologies differ'''
+        """Returns True if morphologies differ."""
         return self._is_different
 
     def __nonzero__(self):
-        '''Returns True if morphologies differ, but for python 2'''
+        """Returns True if morphologies differ, but for python 2."""
         return self.__bool__()
 
 
 def diff(morph1, morph2, rtol=1.e-5, atol=1.e-8):
-    '''
-    Returns a DiffResult object that is equivalent to True when morphologies differ
-    Additional information about why they differ is stored in DiffResult.info
+    """Returns a DiffResult object that is equivalent to True when morphologies differ.
 
+    Additional information about why they differ is stored in DiffResult.info
     Morphologies with different formats can be compared.
-
     Morphologies are considered different if one of the following property differ:
     - number of root sections
     - sections type
     - sections point array
     - sections diameter array
     - sections perimeter array
     - sections number of children
-
     The soma are NOT taken into consideration
 
     Args:
         morph1 (str|morphio.Morphology|morphio.mut.Morphology): a morphology
         morph2 (str|morphio.Morphology|morphio.mut.Morphology): a morphology
         rtol (float): the relative tolerance used for comparing points (see numpy.isclose help)
         atol (float): the absolute tolerance used for comparing points (see numpy.isclose help)
-    '''
-
+    """
     if not isinstance(morph1, Morphology):
         morph1 = Morphology(morph1)
     if not isinstance(morph2, Morphology):
         morph2 = Morphology(morph2)
 
     if len(morph1.root_sections) != len(morph2.root_sections):
         return DiffResult(True,
                           'Both morphologies have a different number of root sections')
 
     for section1, section2 in zip(morph1.iter(), morph2.iter()):
         for attrib in ['points', 'diameters', 'perimeters']:
             val1, val2 = getattr(section1, attrib), getattr(section2, attrib)
             if val1.shape != val2.shape:
                 return DiffResult(True,
-                                  'Attributes Section.{} of:\n'
-                                  '{}\n{}\nhave different shapes: {} vs {}'.format(
-                                      attrib, section1, section2, val1.shape, val2.shape))
+                                  f'Attributes Section.{attrib} of:\n'
+                                  f'{section1}\n'
+                                  f'{section2}\n'
+                                  f'have different shapes: {val1.shape} vs {val2.shape}'
+                                  )
             is_close = np.isclose(val1, val2, rtol=rtol, atol=atol)
             if not is_close.all():
                 first_diff_index = np.where(~is_close)[0][0]
 
                 return DiffResult(True,
                                   f'Attributes Section.{attrib} of:\n'
                                   f'{section1}\n{section2}\nhave the same shape '
                                   'but different values\n'
                                   f'Vector {attrib} differs at index {first_diff_index}: '
                                   f'{val1[first_diff_index]} != {val2[first_diff_index]}')
         if section1.type != section2.type:
-            return DiffResult(True, '{} and {} have different section types'.format(
-                section1, section2))
+            return DiffResult(True,
+                              f'{section1} and {section2} have different section types')
         if len(section1.children) != len(section2.children):
             return DiffResult(True,
-                              '{} and {} have a different number of children'.format(
-                                  section1, section2))
+                              f'{section1} and {section2} have a different number of children')
 
     return DiffResult(False)
```

### Comparing `morph-tool-2.9.0/morph_tool/nrnhines.py` & `morph-tool-2.9.1/morph_tool/nrnhines.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Utils related to the NRN simulator"""
+"""Utils related to the NRN simulator."""
 import logging
 import multiprocessing.pool
 from pathlib import Path
 from typing import List, Sequence, Union
 
 import numpy as np
 from neurom import COLS, NeuriteType, iter_sections, load_morphology
@@ -16,15 +16,15 @@
         'morph-tool[nrn] is not installed. Please install: pip install morph-tool[nrn]'
     ) from e
 
 L = logging.getLogger(__name__)
 
 
 def get_NRN_cell(filename: Path):
-    """Returns a NRN cell"""
+    """Returns a NRN cell."""
     try:
         # pylint: disable=import-outside-toplevel
         from bluepyopt import ephys
     except ImportError as e_:
         raise ImportError(
             'bluepyopt not installed; please use `pip install morph-tool[nrn]`') from e_
     m = ephys.morphologies.NrnFileMorphology(str(filename))
@@ -41,15 +41,15 @@
 
 def _zero_length_section(section, epsilon=1e-8):
     """Is zero length section ?"""
     return section.length < epsilon
 
 
 def _validate_section(nrn_neuron, nrm_neuron, nrm_idx, nrn_idx):
-    """raise if the mapping NeuroM_section_to_NRN_section is not correct"""
+    """Raise if the mapping NeuroM_section_to_NRN_section is not correct."""
     NRN_sections = list(nrn_neuron.icell.all)
 
     nrm_s = nrm_neuron.sections[nrm_idx]
 
     if nrn_idx is None:
         # The only reason for the mapping not to exist is a zero length section
         # because NRN discards them
@@ -57,41 +57,42 @@
         return
 
     nrn_s = NRN_sections[nrn_idx]
 
     nrn_pts = [nrn_s.x3d(0), nrn_s.y3d(0), nrn_s.z3d(0)]
     nrm_pts = nrm_s.points[0, COLS.XYZ]
 
-    err_msg = ('ERROR Section mismatch: NRN ID ({}) != NeuroM ID ({})'
-               'NRN section:\n{}\n\nNeuroM section:\n{}'.format(
-                   nrn_idx, nrm_idx,
-                   nrn_pts, nrm_pts))
+    err_msg = (f'ERROR Section mismatch: NRN ID ({nrn_idx}) != NeuroM ID ({nrm_idx})'
+               'NRN section:\n'
+               f'{nrn_pts}\n\n'
+               'NeuroM section:\n'
+               f'{nrm_pts}')
     assert_almost_equal(nrn_pts,
                         nrm_pts,
                         decimal=2,
                         err_msg=err_msg)
 
 
 def _validate_section_mapping(NeuroM_cell, NRN_cell, mapping):
-    """raise if the mapping NeuroM_section_to_NRN_section is not correct"""
+    """Raise if the mapping NeuroM_section_to_NRN_section is not correct."""
     for nrm_idx, nrn_idx in mapping.items():
         _validate_section(NRN_cell, NeuroM_cell, nrm_idx, nrn_idx)
 
 
 def NeuroM_section_to_NRN_section(filename: Path):
-    """Returns a mapping from NeuroM section IDs to NRN ones"""
+    """Returns a mapping from NeuroM section IDs to NRN ones."""
     NeuroM_cell = load_morphology(filename)
     NRN_cell = get_NRN_cell(filename)
 
     mapping = {}
 
     NRN_sections = list(NRN_cell.icell.all)
 
     def is_soma(NRN_section):
-        """Is the NRN section a soma section"""
+        """Is the NRN section a soma section."""
         return NRN_section.name().endswith('.soma[0]')
 
     # Skip soma if exists
     counter = 1 if is_soma(NRN_sections[0]) else 0
 
     for NeuroM_section in iter_sections(NeuroM_cell, neurite_order=NeuriteIter.NRN):
         if _zero_length_section(NeuroM_section):
@@ -123,16 +124,15 @@
         counter += 1
 
     _validate_section_mapping(NeuroM_cell, NRN_cell, mapping)
     return mapping
 
 
 def _interpolate_compartments(points, boundaries_segment_ids, boundaries_positions):
-    """
-    Returns the path of each compartment based on its starting and ending position
+    """Returns the path of each compartment based on its starting and ending position.
 
     Args:
         points (numpy.array): a 3D array of the section points
         boundaries_segment_ids (List): the ids of the segment in which each
                                        compartment boundary belongs
         boundaries_positions (List): the 3D positions of the compartment boundaries
     """
@@ -154,21 +154,20 @@
             compartment.append(boundaries_positions[i + 1])
 
         compartment_points.append(np.vstack(compartment))
     return compartment_points
 
 
 def _compartment_paths(points, n_compartments):
-    """
-    Returns the list of paths (list of 3D points) that form each compartment
+    """Returns the list of paths (list of 3D points) that form each compartment.
+
     Args:
         points (numpy.array): a 3D array of points
         n_compartments (int): the number of compartments
     """
-
     segments_directions = np.diff(points, axis=0)
     segment_lengths = np.linalg.norm(segments_directions, axis=1)
     cumulative_pathlength = np.append(0, np.cumsum(segment_lengths))
     pathlengths_at_compartment_boundaries = [
         i * cumulative_pathlength[-1] / float(n_compartments) for i in range(n_compartments)]
 
     boundaries_segment_ids = (np.searchsorted(
@@ -190,50 +189,49 @@
     boundaries_segment_ids.append(len(points) - 1)
     boundaries_positions.append(points[-1])
 
     return _interpolate_compartments(points, boundaries_segment_ids, boundaries_positions)
 
 
 def NeuroM_section_to_NRN_compartment_paths(morph_path: Path):
-    """Returns a dictionary NeuroM section id -> path of each compartment for the section
+    """Returns a dictionary NeuroM section id -> path of each compartment for the section.
 
     Path are formed by following the section points until the pathlength of the compartment is
     reached.
 
     Args:
         morph_path: the morphology path
 
-
     1) Compute the cumulative pathlength along the section segments_directions
     2) Get the compartment pathlengths (compartment are of equal pathlength in a given section)
     3) Compartment by compartment, follow the points until the compartment pathlength is reached
 
 
-    Example for one section:
+    Example for one section::
+
+                       (1, 2) ------ (2, 2)
+                          |
+                          |
+                          |
+        (0, 0) ------- (1, 0)
 
-                   (1, 2) ------ (2, 2)
-                      |
-                      |
-                      |
-    (0, 0) ------- (1, 0)
-
-
-    If n_compartments == 3, three paths are returned:
-    [array([[0.        , 0.        , 0.        ],
-            [1.        , 0.        , 0.        ],
-            [1.        , 0.33333333, 0.        ]]),
-
-     array([[1.        , 0.33333333, 0.        ],
-            [1.        , 1.66666667, 0.        ]]),
-
-     array([[1.        , 1.66666667, 0.        ],
-            [1.        , 2.        , 0.        ],
-            [2.        , 2.        , 0.        ]])]
-    """
 
+    If n_compartments == 3, three paths are returned::
+
+        [array([[0.        , 0.        , 0.        ],
+                [1.        , 0.        , 0.        ],
+                [1.        , 0.33333333, 0.        ]]),
+
+         array([[1.        , 0.33333333, 0.        ],
+                [1.        , 1.66666667, 0.        ]]),
+
+         array([[1.        , 1.66666667, 0.        ],
+                [1.        , 2.        , 0.        ],
+                [2.        , 2.        , 0.        ]])]
+    """
     NeuroM_cell = load_morphology(morph_path)
     NRN_neuron = get_NRN_cell(morph_path)
     NRN_sections = list(NRN_neuron.icell.all)
 
     mapping = NeuroM_section_to_NRN_section(morph_path)
 
     NeuroM_to_compartment_position_mapping = {}
@@ -250,70 +248,73 @@
     return NeuroM_to_compartment_position_mapping
 
 
 def point_to_section_end(sections: Sequence[neuron.nrn.Section],  # pylint: disable=no-member
                          point: List[float],
                          atol: float = 1e-08,
                          rtol: float = 1e-05) -> Union[None, int]:
-    '''Returns the index of the first found section whose end is at a distance less than
-    EPSILON from POINT. If no section satisfies this requirement, returns None
+    """Returns the index of the first section whose end is close to ``point``.
 
-    The iteration order is given by the section index.
+    The distance between the end and ``point`` must be less than EPSILON from POINT. If no section
+    satisfies this requirement, returns None. The iteration order is given by the section index.
 
     Args:
         sections: a sequence of sections
         point: the points's 3D coordinates
         atol: absolute tolerance
         rtol: relative tolerance
-    '''
+    """
     point = np.asarray(point)
 
     for index, section in enumerate(sections):
         last_index = section.n3d() - 1
         last_section_point = [section.x3d(last_index),
                               section.y3d(last_index),
                               section.z3d(last_index)]
 
         if np.isclose(point, last_section_point, atol=atol, rtol=rtol).all():
             return index
     return None
 
 
 class NestedPool(multiprocessing.pool.Pool):  # pylint: disable=abstract-method
-    """Class that represents a MultiProcessing nested pool"""
+    """Class that represents a MultiProcessing nested pool."""
 
     class Process(multiprocessing.Process):
-        """Class that represents a non-daemon process"""
+        """Class that represents a non-daemon process."""
 
         def __init__(self, *args, **kwargs):
             """Ensures group=None to avoid exception from multiprocessing.
 
             Note:
                 The exception raised by multiprocessing is:
                 AssertionError: group argument must be None for now
             """
             kwargs.pop("group", None)
             super().__init__(None, *args[1:], **kwargs)
 
         @property
         def daemon(self):
+            """Stub method. Always returns False."""
             return False
 
         @daemon.setter
         def daemon(self, value):
-            pass
+            """Stub method. Does not do anything."""
 
 
 def isolate(func):
     """Isolate a generic function for independent NEURON instances.
 
     It must be used in conjunction with NestedPool.
 
     Example:
 
+    .. code-block:: python
+
         def _to_be_isolated(morphology_path, point):
             cell = nrnhines.get_NRN_cell(morphology_path)
             return nrnhines.point_to_section_end(cell.icell.all, point)
 
         def _isolated(morph_data):
             return nrnhines.isolate(_to_be_isolated)(*morph_data)
```

### Comparing `morph-tool-2.9.0/morph_tool/morphdb.py` & `morph-tool-2.9.1/morph_tool/morphdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-'''Provides two classes to work with neurondb files
+"""Provides two classes to work with neurondb files.
+
 The main use is to provide a neuronDB loader and a method to retrieve
 information as a dataframe.
 
 Example:
-
-old_release = MorphDB.from_neurondb(Path("/realease/one/neuronDB.xml"), label='old-release')
-new_release = MorphDB.from_neurondb(Path("/realease/two/neuronDB.xml"), label='new-release')
+old_release = MorphDB.from_neurondb(Path("/release/one/neuronDB.xml"), label='old-release')
+new_release = MorphDB.from_neurondb(Path("/release/two/neuronDB.xml"), label='new-release')
 total = old_release + new_release
 
 # neurondb information
 print(total.df)
 
 # combined information (neurondb + morph_stats)
 print(total.features({'neurite': {'section_lengths': ['max']}}))
-'''
+"""
+
 import collections
 import logging
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import pandas as pd
 import xmltodict
@@ -43,23 +44,24 @@
 ]
 
 COLUMNS = ['name', 'mtype', 'msubtype', 'mtype_no_subtype',
            'layer', 'label', 'path'] + BOOLEAN_REPAIR_ATTRS + ['axon_inputs']
 
 
 class MorphInfo:
-    '''A class the contains information about a morphology.
+    """A class the contains information about a morphology.
+
     Its role is to abstract away the raw data.
-    '''
+    """
 
     MTYPE_SEPARATOR = ':'
 
     def __init__(self, name: str, mtype: str, layer: Optional[Union[str, int]] = None,
                  **kwargs):
-        '''MorphInfo ctor:
+        """A MorphInfo constructor.
 
         Upon initialization, all repair attributes are set to True.
 
         Args:
             name: the morphology name (without the extension)
             mtype: the full mtype (ie 'L1_DAC:A')
             layer: the layer (accepts both string and int)
@@ -73,15 +75,15 @@
                 - tuft_dendrite_repair
                 - oblique_dendrite_repair
                 - unravel
                 - use_for_stats
                 - axon_inputs
                 - path
                 - label
-        '''
+        """
         self.name = name
         self.mtype = mtype
         if self.MTYPE_SEPARATOR in mtype:
             self.mtype_no_subtype, self.msubtype = mtype.split(self.MTYPE_SEPARATOR)
         else:
             self.mtype_no_subtype, self.msubtype = self.mtype, ''
         self.layer = str(layer or '')
@@ -91,34 +93,36 @@
 
         self.axon_inputs = kwargs.get('axon_inputs', [])
         self.path = kwargs.get('path')
         self.label = kwargs.get('label')
 
     @classmethod
     def _from_xmldict(cls, item: Dict[str, Any]):
-        '''MorphInfo ctor.
+        """A MorphInfo constructor.
+
         Args:
             item: A dictionary that represents the content of the XML file.
                   The only mandatory keys are [name, mtype, layer]
-        '''
+        """
         morph = cls(
             item['name'],
             cls.MTYPE_SEPARATOR.join(filter(None, [item['mtype'], item.get('msubtype')])),
             item['layer']
         )
 
         def is_true(repair: Dict[str, Any], key: str) -> bool:
-            '''Parse a string representing a boolean repair flag and returns its boolean value
+            """Parse a string representing a boolean repair flag and returns its boolean value.
+
             Unless clearly stated as false, missing tags default to True
             - According to Eilif, an empty use_axon (corresponding to a null in the database)
               means that the axon is supposed to be used
             - dendrite_repair       defaults to True in BlueRepairSDK
             - basal_dendrite_repair defaults to True in BlueRepairSDK
             - unravel: well I guess we always want to do it
-            '''
+            """
             el = repair.get(key)
             if el not in {'true', 'false', 'True', 'False', None}:
                 raise ValueError(f'Invalid XML element {key} has invalid value: {el}\n'
                                  'Allowed values:\n'
                                  '- empty tag (which is equivalent to True)\n'
                                  '- true\n'
                                  '- True\n'
@@ -136,44 +140,46 @@
             (repair.get('axon_sources') or {}).get('axoninput', [])
         ))
 
         return morph
 
     @property
     def row(self) -> List:
-        '''Flattened data structude ready to be used by a dataframe.'''
+        """Flattened data structude ready to be used by a dataframe."""
         return [getattr(self, attr) for attr in COLUMNS]
 
     def __repr__(self):
+        """Overloaded method."""
         return (f'MorphInfo(name={self.name!r}, mtype={self.mtype!r}, layer={self.layer!r}, '
                 f'label={self.label!r})')
 
 
 class MorphDB:
-    '''A MorphInfo container.
+    """A MorphInfo container.
+
     It takes care of maintaining uniqueness of the MorphInfo element
     and methods to write neurondb to various format (xml, dat, csv)
-    '''
+    """
 
     def __init__(self, morph_info_seq: Optional[Iterable[MorphInfo]] = None):
         """Constructor of MorphDB.
 
         Args:
             morph_info_seq: an optional sequence of MorphInfo objects
         """
         self.df = pd.DataFrame([morph_info.row for morph_info in (morph_info_seq or ())],
                                columns=COLUMNS)
         MorphDB._sanitize_df_types(self.df)
 
     @classmethod
     def _from_neurondb_dat(cls, neurondb, morph_paths, label):
-        '''Private constructor from neuronDB.dat files
+        """Private constructor from neuronDB.dat files.
 
         The equivalent public method is MorphDB.from_neurondb
-        '''
+        """
         obj = cls()
         columns = ['name', 'layer', 'mtype']
         obj.df = pd.read_csv(neurondb, sep=r'\s+', names=columns, usecols=range(len(columns)))
 
         fulltypes = obj.df.mtype.str.split(':', n=1, expand=True).fillna('')
         if len(fulltypes.columns) > 1:
             obj.df['mtype_no_subtype'] = fulltypes[0]
@@ -217,26 +223,27 @@
         return obj
 
     @classmethod
     def from_neurondb(cls,
                       neurondb: Union[Path, str],
                       label: str = 'default',
                       morphology_folder: Optional[Union[Path, str]] = None):
-        '''Builds a MorphologyDB from a neurondb.(xml|dat) file
+        """Builds a MorphologyDB from a neurondb.(xml|dat) file.
+
         Args:
             neurondb: path to a neurondb.(xml|dat) file
             label: a unique label to mark all morphologies coming from this neurondb
             morphology_folder: the location of the morphology files, if None it will default
                 to the neurondb folder
 
         Raises: ValueError if the neurondb does not abide by the specification
         https://bbpteam.epfl.ch/documentation/projects/morphology-repair-workflow/latest/input_files.html#specification
 
         ..note:: missing keys are filled with `True` values
-        '''
+        """
         neurondb = Path(neurondb)
         if morphology_folder:
             morphology_folder = Path(morphology_folder)
         else:
             morphology_folder = neurondb.parent.resolve()
 
         morph_paths = {path.stem: path for path in iter_morphology_files(morphology_folder)}
@@ -248,43 +255,46 @@
 
     @classmethod
     def from_folder(cls,
                     morphology_folder: Union[Path, str],
                     mtypes: Iterable[Tuple[str, str]],
                     label: str = 'default',
                     extension: Optional[str] = None):
-        '''Factory method to create a MorphDB object from a folder containing morphologies
+        """Factory method to create a MorphDB object from a folder containing morphologies.
 
         Args:
             morphology_folder: a folder containing morphologies
             mtypes: a sequence of 2-tuples (morphology name, mtype)
             label: (optional) a group label to be used to identify the morphlogies from this folder
-            ext: Specify the morphology format to consider, if the folder contains multiple formats
+            extension: Specify the morphology format to consider, if the folder contains multiple
+                formats
 
         Raises: ValueError if the folder contains multiple files with the same name but
         different extensions and the extension argument has not been provided
-        '''
+        Returns:
+            MorphDB: an instance of MorphDB.
+        """
         files = list(iter_morphology_files(Path(morphology_folder),
                                            extensions={extension} if extension else None))
         if not extension:
             duplicates = [item for item, count in
                           collections.Counter(path.stem for path in files).items()
                           if count > 1]
             if duplicates:
                 raise ValueError(
                     f'Folder {morphology_folder} have multiple morphologies with the same '
                     'name but different extensions. This is not supported.\n'
                     f'Duplicate morphogies: {duplicates}\n\n'
-                    'Please provide the extension to use with the arguement: extension')
+                    'Please provide the extension to use with the argument: extension')
         paths = {path.stem: path for path in files}
         return MorphDB(MorphInfo(name, mtype, label=label, path=paths[name])
                        for name, mtype in mtypes)
 
     def _to_xmldict(self):
-        '''Transform the data to a xmldict compatible dictionary'''
+        """Transform the data to a xmldict compatible dictionary."""
         def get_repair_attr(morph, attr):
             if attr == 'axon_inputs':
                 return 'axon_sources', {'axoninput': getattr(morph, attr)}
             else:
                 return attr, getattr(morph, attr)
 
         return {'neurondb': {'listing': {
@@ -297,84 +307,88 @@
                     get_repair_attr(morph, attr)
                     for attr in BOOLEAN_REPAIR_ATTRS + ['axon_inputs']
                 )
             } for morph in self.df.itertuples()]}
         }}
 
     def write(self, output_path: Union[Path, str]):
-        '''Write the neurondb file to XML or DAT format
+        """Write the neurondb file to XML or DAT format.
 
         Args:
             output_path: the output path
-        '''
+        """
         output_path = Path(output_path)
         ext = output_path.suffix.lower()
         if ext == '.dat':
             self.df[['name', 'layer', 'mtype']].to_csv(output_path, sep=' ', header=False,
                                                        index=False)
         elif ext == '.xml':
-            with output_path.open('w') as fd:
+            with output_path.open('w', encoding='utf-8') as fd:
                 fd.write(xmltodict.unparse(self._to_xmldict(), pretty=True))
         else:
             raise ValueError(f'Unsupported neurondb extensions ({ext}).'
                              ' Should be one of: (xml,csv,dat)')
 
     def features(self, config: Dict, n_workers=1):
-        '''Returns a dataframe containing morphometrics and neurondb information
+        """Returns a dataframe containing morphometrics and neurondb information.
 
         Args:
             config: a NeuroM morph_stas config.
                 See https://neurom.readthedocs.io/en/latest/morph_stats.html for more information
             n_workers: the number of workers to use to perform the computations
 
         Returns:
             A jointure dataframe between `neurom.stats.extract_dataframe` and `self.df`
 
         Raises:
             ValueError: if `self.df` has undefined (ie. None) paths
-        '''
+        """
         missing_morphs = self.df[self.df.path.isnull()].name.to_list()
         if missing_morphs:
             raise ValueError(
                 f'DataFrame has morphologies with undefined filepaths: {missing_morphs}')
 
         df = self.df.copy().reset_index(drop=True)
         df.columns = pd.MultiIndex.from_product((["properties"], df.columns.values))
         stats = extract_dataframe(df.loc[:, ('properties', 'path')], config, n_workers)
         return df.join(stats.drop(columns='name', level=1), how='inner')
 
     def check_files_exist(self):
-        '''Raises if `self.df.path` has None values or non existing paths'''
+        """Raises if `self.df.path` has None values or non existing paths."""
         missing_morphs = self.df[self.df.path.isnull()].name.values
         if missing_morphs:
             raise ValueError(
                 f'DataFrame has morphologies with undefined filepaths: {missing_morphs}')
 
         for path in self.df['path']:
             if not path.exists():
                 raise ValueError(f'Non existing path: {path}')
 
     def __add__(self, other):
+        """Overloaded method."""
         obj = MorphDB()
         obj += self
         obj += other
         return obj
 
     def __iadd__(self, other):
+        """Overloaded method."""
         if isinstance(other, MorphDB):
             self.df = pd.concat([self.df, other.df])
             MorphDB._sanitize_df_types(self.df)
         else:
             raise TypeError(f'Must be MorphDB or a sequence of MorphInfo, not {type(other)}')
 
         return self
 
     @staticmethod
     def _create_dataframe(morphologies: List[MorphInfo]):
-        '''Returns a pandas.DataFrame view of the data with the following columns:
+        """Creates a dataframe.
+
+        The dataframe has the following columns:
            'name': the morpho name (without extension)
            'mtype': the mtype with its subtype
            'msubtype': the msubtype (the part of the mtype after the ":")
            'mtype_no_subtype': the mtype without the msubtype
            'layer': the layer (as a string)
            # repair related columns
            'use_axon': states that the morphology's axon can be used as a donor for axon grafting
@@ -388,21 +402,21 @@
            'oblique_dendrite_repair': flag to activate oblique dendrites repair (dendrite_repair
                                     must be true as well)
            'unravel': flag to activate unravelling
            'axon_inputs': the list of morphologies whose axon can be grafted on this morphology
            # deprecated
            'use_for_stats': Legacy flag that was used to determine if an axon was suitable to be
                             used as a axoninput
-        '''
+        """
         df = pd.DataFrame([morph.row for morph in morphologies], columns=COLUMNS)
         MorphDB._sanitize_df_types(df)
         return df
 
     @staticmethod
     def _sanitize_df_types(df):
-        '''Set up the proper types for each columns
+        """Set up the proper types for each columns.
 
         Args:
             df: the dataframe to be sanitized
-        '''
+        """
         df.astype({key: bool for key in BOOLEAN_REPAIR_ATTRS}, copy=False)
         df["axon_inputs"] = df["axon_inputs"].apply(tuple)
```

### Comparing `morph-tool-2.9.0/morph_tool/resampling.py` & `morph-tool-2.9.1/morph_tool/resampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-"""Resampling functionality for morphio morphologies. It allows for the
-generation of new points on the morphology skeleton with different density
+"""Resampling functionality for morphio morphologies.
+
+It allows for the generation of new points on the morphology skeleton with different density.
 """
 import morphio
 import numpy as np
 
 
 def _accumulated_path_lengths(points):
-    """Return the accumulated path lengths along the polygonal line joining
-    the consecutive points, starting with the point of index 0
+    """Return the accumulated path lengths.
+
+    Accumulates along the polygonal line joining the consecutive points, starting with the point
+    of index 0.
 
     Args:
         points (np.ndarray): (N, 3) array of 3D points
 
     Returns:
         path_lengths (np.ndarray): (N,) Accumulated path lengths
 
@@ -24,17 +27,19 @@
     path_lengths = np.empty(len(segment_lengths) + 1, dtype=np.float32)
     path_lengths[0] = 0.
     path_lengths[1:] = np.cumsum(segment_lengths)
     return path_lengths
 
 
 def _resample_from_linear_density(points, linear_density):
-    """Given a polyline of consecutive points that form segments, it creates
-    a new sampling of K points (or point properties) on the same polyline. K
-    is determined from the linear density as points per micron.
+    """Creates a new sampling of K points.
+
+    Given a polyline of consecutive points that form segments, it creates a new sampling of K
+    points (or point properties) on the same polyline. K is determined from the linear density
+    as points per micron.
 
     Each new point / property is determined via two values: a starting point
     at positional id i in the points array i and a fraction along the segment formed
     by the consecutive points (points[i], points[i+1]). Thus, we have:
 
     v'[k] = v[ids[k]] + fractions[k] * (v[ids[k] + 1] - v[ids[k]])
 
@@ -64,15 +69,14 @@
         new_points = points[ids] + fractions * (points[ids + 1] - points[ids])
 
         Similarly, point properties (e.g. diameters) can be interpolated:
 
         new_diams = diams[ids] + fractions * (diams[ids + 1] - diams[ids])
 
     Notes:
-
         It doesn't not return the ids and fractions for first and last points in
         the new resampling, because they should remain unchanged. Therefore, the
         total number of ids and fractions is K-2.
     """
     path_lengths = _accumulated_path_lengths(points)
     total_length = path_lengths[-1]
 
@@ -91,20 +95,19 @@
     # in the parametric equation of the line segment p0 + t * (p1 - p0)
     fractions = (new_path_lengths - path_lengths[ids]) / (path_lengths[ids + 1] - path_lengths[ids])
 
     return ids, fractions
 
 
 def _parametric_values(values, ids, fractions):
-    """It creates a new array of values, where the start and end
-    values remain unchanged and the in-between values are calculated
-    from the parametric equation:
+    """Creates a new array of values.
 
+    The start and the end values remain unchanged and the in-between values are calculated
+    from the parametric equation:
     v'[k] = v[ids[k]] + fractions[k] * (v[ids[k] + 1] - v[ids[k]])
-
     See _resample_from_linear_density for more details on ids and fractions
 
     Args:
         values (np.ndarray): 1D or 2D array of values
             Points or any property defined on points can be interpolated
             using this function.
         ids (np.ndarray): (N,) Array of ints
@@ -132,53 +135,52 @@
     new_values[1:-1] = values[ids] + fractions * (values[ids + 1] - values[ids])
 
     return new_values
 
 
 def _resample_neuron_section(section, linear_density):
     """Resample in-place the section data based on linear density.
+
     Args:
         section (Section): Mutable morphology's section
         linear_density (float): Number of points per micron
     """
     points = section.points
     ids, fractions = _resample_from_linear_density(points, linear_density)
     section.points = _parametric_values(points, ids, fractions)
     section.diameters = _parametric_values(section.diameters, ids, fractions)
 
 
 def _resample_astrocyte_section(section, linear_density):
     """Resample in-place the section data based on linear density.
+
     Args:
         section (Section): Mutable morphology's section
         linear_density (float): Number of points per micron
     """
     points = section.points
     ids, fractions = _resample_from_linear_density(points, linear_density)
     section.points = _parametric_values(points, ids, fractions)
     section.diameters = _parametric_values(section.diameters, ids, fractions)
     section.perimeters = _parametric_values(section.perimeters, ids, fractions)
 
 
 def _dispatch_section_function(cell_family):
-    """Returns section function depending on the cell_family
-    of the morphology
-    """
+    """Returns section function depending on the cell_family of the morphology."""
     return {
         morphio.CellFamily.NEURON: _resample_neuron_section,
         morphio.CellFamily.GLIA: _resample_astrocyte_section
     }[cell_family]
 
 
 def resample_linear_density(obj, linear_density):
-    """Returns a new morphology with new points and point properties,
-    the number of which depends on the linear_density. The new
-    values are linearly interpolated from the old ones.
+    """Returns a new morphology with new points and point properties.
 
-    This function is useful for use cases where morphologies have too
+    The number of points depends on the linear_density. The new values are linearly interpolated
+    from the old ones. This function is useful for use cases where morphologies have too
     many points and a resampling with fewer points/properties is required.
 
     Args:
         obj: Morphology object, mutable or immutable
         linear_density (float): Number of points per micron
 
     Returns:
```

### Comparing `morph-tool-2.9.0/morph_tool/utils.py` & `morph-tool-2.9.1/morph_tool/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,78 @@
-'''Utils'''
+"""Utils."""
 from functools import partial
 from pathlib import Path
 from typing import Optional
 
 import pandas as pd
 from deprecation import deprecated
 
 
 def is_morphology(filename, extensions=None):
-    '''Returns True if the extension is supported'''
+    """Returns True if the extension is supported."""
     extensions = extensions or {'asc', 'h5', 'swc'}
     return Path(filename).suffix[1:].lower() in extensions
 
 
 def iter_morphology_files(folder, recursive=False, extensions=None):
-    '''Iterator that returns path to morphology files'''
+    """Iterator that returns path to morphology files."""
     extensions = extensions or {'asc', 'h5', 'swc'}
     if recursive:
         files = Path(folder).rglob('*')
     else:
         files = Path(folder).glob('*')
     return filter(partial(is_morphology, extensions=extensions), files)
 
 
 def find_morph(folder: Path, stem: str) -> Optional[Path]:
-    '''Returns the path to a morphology in morphology_dir matching stem.
+    """Returns the path to a morphology in morphology_dir matching stem.
 
     If no morphology is found, returns None
-    '''
+    """
     for ext in ('.asc', '.ASC', '.h5', '.H5', '.swc', '.SWC'):
         path = folder / (stem + ext)
         if path.exists():
             return path
     return None
 
 
 def _ensure_list(data):
-    '''Returns the data if already a list else [data].
+    """Returns the data if already a list else [data].
 
     xmltodict.parse will represent the data as a list if it sees
     the same tag multiple times in a row. For example,
     <morphology></morphology> will appear multiple times in neuronDB.xml
 
     However if the neurondb has a single <morphology></morphology> tag the data
     won't be represented as a list so this function enforce it
 
     Args:
         data: the python dict coming from xmltodict.parse.
 
-    '''
+    """
     if isinstance(data, list):
         return data
     return [data]
 
 
 @deprecated(details='Use `morph_tool.morphdb.MorphDB` instead.')
 def neurondb_dataframe(neurondb: Path, morphology_dir: Optional[Path] = None) -> pd.DataFrame:
-    '''Returns a DataFrame: [name, layer, mtype, use_axon, (optional) path]
+    """Returns a DataFrame.
+
+    The expected columns: name, layer, mtype, use_axon, (optional) path. If read from an XML,
+    additional columns maybe be present.
 
-    If read from an XML, additional columns maybe be present
     Args:
-        filename: the neurondb.(dat|xml) file
+        neurondb: the neurondb.(dat|xml) file
         morphology_dir: (Optional) If passed, a column with the path to each morphology file
             will be added
 
     Raises: ValueError if the neurondb does not abide by the specification
     https://bbpteam.epfl.ch/documentation/projects/morphology-repair-workflow/latest/input_files.html#specification
-    '''
+    """
     from morph_tool.morphdb import MorphDB  # pylint: disable=import-outside-toplevel,cyclic-import
     df = MorphDB.from_neurondb(neurondb, morphology_folder=morphology_dir).df
     columns = ['name', 'layer', 'mtype', 'use_axon']
     if not pd.isnull(df.path).all():
         columns.append('path')
     df = df[columns]
     return df
```

### Comparing `morph-tool-2.9.0/morph_tool/graft.py` & `morph-tool-2.9.1/morph_tool/graft.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-'''What we call grafting is the process of taking one piece of a neuron and
-putting it on another neuron.'''
+"""Grafting is the process of taking one piece of a neuron and putting it on another neuron."""
 import logging
 
 import numpy as np
 from morphio import SectionType, SomaType, Section as ImmutSection
 from morphio.mut import Section
 
 
@@ -15,20 +14,19 @@
 
 
 def find_axon(axon_or_donor_axon):
     """Find the root section which is an axon.
 
     If the number of axons found is greater than 1, then return the first axon.
     """
-
     if isinstance(axon_or_donor_axon, (ImmutSection, Section)):
         if axon_or_donor_axon.type == SectionType.axon:
             return axon_or_donor_axon
         else:
-            raise MorphToolException('The section: {} is not an axon'.format(axon_or_donor_axon))
+            raise MorphToolException(f'The section: {axon_or_donor_axon} is not an axon')
 
     axons = [root for root in axon_or_donor_axon.root_sections
              if root.type == SectionType.axon]
 
     if not axons:
         raise NoAxonException('No axon found!')
 
@@ -54,110 +52,108 @@
     cos_angle = dendrite_mean_direction.dot(
         axon_dir) / np.linalg.norm(dendrite_mean_direction) / np.linalg.norm(axon_dir)
     return np.arccos(cos_angle)
 
 
 def _rotation_around_axis(axis, angle):
     """Returns a rotation matrix around the selected axis by an angle."""
-    d = np.array(axis, dtype=np.float) / np.linalg.norm(axis)
+    d = np.array(axis, dtype=float) / np.linalg.norm(axis)
 
     sn = np.sin(angle)
     cs = np.cos(angle)
 
-    eye = np.eye(3, dtype=np.float)
+    eye = np.eye(3, dtype=d.dtype)
     skew = np.array([[0, -d[2], d[1]],
                      [d[2], 0, -d[0]],
-                     [-d[1], d[0], 0]], dtype=np.float)
+                     [-d[1], d[0], 0]], dtype=d.dtype)
 
     mtx = eye + sn * skew + (1. - cs) * np.linalg.matrix_power(skew, 2)
     return mtx
 
 
 def _rotate_vector(vec, axis, angle):
-    """Rotates the input vector vec
-       by a selected angle
-       around a specific axis.
-    """
+    """Rotates ``vec`` by a selected ``angle`` around a specific ``axis``."""
     return np.dot(_rotation_around_axis(axis, angle), vec)
 
 
 def _random_direction(axis, angle, rng=np.random):
-    '''Returns an direction that makes an theta angle 'angle'
-    with 'axis' and that has a random phi angle in [0, 2 pi]'''
+    """Returns a direction that makes an ``angle`` with ``axis``.
+
+    And that has a random phi angle in [0, 2 pi].
+    """
     orthogonal = np.cross(axis, [0, 0, 1])
     if np.linalg.norm(orthogonal) < 1e-7:
         orthogonal = np.cross(axis, [0, 1, 0])
 
     orthogonal = _rotate_vector(orthogonal, axis, rng.uniform(low=0., high=2. * np.pi))
     vec = _rotate_vector(axis, orthogonal, angle)
     vec /= np.linalg.norm(vec)
     return vec
 
 
 def _section_initial_direction(section):
-    '''Returns the section initial direction'''
+    """Returns the section initial direction."""
     direction = section.points[1] - section.points[0]
 
     # In case of duplicate points, we skip first point
     if np.linalg.norm(direction) < 1e-8:
         return section.points[2] - section.points[1]
     return direction
 
 
 def _soma_mean_radius(neuron, soma_center):
-    '''Returns the soma mean radius'''
+    """Returns the soma mean radius."""
     if neuron.soma_type == SomaType.SOMA_SINGLE_POINT:
         return neuron.soma.diameters[0] / 2.
     else:
         return np.mean(np.linalg.norm(neuron.soma.points - soma_center, axis=1))
 
 
 def grafting_position(neuron, axon_or_donor_neuron, rng=np.random):
-    '''Find out where to put the grafted axon
-
-    If the neuron to be grafted already has a neuron reuse its starting point
+    """Find out where to put the grafted axon.
 
+    If the neuron to be grafted already has a neuron reuse its starting point.
     Otherwise try to mimic the position of the axon with respect to dendrites in
-    the donor axon. The position is choosen in order to
+    the donor axon. The position is chosen in order to
     preserve the direction between the axon initial segment direction
     and all other dendrites initial segments directions
 
     Returns:
         The position where to graft the neuron
-    '''
+    """
     try:
         old_axon = find_axon(neuron)
         return old_axon.points[0]
     except NoAxonException:
         axon_direction = _random_direction(axis=_dendrites_mean_direction(neuron),
                                            angle=_axon_dendrites_angle(axon_or_donor_neuron),
                                            rng=rng)
         soma_center = np.mean(neuron.soma.points, axis=0)
         axon_start = soma_center + _soma_mean_radius(neuron, soma_center) * axon_direction
         return axon_start
 
 
 def delete_old_axons(neuron):
-    '''Delete all axons'''
+    """Delete all axons."""
     for root_section in neuron.root_sections:
         if root_section.type == SectionType.axon:
             neuron.delete_section(root_section)
 
 
 def graft_axon(neuron, axon_or_donor_neuron, rng=np.random):
-    '''Graft an axon
-    args:
-        neuron (morphio.mut.Morphology): Neuron where the axon will be grafted
-        axon_or_donor_neuron (morphio.Morphology): An axon or a neuron with an axon
+    """Graft an axon.
 
-    This is a very simple implementation.
-    No check are performed and the new axon is simply
+    This is a very simple implementation. No check are performed and the new axon is simply
     translated at the place where the old axon was.
-    '''
 
+    Args:
+        neuron (morphio.mut.Morphology): Neuron where the axon will be grafted
+        axon_or_donor_neuron (morphio.Morphology): An axon or a neuron with an axon
+        rng (np.random): function for random generation
+    """
     donor_axon = find_axon(axon_or_donor_neuron)
     position = grafting_position(neuron, axon_or_donor_neuron, rng)
 
     delete_old_axons(neuron)
 
     new_axon = neuron.append_root_section(donor_axon, recursive=True)
```

### Comparing `morph-tool-2.9.0/morph_tool/loader.py` & `morph-tool-2.9.1/morph_tool/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Caching morphology loader.
-"""
+"""Caching morphology loader."""
 
 import os
 
 try:
     from functools import lru_cache
 except ImportError:
     from functools32 import lru_cache
@@ -16,24 +14,24 @@
     if file_ext.startswith("."):
         return file_ext
     else:
         return "." + file_ext
 
 
 class MorphLoader(object):
-    """
-    Caching morphology loader.
-
-    Args:
-        base_dir: path to directory with morphology files
-        file_ext: file extension to look for
-        cache_size: size of LRU cache (if `None`, the cache can grow without bound,
-            if 0, no lru_cache is used)
-    """
+    """Caching morphology loader."""
     def __init__(self, base_dir, file_ext, cache_size=None):
+        """Constructor.
+
+        Args:
+            base_dir: path to directory with morphology files
+            file_ext: file extension to look for
+            cache_size: size of LRU cache (if `None`, the cache can grow without bound,
+                if 0, no lru_cache is used)
+        """
         self.base_dir = base_dir
         self.file_ext = _ensure_startswith_point(file_ext)
         if cache_size == 0:
             self.get = self._get
         else:
             self.get = lru_cache(maxsize=cache_size)(self._get)
```

### Comparing `morph-tool-2.9.0/morph_tool/converter.py` & `morph-tool-2.9.1/morph_tool/converter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''A morphology converter that tries to keep the soma surface equal'''
+"""A morphology converter that tries to keep the soma surface equal."""
 import logging
 from pathlib import Path
 
 import numpy as np
 from morphio import Option, SomaType
 from morphio._morphio import WriterError  # pylint: disable=no-name-in-module
 from morphio.mut import Morphology
@@ -16,15 +16,15 @@
 
 XYZ = slice(3)
 X, Y, Z, R = 0, 1, 2, 3
 cX, cY, cXY = np.s_[:, X], np.s_[:, Y], np.s_[:, :Z]
 
 
 def contourcenter(xyz):
-    '''python implementation of NEURON code: lib/hoc/import3d/import3d_sec.hoc '''
+    """Python implementation of NEURON code lib/hoc/import3d/import3d_sec.hoc."""
     POINTS = 101
 
     points = np.vstack((np.diff(xyz[:, [X, Y]], axis=0), xyz[0, [X, Y]]))
     perim = np.cumsum(np.hstack(((0, ), norm(points, axis=1))))[:-1]
 
     d = np.linspace(0, perim[-1], POINTS)
     new_xyz = np.zeros((POINTS, 3))
@@ -33,20 +33,19 @@
 
     mean = np.mean(new_xyz, axis=0)
 
     return mean, new_xyz
 
 
 def get_sides(points, major, minor):
-    '''
-    Circular permutation of the points so that the point with the largest
-    coordinate along the major axis becomes the last point
-    tobj = major.c.mul(d.x[i])  ###### uneeded? line 1191
-    '''
+    """Circular permutation of the points.
 
+    So that the point with the largest coordinate along the major axis becomes the last point
+    ``tobj = major.c.mul(d.x[i])``  ###### unneeded? line 1191
+    """
     major_coord, minor_coord = np.dot(points, major), np.dot(points, minor)
 
     imax = np.argmax(major_coord)
     # pylint: disable=invalid-unary-operand-type
     major_coord, minor_coord = (np.roll(major_coord, -imax),
                                 np.roll(minor_coord, -imax))
 
@@ -54,24 +53,23 @@
 
     sides = [major_coord[:imin][::-1], major_coord[imin:]]
     rads = [minor_coord[:imin][::-1], minor_coord[imin:]]
     return sides, rads
 
 
 def make_convex(sides, rads):
-    '''Keep only points that make path convex'''
+    """Keep only points that make path convex."""
     def convex_idx(m):
-        '''Return index to elements of m that make it convex
+        """Return index to elements of m that make it convex.
 
         Note: not efficient at the moment
         # now we have the two sides without the min and max points (rads[0]=0)
         # we hope both sides now monotonically increase, i.e. convex
         # make it convex
-
-        '''
+        """
         idx = np.ones_like(m, dtype=bool)
         last_val = m[-1]
         for i in range(len(m) - 2, -1, -1):
             if m[i] < last_val:
                 last_val = m[i]
             else:
                 idx[i] = False
@@ -82,19 +80,19 @@
         sides[i_side] = sides[i_side][ci]
         rads[i_side] = rads[i_side][ci]
 
     return sides, rads
 
 
 def contour2centroid(mean, points):
-    '''this follows the function in
-            lib/hoc/import3d/import3d_gui.hoc
-       most of the comments are from there, so if you want to follow along, it should
-       break up the function the same way
-    '''
+    """This follows the function in lib/hoc/import3d/import3d_gui.hoc.
+
+    Most of the comments are from there, so if you want to follow along, it should
+    break up the function the same way.
+    """
     L.info('Converting soma contour into a stack of cylinders')
 
     # find the major axis of the ellipsoid that best fits the shape
     # assuming (falsely in general) that the center is the mean
 
     points = (points - mean)
     eigen_values, eigen_vectors = eig(np.dot(points.T, points))
@@ -124,55 +122,72 @@
     # avoid 0 diameter ends
     diameters[0] = np.mean(diameters[:2])
     diameters[-1] = np.mean(diameters[-2:])
 
     return points, diameters
 
 
-def _to_sphere(neuron):
-    '''Convert a 3-pts cylinder or a 1-pt sphere into a circular
-    contour that represents the same sphere'''
-    radius = neuron.soma.diameters[0] / 2.
-    N = 20
-    points = np.zeros((N, 3))
-    phase = 2 * np.pi / (N - 1) * np.arange(N)
-    points[:, 0] = radius * np.cos(phase)
-    points[:, 1] = radius * np.sin(phase)
-    points += neuron.soma.points[0]
-    neuron.soma.points = points
-    neuron.soma.diameters = np.repeat(radius, N)
+def _create_contour(radius, point_count=20, line_width=0.25):
+    """Create a contour from an origin and radius.
+
+    Note: The contour is created in the xy plan.
+
+    within the corpus of ASC files, the mean is 0.21 for the diameter.
+    this diameter is used for displaying the width of the contour line in
+    Neurolucida, and 0.25 seems to be a nice display value
+    """
+    points = np.zeros((point_count, 3))
+    phase = 2 * np.pi / point_count * np.arange(point_count)
+    points[:, 0] = radius * np.sin(phase)
+    points[:, 1] = radius * np.cos(phase)
+    diameters = np.repeat(line_width, point_count)
+
+    return points, diameters
 
 
 def cylinder_to_cylindrical_contour(neuron):
-    '''We convert the cylinder into a circular contour that represents the same sphere'''
-    L.info('Converting 3 point soma to sperical soma with same surface')
-    _to_sphere(neuron)
+    """We convert the cylinder into a circular contour that represents the same sphere."""
+    L.info('Converting 3 point soma to spherical soma with same surface')
+    assert neuron.soma_type == SomaType.SOMA_NEUROMORPHO_THREE_POINT_CYLINDERS
+    radius = neuron.soma.diameters[0] / 2.
+    points, diameters = _create_contour(radius)
+    origin = neuron.soma.points[0]
+    neuron.soma.points = points + origin
+    neuron.soma.diameters = diameters
 
 
 def single_point_sphere_to_circular_contour(neuron):
-    '''Transform a single point soma that represents a sphere
-    into a circular contour that represents the same sphere'''
+    """Single point soma to contour soma.
+
+    Transform a single point soma that represents a sphere into a circular contour that represents
+    the same sphere.
+    """
     L.info('Converting 1-point soma (sperical soma) to circular contour '
            'representing the same sphere')
-    _to_sphere(neuron)
+    assert neuron.soma_type == SomaType.SOMA_SINGLE_POINT
+    radius = neuron.soma.diameters[0] / 2.
+    points, diameters = _create_contour(radius)
+    origin = neuron.soma.points[0]
+    neuron.soma.points = points + origin
+    neuron.soma.diameters = diameters
 
 
 def soma_to_single_point(soma):
-    '''surface preserving cylindrical soma to a single point sphere'''
+    """Surface preserving cylindrical soma to a single point sphere."""
     L.info('Converting soma to a single point sphere, while preserving the surface')
     neurom_points = np.hstack((soma.points, 0.5 * soma.diameters[:, None]))
     surface_area = sum(morphmath.segment_area(seg)
                        for seg in zip(neurom_points[1:], neurom_points[:-1]))
 
     soma.points = np.mean(soma.points, axis=0)[None, :]
     soma.diameters = [float((surface_area / np.pi) ** 0.5)]
 
 
 def from_swc(neuron, output_ext):
-    '''Convert to SWC'''
+    """Convert to SWC."""
     if output_ext == 'swc':
         return neuron
 
     if neuron.soma_type == SomaType.SOMA_CYLINDERS:
         L.info('Converting soma stack of cylinders into a contour in the XY plane')
 
         direction = neuron.soma.points[-1] - neuron.soma.points[0]
@@ -192,23 +207,21 @@
     elif neuron.soma_type == SomaType.SOMA_NEUROMORPHO_THREE_POINT_CYLINDERS:
         cylinder_to_cylindrical_contour(neuron)
     elif neuron.soma_type == SomaType.SOMA_SINGLE_POINT:
         if output_ext == 'asc':
             single_point_sphere_to_circular_contour(neuron)
     else:
         raise Exception(
-            'A SWC morphology is not supposed to have a soma of type: {}'.format(
-                neuron.soma_type))
+            f'A SWC morphology is not supposed to have a soma of type: {neuron.soma_type}')
 
     return neuron
 
 
 def from_h5_or_asc(neuron, output_ext):
-    '''Convert from ASC/H5.'''
-
+    """Convert from ASC/H5."""
     if neuron.soma_type == SomaType.SOMA_SINGLE_POINT:
         if output_ext == 'asc':
             single_point_sphere_to_circular_contour(neuron)
     elif neuron.soma_type == SomaType.SOMA_SIMPLE_CONTOUR:
         if output_ext == 'swc':
             mean, new_xyz = contourcenter(neuron.soma.points)
             neuron.soma.points, neuron.soma.diameters = contour2centroid(
@@ -219,25 +232,25 @@
 
 def convert(input_file,
             outputfile,
             recenter=False,
             nrn_order=False,
             single_point_soma=False,
             sanitize=False):
-    '''Run the appropriate converter
+    """Run the appropriate converter.
 
     Args:
         input_file(str): path to input file
         outputfile(str): path to output file
         recenter(bool): whether to recenter the morphology based on the
         center of gravity of the soma
         nrn_order(bool): whether to traverse the neuron in the NEURON fashion
         single_point_soma(bool): For SWC only
         sanitize(bool): whether to sanitize the morphology
-    '''
+    """
     kwargs = {}
     if nrn_order:
         kwargs['options'] = Option.nrn_order
 
     neuron = Morphology(input_file, **kwargs)
     if sanitize:
         neuron.remove_unifurcations()
@@ -255,15 +268,15 @@
     try:
         converter = {'swc': from_swc,
                      'asc': from_h5_or_asc,
                      'h5': from_h5_or_asc,
                      }[neuron.version[0]]
     except KeyError as e:
         raise Exception(
-            'No converter for morphology type: {}'.format(neuron.version)) from e
+            f'No converter for morphology type: {neuron.version}') from e
 
     L.info('Original soma type: %s', neuron.soma_type)
     new = converter(neuron, output_ext)
 
     if single_point_soma:
         soma_to_single_point(new.soma)
```

### Comparing `morph-tool-2.9.0/morph_tool/spatial.py` & `morph-tool-2.9.1/morph_tool/spatial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-'''Module for spatial related functions'''
+"""Module for spatial related functions."""
 import numpy as np
 
 from neurom import COLS
 
 
 def point_to_section_segment(neuron, point, rtol=1e-05, atol=1e-08):
-    '''Find section and segment that matches the point.
+    """Find section and segment that matches the point.
 
     Only the first point found with the *exact* same coordinates as the point argument is considered
 
     Args:
         neuron (morphio.Morphology): neuron object
         point (point): value of the point to find in the h5 file
-        rtol, atol (floats): precission of np.isclose
+        rtol, atol (floats): precision of np.isclose
 
     Returns:
         Tuple: (NeuroM/MorphIO section ID, point ID) of the point the matches the input coordinates.
         Since NeuroM v2, section ids of NeuroM and MorphIO are the same excluding soma.
-    '''
-
+    """
     for section in neuron.iter():
         points = section.points
         offset = np.where(
             np.isclose(points[:, COLS.XYZ], point[COLS.XYZ], rtol=rtol, atol=atol).all(axis=1)
         )
         if offset[0].size:
             return section.id, offset[0][0]
 
-    raise ValueError('Cannot find point in morphology that matches: {}'.format(point))
+    raise ValueError(f'Cannot find point in morphology that matches: {point}')
```

### Comparing `morph-tool-2.9.0/morph_tool/plot/consts.py` & `morph-tool-2.9.1/morph_tool/plot/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""Constants for names that are required to be in columns of ``synapses`` arg of
+"""Constants module.
+
+Constants for names that are required to be in columns of ``synapses`` arg of
 ``morph_tool.plot`` package. These constants are the same as edge properties of `Sonata
 <https://github.com/AllenInstitute/sonata/blob/master/docs/SONATA_DEVELOPER_GUIDE.md#
 edges---optional-reserved-attributes>`__. So you can use these constants, their values as plain
 strings or constants from `bluepysnap <https://github.com/BlueBrain/snap/>`__ library:
 
 An example of using constants or plain strings:
     .. literalinclude:: ../../../examples/dendrogram.py
```

### Comparing `morph-tool-2.9.0/morph_tool/plot/dendrogram.py` & `morph-tool-2.9.1/morph_tool/plot/dendrogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,32 @@
                                     PRE_SECTION_ID, PRE_SECTION_POS)
 
 
 class SynDendrogram(Dendrogram):
     """Dendrogram that keeps track of ``neurom_section.id`` that was used to create it."""
 
     def __init__(self, neurom_section):
+        """Create a dendrogram."""
         super().__init__(neurom_section)
         if isinstance(neurom_section, Morphology):
             self.section_id = -1
             self.children = [
                 SynDendrogram(neurite.root_node) for neurite in neurom_section.neurites]
         else:
             if isinstance(neurom_section, Neurite):
                 neurom_section = neurom_section.root_node
             self.section_id = neurom_section.id
             self.children = [SynDendrogram(child) for child in neurom_section.children]
 
 
 def _draw_polygon(coords, color):
-    path = 'M' + ' L'.join('{:.2f},{:.2f}'.format(coord[0], coord[1]) for coord in coords) + ' Z'
+    path = ('M' +
+            ' L'.join(f'{coord[0]:.2f},{coord[1]:.2f}' for coord in coords) +
+            ' Z'
+            )
 
     return graph_objects.layout.Shape(
         opacity=0.4, type="path", path=path, fillcolor=color, line_color=color)
 
 
 def _draw_line(start, end, color):
     return graph_objects.layout.Shape(
@@ -100,19 +104,19 @@
         pre_section = ((synapses[PRE_SECTION_ID] == dendrogram.section_id)
                        & (synapses[SOURCE_NODE_ID] == neuron_node_id))
         synapses.loc[pre_section, 'x'] = position[0]
         synapses.loc[pre_section, 'y'] = position[1] + synapses.loc[
             pre_section, PRE_SECTION_POS] * dendrogram.height
 
         # jitter too close synapses
-        df = synapses[pre_section | post_section]
+        df = synapses.loc[pre_section | post_section]
         if len(df) > 1:
             # pylint: disable=cell-var-from-loop
             # group by Y coordinate and jitter by X coordinate
-            synapses[pre_section | post_section] = df \
+            synapses.loc[pre_section | post_section] = df \
                 .groupby(lambda idx: round(df.loc[idx, 'y'])) \
                 .apply(_jitter_x)
 
 
 def _add_neurite_legend(fig, dendrogram):
     def neurite_legend(neurite_type):
         fig.add_trace(graph_objects.Scatter(
```

### Comparing `morph-tool-2.9.0/morph_tool/plot/morphology.py` & `morph-tool-2.9.1/morph_tool/plot/morphology.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
                       'will be forced to integer type')
 
 
 def _add_coords(synapse, morphology):
     """Adds coordinates and direction fields to ``synapses`` via ``apply`` function."""
     is_pre = PRE_SECTION_ID in synapse.index and not pd.isnull(synapse[PRE_SECTION_ID])
     is_post = POST_SECTION_ID in synapse.index and not pd.isnull(synapse[POST_SECTION_ID])
-    assert is_pre != is_post, 'Synapse must have either afferent or efferent section ids for the ' \
-                              'morphology. It cant have both at the same time.'
+    assert is_pre != is_post, "Synapse must have either afferent or efferent section ids for the " \
+                              "morphology. It can't have both at the same time."
 
     if is_post:
         sec_id = int(synapse[POST_SECTION_ID])
         seg_id = int(synapse[POST_SEGMENT_ID])
         seg_ofst = float(synapse[POST_SEGMENT_OFFSET])
         synapse['direction'] = 'afferent'
     else:
```

### Comparing `morph-tool-2.9.0/morph_tool/cli.py` & `morph-tool-2.9.1/morph_tool/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''The morph-tool command line launcher'''
+"""The morph-tool command line launcher."""
 import logging
 import sys
 from pathlib import Path
 
 import click
 
 import morph_tool
@@ -14,71 +14,72 @@
 L.setLevel(logging.INFO)
 
 REQUIRED_PATH = click.Path(exists=True, readable=True, dir_okay=False, resolve_path=True)
 
 
 @click.group()
 def cli():
-    '''The CLI entry point'''
+    """The CLI entry point."""
 
 
 @cli.command(short_help='Get soma surface as computed by NEURON')
 @click.argument('input_file', type=REQUIRED_PATH)
 @click.option('--quiet/--no-quiet', default=False)
 def soma_surface(input_file, quiet):
-    '''Get soma surface as computed by NEURON'''
+    """Get soma surface as computed by NEURON."""
     # pylint: disable=import-outside-toplevel
     from morph_tool.neuron_surface import get_NEURON_surface
     if quiet:
         L.setLevel(logging.WARNING)
 
     try:
-        click.echo('Soma surface: {}'.format(get_NEURON_surface(input_file)))
+        click.echo(f'Soma surface: {get_NEURON_surface(input_file)}')
     except ImportError as e:
-        raise ImportError('''the NEURON module is not installed.
+        raise ImportError("""the NEURON module is not installed.
         - if you are on the cluster, you can try: module load nix/hpc/neuron
-        - otherwise, get it here: https://github.com/neuronsimulator/nrn and compile it...'''
+        - otherwise, get it here: https://github.com/neuronsimulator/nrn and compile it..."""
                           ) from e
 
 
 @cli.group()
 def convert():
-    '''Convert a file format between its different representation.
+    """Convert a file format between its different representation.
 
     A special care has been given to the soma conversion as each file format
     has its own representation of the soma.
     While the soma shape cannot be preserved during the conversion,
     the soma surface should be.
 
-    More information at: https://bbpteam.epfl.ch/project/issues/browse/NSETM-458'''
+    More information at: https://bbpteam.epfl.ch/project/issues/browse/NSETM-458
+    """
 
 
 @convert.command(short_help='Convert a single morphology')
 @click.argument('input_file', type=REQUIRED_PATH)
 @click.argument('output_file')
 @click.option('--quiet/--no-quiet', default=False)
 @click.option('--recenter', is_flag=True,
               help='recenter the morphology based on the center of gravity of the soma')
 @click.option('--nrn-order', is_flag=True,
               help='whether to traverse the neuron in the NEURON fashion')
 @click.option('--single-point-soma', is_flag=True, help='For SWC files only')
 @click.option('--sanitize', is_flag=True, help='whether to sanitize the morphology')
 def file(input_file, output_file, quiet, recenter, nrn_order, single_point_soma, sanitize):
-    '''Convert a single morphology from/to the following formats: ASC, SWC, H5'''
+    """Convert a single morphology from/to the following formats: ASC, SWC, H5."""
     if quiet:
         L.setLevel(logging.WARNING)
 
     converter.convert(input_file, output_file, recenter, nrn_order, single_point_soma, sanitize)
 
 
 def _attempt_convert(path, output_dir, extension, recenter, nrn_order, single_point_soma, sanitize):
-    '''Function to be passed to dask.bag.map
+    """Function to be passed to dask.bag.map.
 
     Attempts a conversion and returns the path if it failed
-    '''
+    """
     try:
         converter.convert(path, Path(output_dir) / (path.stem + '.' + extension),
                           recenter, nrn_order, single_point_soma, sanitize)
         return None
     except:  # noqa, pylint: disable=bare-except
         return str(path)
 
@@ -102,15 +103,15 @@
            extension,
            quiet,
            recenter,
            nrn_order,
            single_point_soma,
            sanitize,
            ncores):
-    '''Convert all morphologies in the folder and its subfolders'''
+    """Convert all morphologies in the folder and its subfolders."""
     # pylint: disable=import-outside-toplevel
     try:
         import dask.bag as dask_bag
     except ImportError as e:
         raise ImportError(
             'morph-tool[parallel] is not installed. Run: pip install morph-tool[parallel]'
         ) from e
@@ -139,24 +140,23 @@
 @click.argument('morph2')
 @click.option('--rtol', type=float, default=None, help='The relative tolerance. '
               'See https://numpy.org/doc/stable/reference/generated/numpy.allclose.html')
 @click.option('--atol', type=float, default=None, help='The absolute tolerance. '
               'See https://numpy.org/doc/stable/reference/generated/numpy.allclose.html')
 @click.option('--quiet/--no-quiet', default=False)
 def diff(morph1, morph2, rtol, atol, quiet):
-    '''
-    Compare two morphology files.
+    """Compare two morphology files.
 
     Return exit code 0 if morphology objects stored in `file1` and `file2`
     are deemed identical by MorphIO; and exit code 1 otherwise.
 
     Morphologies with different formats can be compared.
 
     MORPH1 and MORPH2 can be either filenames or morphio.Morpholgy objects
-    '''
+    """
     if quiet:
         L.setLevel(logging.WARNING)
 
     kwargs = {}
     if atol is not None:
         kwargs['atol'] = atol
     if rtol is not None:
```

### Comparing `morph-tool-2.9.0/morph_tool/neuron_surface.py` & `morph-tool-2.9.1/morph_tool/neuron_surface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-'''A utility module to get the surface as computed by neuron'''
+"""A utility module to get the surface as computed by neuron."""
 
 
 def get_NEURON_surface(path):
-    '''Return the soma surface computed by the NEURON simulator. Maybe.'''
+    """Return the soma surface computed by the NEURON simulator."""
     try:
         # pylint: disable=import-outside-toplevel
         from bluepyopt.ephys import simulators, morphologies, models  # pylint: disable=import-error
     except ImportError as e:
         raise ImportError(
             'bluepyopt not installed; please use `pip install morph-tool[nrn]`') from e
```

### Comparing `morph-tool-2.9.0/morph_tool/transform.py` & `morph-tool-2.9.1/morph_tool/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Tools for morphology geometric transformations (translation, rotation, etc).
-"""
+"""Tools for morphology geometric transformations (translation, rotation, etc)."""
 import logging
 from enum import Enum
 import numpy as np
 
 from scipy.spatial.transform import Rotation
 
 from morphio import SectionType, IterType
@@ -22,76 +20,77 @@
     if hasattr(obj, 'soma'):
         obj.soma.points = origin + func(obj.soma.points - origin)
     for s in obj.iter():
         s.points = origin + func(s.points - origin)
 
 
 def transform(obj, A):
-    """
-    Apply transformation matrix `A` to a given morphology object.
+    """Apply transformation matrix `A` to a given morphology object.
 
     Args:
         obj: Morphology / Section
         A: rotation matrix (4 x 4 NumPy array)
     """
     if A is None:
         return
     A = np.asarray(A)
     if A.shape != (4, 4):
-        raise ValueError(
-            "`A` should be 4 x 4 matrix (got instead: %s)" % str(A.shape)
-        )
+        raise ValueError(f"`A` should be 4 x 4 matrix (got: {A.shape})")
     A = A.transpose()
-    func = lambda p: np.dot(np.column_stack((p, np.ones(len(p)))), A)[:, :3]
+
+    def func(p):
+        return np.dot(np.column_stack((p, np.ones(len(p)))), A)[:, :3]
+
     _apply_recursively(func, obj)
 
 
 def rotate(obj, A, origin=(0, 0, 0)):
-    """
-    Apply rotation matrix `A` to a given morphology object.
+    """Apply rotation matrix `A` to a given morphology object.
 
     Args:
         obj: Morphology / Section
         A: rotation matrix (3 x 3 NumPy array)
         origin (3D point): the origin of the rotation
     """
     if A is None:
         return
     A = np.asarray(A)
     if A.shape != (3, 3):
-        raise ValueError(
-            "`A` should be 3 x 3 matrix (got instead: %s)" % str(A.shape)
-        )
+        raise ValueError(f"`A` should be 3 x 3 matrix (got: {A.shape})")
     A = A.transpose()
-    func = lambda p: np.dot(p, A)
+
+    def func(p):
+        return np.dot(p, A)
+
     _apply_recursively(func, obj, origin)
 
 
 def translate(obj, shift):
-    """
-    Apply translation to a given morphology object.
+    """Apply translation to a given morphology object.
 
     Args:
         obj: Morphology / Section
         shift: shift vector ((x, y, z) NumPy array)
     """
     if shift is None:
         return
     shift = np.asarray(shift)
     if shift.shape != (3,):
         raise ValueError(
-            "`shift` should be vector of shape (3,) (got instead: %s)" % str(shift.shape)
+            f"`shift` should be vector of shape (3,) (got: {shift.shape})"
         )
-    func = lambda p: p + shift
+
+    def func(p):
+        return p + shift
+
     _apply_recursively(func, obj)
 
 
 def align(section, direction):
-    '''Rotate a section (and all its descendents) so that its initial segment is oriented along
-    "direction"'''
+    """Rotate a section (and all its descendents) so its initial segment is along ``direction``."""
     section_dir = section.points[1] - section.points[0]
     alpha = angle_between_vectors(section_dir, direction)
     if alpha < 1e-8:
         return
 
     if abs(alpha - np.pi) < 1e-8:
         axis = np.cross(section_dir, [1, 0, 0])
@@ -104,29 +103,29 @@
     axis /= np.linalg.norm(axis)
     matrix = Rotation.from_rotvec(alpha * axis).as_matrix()
 
     rotate(section, matrix, origin=section.points[0])
 
 
 class AlignMethod(Enum):
-    """Contains possible align methods for align_morphology"""
+    """Contains possible align methods for align_morphology."""
 
     WHOLE = 'whole'
     TRUNK = 'trunk'
     FIRST_SECTION = 'first_section'
     FIRST_SEGMENT = 'first_segment'
 
     @classmethod
     def values(cls):
         """Get all possible values."""
         return list(map(lambda c: c.value, cls))
 
 
 def rotation_matrix_from_vectors(vec1, vec2):
-    """ Find the rotation matrix that aligns vec1 to vec2
+    """Find the rotation matrix that aligns vec1 to vec2.
 
     Picked from: https://stackoverflow.com/a/59204638/3868743
     Args:
         vec1: A 3d "source" vector
         vec2: A 3d "destination" vector
 
     Returns:
@@ -173,32 +172,32 @@
             if method == AlignMethod.FIRST_SEGMENT.value:
                 return root_section.points[:2]
 
             return np.vstack([section.points for section in root_section.iter()])
 
 
 def _get_principal_direction(points):
-    '''Return the principal direction of a point cloud
-    It is the eigen vector of the covariance matrix with the highest eigen value.
+    """Return the principal direction of a point cloud.
 
-    Taken from neuror.unravel.'''
+    It is the eigen vector of the covariance matrix with the highest eigen value. Taken from
+    :mod:`neuror.unravel`.
+    """
     X = np.copy(np.asarray(points))
-    X -= np.mean(X, axis=0)
     C = np.dot(X.T, X)
     w, v = np.linalg.eig(C)
     return v[:, w.argmax()]
 
 
 def align_morphology(
     morph, direction=None, method='whole', neurite_type='apical', target_point=None
 ):
     """In-place alignment of a morphology towards a 'direction'.
 
     The base algorithm is based on eigenvalue decomposition of the correlation matrix obtained
-    from points in specified neurites, giving the principal axis of the neurite.
+    from points in specified neurites, giving the principal axis of the neurite, centered at soma.
     Currently, five algorithms are implemented, differing in the choice of points:
 
     1) with method='whole': All the points in the apical dendrite are used.
     2) with method='trunk': Points in section up to the target points are used.
     3) with method='first_section': Only the points in the first section are used.
     4) with method='first_segment': Only the points in the first segment are used.
     5) with method an ndarray or list, we will use it as the direction directly
@@ -211,18 +210,18 @@
         direction (ndarray): 3-vector for final direction, if None, [0, 1, 0] will be used
         method (str|ndarray): method for alignment.
         neurite_type (str): neurite to consider, can only be apical or axon
         target_point (ndarray): position of target point for method='trunk',
             if None and neurite_type='apical', it will be estimated
 
     Returns:
-        3x3 array with applied rotation matrix
+        3x3 array with applied rotation matrix, 3 array with center of rotation
     """
     if isinstance(method, str) and method not in AlignMethod.values():
-        raise NotImplementedError(f"Method {method} is not implementd")
+        raise NotImplementedError(f"Method {method} is not implemented")
 
     if direction is None:
         direction = [0.0, 1.0, 0.0]
     else:
         direction /= np.linalg.norm(direction)
 
     if isinstance(method, (np.ndarray, list)):
@@ -230,14 +229,16 @@
     else:
         points = _get_points(morph, method, neurite_type, target_point)
 
     if points is None:
         L.info('We did not find an apical point to align the morphology')
         return np.eye(3)
 
-    principal_direction = _get_principal_direction(points)
+    center = np.mean(morph.soma.points, axis=0)
+
+    principal_direction = _get_principal_direction(points - center)
     principal_direction *= np.sign(points.dot(principal_direction).sum())
 
     rotation_matrix = rotation_matrix_from_vectors(principal_direction, direction)
-    rotate(morph, rotation_matrix)
+    rotate(morph, rotation_matrix, origin=center)
 
     return rotation_matrix
```

### Comparing `morph-tool-2.9.0/morph_tool/apical_point.py` & `morph-tool-2.9.1/morph_tool/apical_point.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''Module to retrieve the position of the apical point'''
+"""Module to retrieve the position of the apical point."""
 import logging
 import numpy as np
 
 from neurom import COLS
 
 from morphio import SectionType, IterType
 
@@ -10,69 +10,69 @@
 
 
 L = logging.getLogger(__name__)
 
 X, Y, Z = 0, 1, 2
 
 
-def apical_point_section_segment(neuron):
-    '''find the apical point's section and segment
+def apical_point_section_segment(neuron, tuft_percent=20):
+    """Find the apical point's section and segment.
 
     Args:
         neuron (morphio.Morphology): a morphology
+        tuft_percent:
+            percentage of the 'height' of the apical dendrite that would enclose the
+            tuft, only leaves in this volume are considered as endpoints
+            See apical_point_position for more details
 
     Returns:
         Tuple: (NeuroM/MorphIO section ID, point ID) of the apical point. Since NeuroM v2, section
         ids of NeuroM and MorphIO are the same excluding soma.
-    '''
-    point = apical_point_position(neuron)
+    """
+    point = apical_point_position(neuron, tuft_percent)
 
     if point is None:
         L.warning('Could not find apical point')
         return None, None
 
     section, segment = point_to_section_segment(neuron, point)
     return section, segment
 
 
 def apical_point_position(neuron, tuft_percent=20):
-    '''Attempt to find the apical point in 'tufted' neurons
+    """Attempt to find the apical point in 'tufted' neurons.
 
-    The algorithm is a simplification of:
-https://bbpcode.epfl.ch/source/xref/analysis/Pneumatk/pneumatk/__tools__/ \
-    Tree/methods/get_apical_point_index.py
-
-    Consider a neuron:
-
-        |   /    | Tuft = 20%
-        |--/     |
-        |   /
-        |--/
-        |
-    ----.-----
+    Consider a neuron::
+
+            |   /    | Tuft = 20%
+            |--/     |
+            |   /
+            |--/
+            |
+        ----.-----
 
     All endpoints in the top 'tuft_percent' are found, then their common
     branch segment, furthest from the soma, is identified.
 
     Using the release from 2012 as the base, apical points were compared from
     the annotated versions, and using this algorithm.  Of 239 morphologies that
     were annotated, 48 differed in the apical point choice by more than 1um
-    in the y component.  Many of the differences were morphologies that
+    in the y component. Many of the differences were morphologies that
     shoulnd't have had apical points in the first place (ie: weren't pyramidal
-    cells, ex: C050398B-I4.)
+    cells, ex: C050398B-I4).
 
     Args:
-        neuron (morphio.Morphology): a neuron
-        tuft_percent: percentage of the 'height' of the apical dendrite that
-        would enclose the tuft, only leaves in this volume are considered as
-        endpoints
+        neuron (morphio.Morphology): a neuron morphology
+        tuft_percent:
+            percentage of the 'height' of the apical dendrite that would enclose the
+            tuft, only leaves in this volume are considered as endpoints
 
     Returns:
-        neurom.core.point if point is found, or None if it isn't
-    '''
+        neurom.core.dataformat.Point: a point if it is found, or None otherwise
+    """
     apical = [root for root in neuron.root_sections
               if SectionType.apical_dendrite == root.type]
 
     if not len(apical):
         return None
     assert len(apical) >= 1, 'Too many apical dendrites'
     apical = apical[0]
```

### Comparing `morph-tool-2.9.0/COPYING.LESSER` & `morph-tool-2.9.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/.github/workflows/run-tox.yml` & `morph-tool-2.9.1/.github/workflows/run-tox.yml`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8]
+        python-version: [3.7, 3.8, 3.9]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `morph-tool-2.9.0/.github/workflows/publish-sdist.yml` & `morph-tool-2.9.1/.github/workflows/publish-sdist.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 jobs:
   build-n-publish:
     name: Build and publish on PyPI
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@master
-      - name: Set up Python 3.6
+      - name: Set up Python 3.8
         uses: actions/setup-python@v2
         with:
-          python-version: 3.6
+          python-version: 3.8
       - name: Build a source tarball
         run:
             python setup.py sdist
 
       - name: Publish distribution package to PyPI
         uses: pypa/gh-action-pypi-publish@master
         with:
```

### Comparing `morph-tool-2.9.0/README.rst` & `morph-tool-2.9.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. image:: doc/source/logo/BBP-Morph-Tool.jpg
+
 |docs|
 
 MorphTool
 =========
 
 A toolbox for morphology editing. It aims to provide small helper programs that perform simple tasks.
 
@@ -95,15 +97,15 @@
 - sections point array
 - sections diameter array
 - sections perimeter array
 - sections number of children
 
 The soma are *not* taken into consideration
 
-The same functionality is also avalaible through the python API:
+The same functionality is also available through the python API:
 
 .. code:: python
 
    from morph_tool import diff
 
    # The result can be used as a boolean:
    if diff(filename1, filename2):
@@ -306,12 +308,12 @@
 
 License
 -------
 
 morph-tool is licensed under the terms of the GNU Lesser General Public License version 3.
 Refer to COPYING.LESSER and COPYING for details.
 
-Copyright (c) 2018-2021 Blue Brain Project/EPFL
+Copyright (c) 2018-2022 Blue Brain Project/EPFL
 
 .. |docs| image:: https://readthedocs.org/projects/morph-tool/badge/?version=latest
              :target: https://morph-tool.readthedocs.io/
              :alt: documentation status
```

### Comparing `morph-tool-2.9.0/doc/Makefile` & `morph-tool-2.9.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/doc/source/morphdb.rst` & `morph-tool-2.9.1/doc/source/morphdb.rst`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/doc/source/conf.py` & `morph-tool-2.9.1/doc/source/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.napoleon',
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
+    "sphinx.ext.intersphinx",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = []
 
 # The suffix of source filenames.
 source_suffix = '.rst'
@@ -88,14 +89,22 @@
 #modindex_common_prefix = []
 
 autosummary_generate = True
 autosummary_imported_members = False
 autosummary_mock_imports = ['neuron', 'plotly']
 autodoc_default_options = {'members': True}
 
+intersphinx_mapping = {
+    "neurom": ("https://neurom.readthedocs.io/en/stable", None),
+    "neuror": ("https://neuror.readthedocs.io/en/stable", None),
+    "numpy": ("https://numpy.org/doc/stable/", None),
+    "pandas": ("https://pandas.pydata.org/docs", None),
+    "python": ("https://docs.python.org/3", None),
+}
+
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = 'sphinx-bluebrain-theme'
```

### Comparing `morph-tool-2.9.0/tests/test_resampling.py` & `morph-tool-2.9.1/tests/test_resampling.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/test_dendrogram.py` & `morph-tool-2.9.1/tests/test_dendrogram.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/test_diff.py` & `morph-tool-2.9.1/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/test_loader.py` & `morph-tool-2.9.1/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/test_cli.py` & `morph-tool-2.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/test_morphdb.py` & `morph-tool-2.9.1/tests/test_morphdb.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/test_graft.py` & `morph-tool-2.9.1/tests/test_graft.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/test_transform.py` & `morph-tool-2.9.1/tests/test_transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -192,23 +192,34 @@
         )
 
         # Test with whole apical
         morph = morphio.mut.Morphology(DATA / 'apical_test.h5')
         rotation_mat = tested.align_morphology(morph, [0, 0, 1], method="whole")
         npt.assert_almost_equal(
             rotation_mat,
-            [[ 9.9992979e-01, -8.3787108e-03, -8.3790049e-03],
-             [-8.3787108e-03,  7.0207723e-05, -9.9996489e-01],
-             [ 8.3790049e-03,  9.9996489e-01,  0.0000000e+00]],
+            [[ 9.99998738e-01, -1.12359279e-03, -1.12359354e-03],
+             [-1.12359279e-03,  1.26246235e-06, -9.99999404e-01],
+             [ 1.12359354e-03,  9.99999404e-01,  2.22044605e-16]]
         )
 
+        # Test with whole apical on non-centered morphology
+        morph = morphio.mut.Morphology(DATA / 'apical_test.h5')
+        shift = [1.0, 2.0, 3.0]
+        tested.translate(morph, shift)
+        rotation_mat = tested.align_morphology(morph, [0, 0, 1], method="whole")
+        npt.assert_almost_equal(
+            rotation_mat,
+            [[ 9.99998738e-01, -1.12359279e-03, -1.12359354e-03],
+             [-1.12359279e-03,  1.26246235e-06, -9.99999404e-01],
+             [ 1.12359354e-03,  9.99999404e-01,  2.22044605e-16]]
+        )
+
+
         # Test with custom direction
         morph = morphio.mut.Morphology(DATA / 'apical_test.h5')
         rotation_mat = tested.align_morphology(morph, [0, 0, 1], method=[0, 1, 0])
         npt.assert_almost_equal(
             rotation_mat,
             [[ 1,  0,  0],
              [ 0,  0, -1],
              [ 0,  1,  0]]
         )
-
-
```

### Comparing `morph-tool-2.9.0/tests/test_utils.py` & `morph-tool-2.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/test_nrnhines.py` & `morph-tool-2.9.1/tests/test_nrnhines.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/test_spatial.py` & `morph-tool-2.9.1/tests/test_spatial.py`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/test_converter.py` & `morph-tool-2.9.1/tests/test_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pathlib import Path
 import itertools as it
 import numpy as np
+import numpy.testing as npt
 
 import pytest
 
 import morphio
+from morph_tool import converter
 from morph_tool import diff
 from morph_tool.exceptions import MorphToolException
 from morph_tool.converter import convert
 
 DATA = Path(__file__).parent / 'data'
 
 
@@ -52,20 +54,30 @@
     convert(simple, outname, single_point_soma=True)
 
     m = morphio.Morphology(outname)
     assert 1 == len(m.soma.points)
     assert 1 == len(m.soma.diameters)
 
     #value dumped from NEURON: h.area(0.5, sec=icell.soma[0])
-    np.testing.assert_approx_equal(m.soma.surface, 476.0504050847511)
+    npt.assert_approx_equal(m.soma.surface, 476.0504050847511)
 
 
 def test_convert_sanitize(tmpdir):
     # needs to have a complex contour soma
     simple = DATA / 'single_child.asc'
     outname = Path(tmpdir, 'single_child.swc')
     with pytest.raises(MorphToolException, match='Use `sanitize` option for converting'):
         convert(simple, outname, single_point_soma=True)
 
     convert(simple, outname, single_point_soma=True, sanitize=True)
     m = morphio.Morphology(outname)
     assert len(m.sections) == 1
+
+
+def test__create_contour(tmpdir):
+    for point_count in range(3, 20):
+        points, diameters = converter._create_contour(radius=10, point_count=point_count, line_width=0.1)
+        assert len(points) == point_count
+        assert len(diameters) == point_count
+        npt.assert_allclose(points[:, 2], [0]*point_count)
+        npt.assert_allclose(diameters, [0.1]*point_count)
+        assert len(np.unique(np.around(points, decimals=4), axis=0)) == point_count
```

### Comparing `morph-tool-2.9.0/tests/test_apical_point.py` & `morph-tool-2.9.1/tests/test_apical_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DATA = Path(__file__).parent / 'data'
 
 def test_get_apical_point():
     morph = Morphology(DATA / 'apical_test.swc')
     point = apical_point_position(morph)
     assert point[COLS.Y] == 25.0
 
-    # if we only take the very top, we only get one branch, whos common parents
+    # if we only take the very top, we only get one branch, whose common parents
     # is just itself
     point = apical_point_position(morph, tuft_percent=2)
     assert point[COLS.Y] == 30.0
 
     #try w/ a h5v2: this was converted using morphologyConverter
     morph = Morphology(DATA / 'apical_test.h5')
     point = apical_point_position(morph)
```

### Comparing `morph-tool-2.9.0/tests/data/morphdb/from_neurondb/neurondb-msubtype.xml` & `morph-tool-2.9.1/tests/data/morphdb/from_neurondb/neurondb-msubtype.xml`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/morphdb/from_neurondb/expected.csv` & `morph-tool-2.9.1/tests/data/morphdb/from_neurondb/expected.csv`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/morphdb/from_neurondb/tkb061126a4_ch0_cc2_h_zk_60x_1.h5` & `morph-tool-2.9.1/tests/data/morphdb/from_neurondb/tkb061126a4_ch0_cc2_h_zk_60x_1.h5`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/morphdb/from_neurondb/neurondb.xml` & `morph-tool-2.9.1/tests/data/morphdb/from_neurondb/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/morphdb/from_neurondb/features.csv` & `morph-tool-2.9.1/tests/data/morphdb/from_neurondb/features.csv`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/morphdb/from_neurondb/single-axon-input.neurondb` & `morph-tool-2.9.1/tests/data/morphdb/from_neurondb/single-axon-input.neurondb`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/morphdb/from_neurondb/neurondb-only-dat-info.xml` & `morph-tool-2.9.1/tests/data/morphdb/from_neurondb/neurondb-only-dat-info.xml`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/morphdb/from_folder/simple.h5` & `morph-tool-2.9.1/tests/data/morphdb/from_folder/simple.h5`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/tkb061126a4_ch0_cc2_h_zk_60x_1.asc` & `morph-tool-2.9.1/tests/data/tkb061126a4_ch0_cc2_h_zk_60x_1.asc`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/apical_test.h5` & `morph-tool-2.9.1/tests/data/apical_test.h5`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/tkb061126a4_ch0_cc2_h_zk_60x_1.h5` & `morph-tool-2.9.1/tests/data/tkb061126a4_ch0_cc2_h_zk_60x_1.h5`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/neurondb.xml` & `morph-tool-2.9.1/tests/data/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/neurondb-no-repair.xml` & `morph-tool-2.9.1/tests/data/neurondb-no-repair.xml`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/simple.asc` & `morph-tool-2.9.1/tests/data/simple.asc`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/neuron.asc` & `morph-tool-2.9.1/tests/data/neuron.asc`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/two_axons.asc` & `morph-tool-2.9.1/tests/data/two_axons.asc`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/simple.h5` & `morph-tool-2.9.1/tests/data/simple.h5`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/astrocyte.h5` & `morph-tool-2.9.1/tests/data/astrocyte.h5`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/neurondb-empty-morph-tag.xml` & `morph-tool-2.9.1/tests/data/neurondb-empty-morph-tag.xml`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tests/data/tkb061126a4_ch0_cc2_h_zk_60x_1.swc` & `morph-tool-2.9.1/tests/data/tkb061126a4_ch0_cc2_h_zk_60x_1.swc`

 * *Files identical despite different names*

### Comparing `morph-tool-2.9.0/tox.ini` & `morph-tool-2.9.1/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [base]
 name = morph_tool
 testdeps =
     mock
     pytest
     bluepysnap>=0.5
-    pandas<=1.2.5  # 1.3.0 contains an error that breaks tests, waiting for 1.3.1
+    pandas
 
 [tox]
 envlist =
-    {py36, py37, py38}
+    {py37,py38,py39}
     check-dist
     lint
     docs
     coverage
 
 [testenv]
 extras = all
@@ -27,17 +27,19 @@
     twine check {toxinidir}/dist/*
 whitelist_externals = rm
 
 [testenv:lint]
 deps =
      {[base]testdeps}
      pycodestyle
+     pydocstyle
      pylint
 commands =
     pycodestyle {[base]name} --exclude tests
+    pydocstyle {[base]name}
     pylint {[base]name} --ignore tests
 
 [testenv:coverage]
 deps =
     {[base]testdeps}
     coverage
 commands =
@@ -61,12 +63,24 @@
 # E731: do not assign a lambda expression, use a def
 # W503: line break after binary operator
 # W504: line break before binary operator
 [pycodestyle]
 ignore = E731,W503,W504
 max-line-length = 100
 
+[flake8]
+# ignore the following
+#   - E731: do not assign a lambda expression, use a def
+#   - W503: line break after binary operator
+#   - W504: line break before binary operator
+extend-ignore = E731,W503,W504
+max-line-length = 100
+exclude = tests,functional_tests,doc/source,.tox,.eggs
+
+[pydocstyle]
+convention = google
+
 [gh-actions]
 python =
-  3.6: py36
-  3.7: py37, check-dist, lint, docs, coverage
-  3.8: py38
+  3.7: py37, check-dist, lint
+  3.8: docs, coverage
+  3.9: py39
```

