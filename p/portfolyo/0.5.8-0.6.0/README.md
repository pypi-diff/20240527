# Comparing `tmp/portfolyo-0.5.8.tar.gz` & `tmp/portfolyo-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolyo-0.5.8.tar", max compression
+gzip compressed data, was "portfolyo-0.6.0.tar", max compression
```

## Comparing `portfolyo-0.5.8.tar` & `portfolyo-0.6.0.tar`

### file list

```diff
@@ -1,70 +1,77 @@
--rw-r--r--   0        0        0     2811 2023-12-12 18:33:00.570661 portfolyo-0.5.8/README.rst
--rw-r--r--   0        0        0      960 2023-12-12 18:33:00.582661 portfolyo-0.5.8/portfolyo/__init__.py
--rw-r--r--   0        0        0    23655 2023-12-12 18:33:00.582661 portfolyo-0.5.8/portfolyo/_version.py
--rw-r--r--   0        0        0       46 2023-12-12 18:33:00.582661 portfolyo-0.5.8/portfolyo/core/__init__.py
--rw-r--r--   0        0        0      635 2023-12-12 18:33:00.582661 portfolyo-0.5.8/portfolyo/core/commodity/commodity.py
--rw-r--r--   0        0        0      425 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/extendpandas.py
--rw-r--r--   0        0        0      152 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/mixins/__init__.py
--rw-r--r--   0        0        0      959 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/mixins/excelclipboard.py
--rw-r--r--   0        0        0    12478 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/mixins/plot.py
--rw-r--r--   0        0        0     8911 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/mixins/text.py
--rw-r--r--   0        0        0     1993 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/ndframelike.py
--rw-r--r--   0        0        0       71 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/__init__.py
--rw-r--r--   0        0        0    13977 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/arithmatic.py
--rw-r--r--   0        0        0     3292 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/children.py
--rw-r--r--   0        0        0    18958 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/classes.py
--rw-r--r--   0        0        0     3131 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/create.py
--rw-r--r--   0        0        0     2659 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/dataframeexport.py
--rw-r--r--   0        0        0     1512 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/decorators.py
--rw-r--r--   0        0        0     1054 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/developernotes.py
--rw-r--r--   0        0        0      861 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/enums.py
--rw-r--r--   0        0        0     1895 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/flat_helper.py
--rw-r--r--   0        0        0     1026 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/flat_methods.py
--rw-r--r--   0        0        0    16744 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/interop.py
--rw-r--r--   0        0        0     2586 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/nested_helper.py
--rw-r--r--   0        0        0     1380 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/nested_methods.py
--rw-r--r--   0        0        0     3379 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfline/prices.py
--rw-r--r--   0        0        0       29 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfstate/__init__.py
--rw-r--r--   0        0        0     7060 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfstate/arithmatic.py
--rw-r--r--   0        0        0    10243 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfstate/pfstate.py
--rw-r--r--   0        0        0     3238 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/pfstate/pfstate_helper.py
--rw-r--r--   0        0        0      478 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/core/suppresswarnings.py
--rw-r--r--   0        0        0      125 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/dev/__init__.py
--rw-r--r--   0        0        0    10528 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/dev/develop.py
--rw-r--r--   0        0        0     6857 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/dev/mockup.py
--rw-r--r--   0        0        0       22 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/prices/__init__.py
--rw-r--r--   0        0        0    16678 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/prices/convert.py
--rw-r--r--   0        0        0     5700 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/prices/hedge.py
--rw-r--r--   0        0        0     6607 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/prices/utils.py
--rw-r--r--   0        0        0      153 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/testing/__init__.py
--rw-r--r--   0        0        0     3234 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/testing/testing.py
--rw-r--r--   0        0        0     8655 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/todo.txt
--rw-r--r--   0        0        0      403 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/__init__.py
--rw-r--r--   0        0        0     2996 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/ceil.py
--rw-r--r--   0        0        0     9339 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/changefreq.py
--rw-r--r--   0        0        0    16947 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/changeyear.py
--rw-r--r--   0        0        0     1620 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/duration.py
--rw-r--r--   0        0        0     3030 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/floor.py
--rw-r--r--   0        0        0     4101 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/frame.py
--rw-r--r--   0        0        0     9010 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/freq.py
--rw-r--r--   0        0        0     2500 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/intersect.py
--rw-r--r--   0        0        0     4640 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/isboundary.py
--rw-r--r--   0        0        0     3105 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/leftandright.py
--rw-r--r--   0        0        0     4675 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/peakperiod.py
--rw-r--r--   0        0        0     1455 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/right.py
--rw-r--r--   0        0        0     1839 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/righttoleft.py
--rw-r--r--   0        0        0     5814 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/round.py
--rw-r--r--   0        0        0     1237 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/stamp.py
--rw-r--r--   0        0        0     9312 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/standardize.py
--rw-r--r--   0        0        0     2274 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/startofday.py
--rw-r--r--   0        0        0     2542 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/trim.py
--rw-r--r--   0        0        0    11619 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/tzone.py
--rw-r--r--   0        0        0     4422 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/unit.py
--rw-r--r--   0        0        0      864 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/unitdefinitions.txt
--rw-r--r--   0        0        0    16472 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/tools/wavg.py
--rw-r--r--   0        0        0      224 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/visualize/__init__.py
--rw-r--r--   0        0        0     3607 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/visualize/categories.py
--rw-r--r--   0        0        0     1670 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/visualize/colors.py
--rw-r--r--   0        0        0    13526 2023-12-12 18:33:00.586661 portfolyo-0.5.8/portfolyo/visualize/plot.py
--rw-r--r--   0        0        0     1241 2023-12-12 18:33:00.586661 portfolyo-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 portfolyo-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1634 2024-05-27 17:45:16.019529 portfolyo-0.6.0/LICENCE
+-rw-r--r--   0        0        0     3110 2024-05-27 17:45:16.019529 portfolyo-0.6.0/README.rst
+-rw-r--r--   0        0        0     1343 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/__init__.py
+-rw-r--r--   0        0        0    23655 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/_version.py
+-rw-r--r--   0        0        0       46 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/__init__.py
+-rw-r--r--   0        0        0      635 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/commodity/commodity.py
+-rw-r--r--   0        0        0      425 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/extendpandas.py
+-rw-r--r--   0        0        0       71 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/__init__.py
+-rw-r--r--   0        0        0    13929 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/arithmatic.py
+-rw-r--r--   0        0        0     3262 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/children.py
+-rw-r--r--   0        0        0    16259 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/classes.py
+-rw-r--r--   0        0        0     3131 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/create.py
+-rw-r--r--   0        0        0     2659 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/dataframeexport.py
+-rw-r--r--   0        0        0     1017 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/decorators.py
+-rw-r--r--   0        0        0     1054 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/developernotes.py
+-rw-r--r--   0        0        0      861 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/enums.py
+-rw-r--r--   0        0        0     1895 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/flat_helper.py
+-rw-r--r--   0        0        0     4039 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/flat_methods.py
+-rw-r--r--   0        0        0    16734 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/interop.py
+-rw-r--r--   0        0        0     2586 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/nested_helper.py
+-rw-r--r--   0        0        0     2068 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/nested_methods.py
+-rw-r--r--   0        0        0     5798 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/plot.py
+-rw-r--r--   0        0        0     4559 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfline/text.py
+-rw-r--r--   0        0        0       29 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfstate/__init__.py
+-rw-r--r--   0        0        0     7015 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfstate/arithmatic.py
+-rw-r--r--   0        0        0    12250 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfstate/pfstate.py
+-rw-r--r--   0        0        0     3240 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfstate/pfstate_helper.py
+-rw-r--r--   0        0        0     2767 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfstate/plot.py
+-rw-r--r--   0        0        0     1372 2024-05-27 17:45:16.031529 portfolyo-0.6.0/portfolyo/core/pfstate/text.py
+-rw-r--r--   0        0        0        1 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/core/shared/__init__.py
+-rw-r--r--   0        0        0      805 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/core/shared/excelclipboard.py
+-rw-r--r--   0        0        0     2228 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/core/shared/ndframelike.py
+-rw-r--r--   0        0        0     3361 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/core/shared/text.py
+-rw-r--r--   0        0        0      478 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/core/suppresswarnings.py
+-rw-r--r--   0        0        0      125 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/dev/__init__.py
+-rw-r--r--   0        0        0    10914 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/dev/develop.py
+-rw-r--r--   0        0        0     6877 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/dev/mockup.py
+-rw-r--r--   0        0        0     8655 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/todo.txt
+-rw-r--r--   0        0        0      442 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/__init__.py
+-rw-r--r--   0        0        0     2996 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/ceil.py
+-rw-r--r--   0        0        0     9471 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/changefreq.py
+-rw-r--r--   0        0        0    16935 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/changeyear.py
+-rw-r--r--   0        0        0     2035 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/duration.py
+-rw-r--r--   0        0        0     3030 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/floor.py
+-rw-r--r--   0        0        0     4106 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/frame.py
+-rw-r--r--   0        0        0     7905 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/freq.py
+-rw-r--r--   0        0        0     4489 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/hedge.py
+-rw-r--r--   0        0        0     8135 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/intersect.py
+-rw-r--r--   0        0        0     5137 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/isboundary.py
+-rw-r--r--   0        0        0     3105 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/leftandright.py
+-rw-r--r--   0        0        0    14140 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/peakconvert.py
+-rw-r--r--   0        0        0     7078 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/peakfn.py
+-rw-r--r--   0        0        0     2567 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/product.py
+-rw-r--r--   0        0        0     1455 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/right.py
+-rw-r--r--   0        0        0     1839 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/righttoleft.py
+-rw-r--r--   0        0        0     5814 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/round.py
+-rw-r--r--   0        0        0     1237 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/stamp.py
+-rw-r--r--   0        0        0     9555 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/standardize.py
+-rw-r--r--   0        0        0     3064 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/startofday.py
+-rw-r--r--   0        0        0     3329 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/testing.py
+-rw-r--r--   0        0        0     2651 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/trim.py
+-rw-r--r--   0        0        0      157 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/types.py
+-rw-r--r--   0        0        0    11448 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/tzone.py
+-rw-r--r--   0        0        0     4905 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/unit.py
+-rw-r--r--   0        0        0      864 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/unitdefinitions.txt
+-rw-r--r--   0        0        0      204 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/visualize/__init__.py
+-rw-r--r--   0        0        0     3607 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/visualize/categories.py
+-rw-r--r--   0        0        0     1861 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/visualize/colors.py
+-rw-r--r--   0        0        0    11879 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/visualize/plot.py
+-rw-r--r--   0        0        0    16980 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools/wavg.py
+-rw-r--r--   0        0        0     2917 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools2/changeyear.py
+-rw-r--r--   0        0        0     5341 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools2/concat.py
+-rw-r--r--   0        0        0     1567 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools2/intersect.py
+-rw-r--r--   0        0        0     4833 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools2/plot.py
+-rw-r--r--   0        0        0      251 2024-05-27 17:45:16.035529 portfolyo-0.6.0/portfolyo/tools2/types.py
+-rw-r--r--   0        0        0     1330 2024-05-27 17:45:16.039529 portfolyo-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3904 1970-01-01 00:00:00.000000 portfolyo-0.6.0/PKG-INFO
```

### Comparing `portfolyo-0.5.8/README.rst` & `portfolyo-0.6.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+=========
 portfolyo
 =========
 
 .. image:: https://img.shields.io/pypi/v/portfolyo
    :target: https://pypi.org/project/portfolyo
    :alt: Pypi
 
@@ -24,14 +25,16 @@
 .. image:: https://readthedocs.org/projects/portfolyo/badge/?version=latest
     :target: https://portfolyo.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 Portfolyo is a Python package to analyse and manipulate timeseries related to power 
 and gas offtake portfolios.
 
+
+------------
 Installation
 ------------
 
 .. code-block:: bash
 
    pip install portfolyo
 
@@ -41,43 +44,57 @@
 
    pip install portfolyo==x.y.z
 
    # or, in pyproject.toml
    portfolyo = "x.y.z"
 
 
+-------------
 Documentation
 -------------
 
 Documentation is hosted on readthedocs:
 
 https://portfolyo.readthedocs.io/
 
+
+----------
 Repository
 ----------
 
 The git repository is hosted on github:
 
 http://www.github.com/rwijtvliet/portfolyo
 
 
+----------
 Developing
 ----------
 
 This project uses ``black`` to format code and ``flake8`` for linting. We also support ``pre-commit`` to ensure
 these have been run. To configure your local environment please install these development dependencies and set up
 the commit hooks.
 
 .. code-block:: bash
 
    poetry install --with dev,test
    pre-commit install
 
 Feature branches are merged into the ``develop`` branch via pull request.
 
+
+Internal dependencies
+---------------------
+
+Inside the package, modules depend on each other in the following chain. A module may depend on another module if it is further to the left:
+
+tools >> pfline >> pfstate >> tools2
+
+
+----------
 Publishing
 ----------
 
 To publish a new release from ``develop``, create a new branch, increment the version number and push to github. For convenience, there is a ``create_release_branch.sh`` script that accomplishes the same, which takes one argument:
 
 .. code-block:: bash
```

### Comparing `portfolyo-0.5.8/portfolyo/__init__.py` & `portfolyo-0.6.0/portfolyo/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 """Package to analyse and manipulate timeseries related to power and gas offtake portfolios."""
 
-
 from . import _version, dev, tools
 from .core import extendpandas  # extend functionalty of pandas
 from .core import suppresswarnings
-from .core.mixins.plot import plot_pfstates
 from .core.pfline import Kind, PfLine, Structure, create
 from .core.pfstate import PfState
-from .prices.hedge import hedge
-from .prices.utils import is_peak_hour
+from .tools import testing
+from .tools2.changeyear import map_to_year
+from .tools2.concat import general as concat
+from .tools2.intersect import indexable as intersection
+from .tools2.plot import plot_pfstates
+from .tools.changefreq import averagable as asfreq_avg
+from .tools.changefreq import summable as asfreq_sum
 from .tools.changeyear import characterize_index, map_frame_to_year
 from .tools.freq import FREQUENCIES
+from .tools.hedge import hedge
+from .tools.peakfn import PeakFunction
+from .tools.peakfn import factory as create_peakfn
+from .tools.product import germanpower_peakfn, is_peak_hour
 from .tools.standardize import frame as standardize
 from .tools.tzone import force_agnostic, force_aware
-from .tools.unit import Q_, ureg, Unit
+from .tools.unit import Q_, Unit, ureg
 from .tools.wavg import general as wavg
 
 VOLUME = Kind.VOLUME
 PRICE = Kind.PRICE
 REVENUE = Kind.REVENUE
 COMPLETE = Kind.COMPLETE
```

### Comparing `portfolyo-0.5.8/portfolyo/_version.py` & `portfolyo-0.6.0/portfolyo/_version.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/core/commodity/commodity.py` & `portfolyo-0.6.0/portfolyo/core/commodity/commodity.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/core/ndframelike.py` & `portfolyo-0.6.0/portfolyo/core/shared/ndframelike.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 class NDFrameLike(abc.ABC):
     """Class that specifies which attributes from pandas Series and DataFrames must be
     implemented by descendents of this class (=PfLine and PfState)."""
 
     # Abstract methods to be implemented by descendents.
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def index(self) -> pd.DatetimeIndex:
         """Left timestamp of time period corresponding to each data row."""
         ...
 
     @abc.abstractmethod
     def asfreq(self, freq: str = "MS") -> NDFrameLike:
         """Resample the instance to a new frequency.
@@ -32,20 +33,28 @@
         Returns
         -------
         Instance
             Resampled at wanted frequency.
         """
         ...
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def loc(self):
         """Create a new instance with a subset of the rows (selection by row label(s) or
         a boolean array.)"""
         ...
 
+    @property
+    @abc.abstractmethod
+    def slice(self):
+        """Create a new instance with a subset of the rows.
+        Different from loc since performs slicing with right-open interval."""
+        ...
+
     @abc.abstractmethod
     def dataframe(
         self, cols: Iterable[str] = None, has_units: bool = True, *args, **kwargs
     ) -> pd.DataFrame:
         """DataFrame for portfolio line in default units.
 
         Parameters
```

### Comparing `portfolyo-0.5.8/portfolyo/core/pfline/arithmatic.py` & `portfolyo-0.6.0/portfolyo/core/pfline/arithmatic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Enable arithmatic with PfLine classes."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Union
+from typing import TYPE_CHECKING, Any
 
 import numpy as np
 import pandas as pd
 
-from ... import testing, tools
+from ... import tools
 from . import classes, create, interop
 from .enums import Kind, Structure
 
 if TYPE_CHECKING:  # needed to avoid circular imports
     from .classes import FlatPfLine, NestedPfLine, PfLine
 
 STRICT = False  # TODO: make setting
@@ -19,15 +19,15 @@
 
 class Prep:
     def assert_objects_indexcompatibility(fn):
         """Indices must have same frequency and same start-of-day; if not, raise Error."""
 
         def wrapper(o1, o2, *args, **kwargs):
             try:
-                testing.assert_indices_compatible(o1.index, o2.index)
+                tools.testing.assert_indices_compatible(o1.index, o2.index)
             except AssertionError as e:
                 raise NotImplementedError from e
             return fn(o1, o2, *args, **kwargs)
 
         return wrapper
 
     def assert_pflines_samekind(fn):
@@ -181,25 +181,25 @@
 
     def __rmul__(self: PfLine, other: Any) -> PfLine:
         return self * other  # defer to __mul__
 
     @Prep.standardize_other  # other converted to None, a PfLine, or dimless Series
     @Prep.raiseerror_if_otherNone  # other is now a PfLine or dimless Series...
     @Prep.assert_objects_indexcompatibility  # ... with a compatible index
-    def __truediv__(self: PfLine, other: Any) -> Union[PfLine, pd.Series]:
+    def __truediv__(self: PfLine, other: Any) -> PfLine | pd.Series:
         if isinstance(other, pd.Series):
             return Multiply.pfline_and_series(self, 1 / other)
         else:
             return Divide.two_pflines(self, other)
 
     @Prep.standardize_other  # other converted to None, a PfLine, or dimless Series
     @Prep.raiseerror_if_otherNone  # other is now a PfLine or dimless Series
     @Prep.raiseerror_if_otherdimlessseries  # other is now a PfLine...
     @Prep.assert_objects_indexcompatibility  # ... with a compatible index
-    def __rtruediv__(self: PfLine, other: Any) -> Union[PfLine, pd.Series]:
+    def __rtruediv__(self: PfLine, other: Any) -> PfLine | pd.Series:
         return Divide.two_pflines(other, self)  # NB order!
 
     @Prep.standardize_other  # other converted to None, a PfLine, or dimless Series
     @Prep.returnself_if_otherNone  # other is now a PfLine or dimless Series
     @Prep.raiseerror_if_otherdimlessseries  # other is now a PfLine...
     @Prep.assert_objects_indexcompatibility  # ... with a compatible index
     def __or__(self: PfLine, other: Any) -> PfLine:
@@ -281,20 +281,18 @@
     def nestedpfline_and_series(pfl: NestedPfLine, s: pd.Series) -> NestedPfLine:
         newchildren = {name: child * s for name, child in pfl.items()}
         return pfl.__class__(newchildren)
 
 
 class Divide:
     @Prep.ensure_pflines_flat  # pfl1 and pfl2 are now both flat
-    def two_pflines(pfl1: PfLine, pfl2: PfLine) -> Union[pd.Series, PfLine]:
+    def two_pflines(pfl1: PfLine, pfl2: PfLine) -> pd.Series | PfLine:
         return Divide.two_flatpflines(pfl1, pfl2)
 
-    def two_flatpflines(
-        pfl1: FlatPfLine, pfl2: FlatPfLine
-    ) -> Union[pd.Series, FlatPfLine]:
+    def two_flatpflines(pfl1: FlatPfLine, pfl2: FlatPfLine) -> pd.Series | FlatPfLine:
         if pfl1.kind is pfl2.kind:
             if pfl1.kind is Kind.COMPLETE:
                 raise NotImplementedError(
                     "Cannot divide complete PfLines. First select e.g. .volume or .price."
                 )
 
             if pfl1.kind is Kind.PRICE:
```

### Comparing `portfolyo-0.5.8/portfolyo/core/pfline/children.py` & `portfolyo-0.6.0/portfolyo/core/pfline/children.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 from __future__ import annotations
 
 import warnings
-from typing import TYPE_CHECKING, Any, Mapping, Union
+from typing import TYPE_CHECKING, Any, Mapping
 
-from ... import testing, tools
+from ... import tools
 from . import create
 
 if TYPE_CHECKING:
     from .classes import NestedPfLine, PfLine
 
 
 class ChildFunctionality(Mapping):
-    def set_child(
-        self: NestedPfLine, name: str, child: Union[PfLine, Any]
-    ) -> NestedPfLine:
+    def set_child(self: NestedPfLine, name: str, child: PfLine | Any) -> NestedPfLine:
         """Set/add/update child; returns new pfline instance without changing current instance."""
         if name in ["w", "q", "p", "r"]:
             raise ValueError("Name cannot be one of 'w', 'q', 'p', 'r'.")
         try:
             child = create.pfline(child)
         except (ValueError, TypeError) as e:
             raise ValueError(
                 f"Parameter ``child`` cannot be turned into a PfLine; got {child}."
             ) from e
         if child.kind is not self.kind:
             raise ValueError(
                 f"Incompatible kinds; the portfolio line has {self.kind} but the child has {child.kind}."
             )
         try:
-            testing.assert_indices_compatible(self.index, child.index)
+            tools.testing.assert_indices_compatible(self.index, child.index)
         except AssertionError as e:
             raise ValueError(
                 "Index of new child is not compatible with the existing data."
             ) from e
         idx = tools.intersect.indices(self.index, child.index)
         if len(idx) == 0:
             raise ValueError(
```

### Comparing `portfolyo-0.5.8/portfolyo/core/pfline/classes.py` & `portfolyo-0.6.0/portfolyo/core/pfline/classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 from __future__ import annotations
 
 import abc
 import dataclasses
-from typing import Any, Callable, Dict, Iterable, Mapping, Union  # noqa
+from typing import Callable, Dict  # noqa
 
 import numpy as np
 import pandas as pd
 
 from ... import tools
-from ..mixins import ExcelClipboardOutput, PfLinePlot, PfLineText
-from ..ndframelike import NDFrameLike
-from . import (
-    create,
-    dataframeexport,
-    decorators,
-    flat_methods,
-    nested_methods,
-    prices,
-    children,
-)
+from ..shared.excelclipboard import ExcelClipboardOutput
+from ..shared.ndframelike import NDFrameLike
+from . import children, create, dataframeexport, flat_methods, nested_methods
 from .arithmatic import PfLineArithmatic
 from .enums import Kind, Structure
+from .plot import PfLinePlot
+from .text import PfLineText
 
 
 def constructor(structure: Structure, kind: Kind) -> type:
     """Return reference to class constructor."""
     classmatrix = {
         (Structure.FLAT, Kind.VOLUME): FlatVolumePfLine,
         (Structure.FLAT, Kind.PRICE): FlatPricePfLine,
@@ -83,93 +77,86 @@
         return create.pfline(data)
 
     def __post_init__(self):
         err = f"Expected columns {self.kind.available}, received {self.df.columns}."
         assert set(self.df.columns) == set(self.kind.available), err
 
     @property
+    @abc.abstractmethod
+    def kind(self) -> Kind:
+        ...
+
+    @property
+    @abc.abstractmethod
+    def structure(self) -> Structure:
+        ...
+
+    @property
     def index(self) -> pd.DatetimeIndex:
         """Index of the data, containing the left-bound timestamps of the delivery periods."""
         return self.df.index
 
-    @abc.abstractproperty
-    def w(self) -> pd.Series:  # override if applicable
+    @property
+    @abc.abstractmethod
+    def w(self) -> pd.Series:
         """Return (flat) volume timeseries in [MW]."""
         ...
 
-    @abc.abstractproperty
-    def q(self) -> pd.Series:  # override if applicable
+    @property
+    @abc.abstractmethod
+    def q(self) -> pd.Series:
         """Return (flat) volume timeseries in [MWh]."""
         ...
 
-    @abc.abstractproperty
-    def p(self) -> pd.Series:  # override if applicable
+    @property
+    @abc.abstractmethod
+    def p(self) -> pd.Series:
         """Return (flat) price timeseries in [Eur/MWh]."""
         ...
 
-    @abc.abstractproperty
-    def r(self) -> pd.Series:  # override if applicable
+    @property
+    @abc.abstractmethod
+    def r(self) -> pd.Series:
         """Return (flat) revenue timeseries in [Eur]."""
         ...
 
-    @abc.abstractproperty
-    def volume(self) -> PfLine:  # override if applicable
+    @property
+    @abc.abstractmethod
+    def volume(self) -> PfLine:
         """Return volume-only PfLine."""
         ...
 
-    @abc.abstractproperty
-    def price(self) -> PfLine:  # override if applicable
+    @property
+    @abc.abstractmethod
+    def price(self) -> PfLine:
         """Return price-only PfLine."""
         ...
 
-    @abc.abstractproperty
-    def revenue(self) -> PfLine:  # override if applicable
+    @property
+    @abc.abstractmethod
+    def revenue(self) -> PfLine:
         """Return revenue-only PfLine"""
         ...
 
     @abc.abstractmethod
     def flatten(self) -> PfLine:
         """Return flattened instance, i.e., without children."""
         ...
 
     @abc.abstractmethod
-    def map_to_year(self, year: int, holiday_country: str = None) -> PfLine:
-        """Transfer the data to a hypothetical other year.
-
-        Parameters
-        ----------
-        year : int
-            Year to transfer the data to.
-        holiday_country : str, optional (default: None)
-            Country or region for which to assume the holidays. E.g. 'DE' (Germany), 'NL'
-            (Netherlands), or 'USA'. See ``holidays.list_supported_countries()`` for
-            allowed values.
-
-        Returns
-        -------
-        PfLine
-
-        Notes
-        -----
-        Useful for daily (and shorter) data. Copies over the data but takes weekdays (and
-        holidays) of target year into consideration. See ``portfolyo.map_frame_as_year()``
-        for more information.
-        Inaccurate for monthly data and longer, because we only have one value per month,
-        and can therefore not take different number of holidays/weekends (i.e., offpeak
-        hours) into consideration.
-        """
-        ...
-
-    @abc.abstractmethod
-    def po(self: PfLine, freq: str = "MS") -> pd.DataFrame:
-        """Decompose the portfolio line into peak and offpeak values. Takes simple averages
-        of volume [MW] and price [Eur/MWh] - does not hedge!
+    def po(
+        self: PfLine, peak_fn: tools.peakfn.PeakFunction, freq: str = "MS"
+    ) -> pd.DataFrame:
+        """Decompose the portfolio line into peak and offpeak values. Takes simple (duration-
+        weighted) averages of volume [MW] and price [Eur/MWh] - does not hedge!
 
         Parameters
         ----------
+        peak_fn : PeakFunction
+            Function that returns boolean Series indicating if timestamps in index lie in peak period.
         freq : {'MS' (months, default), 'QS' (quarters), 'AS' (years)}
             Frequency of resulting dataframe.
 
         Returns
         -------
         pd.DataFrame
             The dataframe shows a composition into peak and offpeak values.
@@ -181,41 +168,47 @@
         ...
 
     @abc.abstractmethod
     def hedge_with(
         self: PfLine,
         p: PricePfLine,
         how: str = "val",
+        peak_fn: tools.peakfn.PeakFunction = None,
         freq: str = "MS",
-        po: bool = None,
     ) -> PfLine:
         """Hedge the volume in the portfolio line with a price curve.
 
         Parameters
         ----------
         p : PricePfLine
             Portfolio line with prices to be used in the hedge.
         how : str, optional (Default: 'val')
             Hedge-constraint. 'vol' for volumetric hedge, 'val' for value hedge.
+        peak_fn : PeakFunction, optional (default: None)
+            To hedge with peak and offpeak products: function that returns boolean
+            Series indicating if timestamps in index lie in peak period.
+            If None, hedge with base products.
         freq : {'D' (days), 'MS' (months, default), 'QS' (quarters), 'AS' (years)}
             Frequency of hedging products. E.g. 'QS' to hedge with quarter products.
-        po : bool, optional
-            Type of hedging products. Set to True to split hedge into peak and offpeak.
-            (Default: split if volume timeseries has hourly values or shorter.)
+
+        See also
+        --------
+        portfolyo.create_peakfn
+        portfolyo.germanpower_peakfn
 
         Returns
         -------
         PfLine
             Hedged volume and prices. Index with same frequency as original, but every
             timestamp within a given hedging frequency has the same volume [MW] and price.
             (or, one volume-price pair for peak, and another volume-price pair for offpeak.)
 
         Notes
         -----
-        - If the PfLine contains prices, these are ignored.
+        If the PfLine contains prices, these are ignored.
         """
         ...
 
     @abc.abstractmethod
     def __bool__(self) -> bool:
         """Return True if object (i.e., its children) contains any non-zero data."""
         ...
@@ -263,47 +256,37 @@
     kind = Kind.COMPLETE
     w: pd.Series = property(lambda self: self.df["w"])
     q: pd.Series = property(lambda self: self.df["q"])
     p: pd.Series = property(lambda self: self.df["p"])
     r: pd.Series = property(lambda self: self.df["r"])
 
 
-class FlatPfLine(PfLine):
-    """Flat portfolio line, i.e., without children. Only has a single dataframe.
-
-    Notes
-    -----
-    * If the timeseries or values in ``data`` do not have a ``pint`` data type, the
-    standard units are assumed (MW, MWh, Eur, Eur/MWh).
-    * If the timeseries or values in ``data`` do have a ``pint`` data type, they are
-    converted into the standard units.
-    """
-
+class FlatPfLine:
     structure = Structure.FLAT
 
     dataframe = dataframeexport.Flat.dataframe
     flatten = flat_methods.flatten
-    po = prices.Flat.po
-    hedge_with = prices.Flat.hedge_with
-    # map_to_year => on child classes
+    po = flat_methods.po
+    hedge_with = flat_methods.hedge_with
     loc = flat_methods.loc
+    slice = flat_methods.slice
     __getitem__ = flat_methods.__getitem__
     # __bool__ => on child classes
     __eq__ = flat_methods.__eq__
 
 
-class NestedPfLine(PfLine, children.ChildFunctionality):
+class NestedPfLine(children.ChildFunctionality):
     structure = Structure.NESTED
 
     dataframe = dataframeexport.Nested.dataframe
     flatten = nested_methods.flatten
-    po = prices.Nested.po
-    hedge_with = prices.Nested.hedge_with
-    map_to_year = nested_methods.map_to_year
+    po = nested_methods.po
+    hedge_with = nested_methods.hedge_with
     loc = nested_methods.loc
+    slice = nested_methods.slice
     __bool__ = nested_methods.__bool__
     __eq__ = nested_methods.__eq__
 
 
 @dont_init_twice
 @dataclasses.dataclass(frozen=True, repr=False, eq=False)
 class FlatVolumePfLine(FlatPfLine, VolumePfLine, PfLine):
@@ -315,21 +298,14 @@
         if not len(newdf):
             raise ValueError(
                 f"There are no full periods available when changing to the frequency {freq}."
             )
         newdf["w"] = newdf["q"] / tools.duration.index(newdf.index)  # TODO: check unit
         return FlatVolumePfLine(newdf)
 
-    @decorators.map_to_year_warning
-    def map_to_year(self, year: int, holiday_country: str = None) -> FlatVolumePfLine:
-        df = self.df[["w"]]  # Averageble data to allow mapping unequal-length periods
-        newdf = tools.changeyear.map_frame_to_year(df, year, holiday_country)
-        newdf["q"] = newdf["w"] * tools.duration.index(newdf.index)
-        return FlatVolumePfLine(newdf)
-
     def __bool__(self) -> bool:
         return not np.allclose(self.df["w"].pint.magnitude, 0.0)
 
 
 @dont_init_twice
 @dataclasses.dataclass(frozen=True, repr=False, eq=False)
 class NestedVolumePfLine(NestedPfLine, VolumePfLine, PfLine):
@@ -356,20 +332,14 @@
         newdf = tools.changefreq.averagable(self.df[["p"]], freq)
         if not len(newdf):
             raise ValueError(
                 f"There are no full periods available when changing to the frequency {freq}."
             )
         return FlatPricePfLine(newdf)
 
-    @decorators.map_to_year_warning
-    def map_to_year(self, year: int, holiday_country: str = None) -> FlatVolumePfLine:
-        df = self.df[["p"]]  # Averageble data to allow mapping unequal-length periods
-        newdf = tools.changeyear.map_frame_to_year(df, year, holiday_country)
-        return FlatPricePfLine(newdf)
-
     def __bool__(self) -> bool:
         return not np.allclose(self.df["p"].pint.magnitude, 0.0)
 
 
 @dont_init_twice
 @dataclasses.dataclass(frozen=True, repr=False, eq=False)
 class NestedPricePfLine(NestedPfLine, PricePfLine, PfLine):
@@ -396,23 +366,14 @@
         newdf = tools.changefreq.summable(self.df[["r"]], freq)
         if not len(newdf):
             raise ValueError(
                 f"There are no full periods available when changing to the frequency {freq}."
             )
         return FlatRevenuePfLine(newdf)
 
-    @decorators.map_to_year_warning
-    def map_to_year(self, year: int, holiday_country: str = None) -> FlatVolumePfLine:
-        # Assume that revenue is scales proportionately with duration of period.
-        # E.g. 290 Eur in leapyear Feb --> 280 Eur in non-leapyear Feb.
-        df = self.df[["r"]] * tools.duration.index(self.df.index)  # Make averageble
-        newdf = tools.changeyear.map_frame_to_year(df, year, holiday_country)
-        newdf = newdf / tools.duration.index(newdf.index)  # Make summable again
-        return FlatRevenuePfLine(newdf)
-
     def __bool__(self) -> bool:
         return not np.allclose(self.df["r"].pint.magnitude, 0.0)
 
 
 @dont_init_twice
 @dataclasses.dataclass(frozen=True, repr=False, eq=False)
 class NestedRevenuePfLine(NestedPfLine, RevenuePfLine, PfLine):
@@ -453,22 +414,14 @@
             raise ValueError(
                 f"There are no full periods available when changing to the frequency {freq}."
             )
         newdf["w"] = newdf["q"] / tools.duration.index(newdf.index)
         newdf["p"] = newdf["r"] / newdf["q"]
         return FlatCompletePfLine(newdf)
 
-    @decorators.map_to_year_warning
-    def map_to_year(self, year: int, holiday_country: str = None) -> FlatVolumePfLine:
-        df = self.df[["w", "p"]]  # Averagable
-        newdf = tools.changeyear.map_frame_to_year(df, year, holiday_country)
-        newdf["q"] = newdf["w"] * tools.duration.index(newdf.index)
-        newdf["r"] = newdf["q"] * newdf["p"]
-        return FlatCompletePfLine(newdf)
-
     def __bool__(self) -> bool:
         return not (
             np.allclose(self.df["w"].pint.magnitude, 0.0)
             and np.allclose(self.df["r"].pint.magnitude, 0.0)
         )
```

### Comparing `portfolyo-0.5.8/portfolyo/core/pfline/create.py` & `portfolyo-0.6.0/portfolyo/core/pfline/create.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/core/pfline/dataframeexport.py` & `portfolyo-0.6.0/portfolyo/core/pfline/dataframeexport.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/core/pfline/developernotes.py` & `portfolyo-0.6.0/portfolyo/core/pfline/developernotes.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/core/pfline/enums.py` & `portfolyo-0.6.0/portfolyo/core/pfline/enums.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/core/pfline/flat_helper.py` & `portfolyo-0.6.0/portfolyo/core/pfline/flat_helper.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/core/pfline/interop.py` & `portfolyo-0.6.0/portfolyo/core/pfline/interop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Ensure interoperability by extracting power, energy, price, revenue, and
 dimensionless values/timeseries from data."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Mapping, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Mapping
 
 import numpy as np
 import pandas as pd
 
-from ... import testing, tools
+from ... import tools
 from . import classes, create
 
 if TYPE_CHECKING:  # needed to avoid circular imports
     from .classes import FlatPfLine
 
 _ATTRIBUTES = ("w", "q", "p", "r", "nodim", "agn")
 
@@ -40,20 +40,20 @@
     . Check for consistency and fill the missing attributes as much as possible:
         inop = inop.make_consistent()
 
     . And finally, return as dataframe with columns 'w', 'q', 'p', 'r', 'nodim'
         inop = inop.to_df()
     """
 
-    w: Union[tools.unit.Q_, pd.Series] = None
-    q: Union[tools.unit.Q_, pd.Series] = None
-    p: Union[tools.unit.Q_, pd.Series] = None
-    r: Union[tools.unit.Q_, pd.Series] = None
-    nodim: Union[tools.unit.Q_, pd.Series] = None  # explicitly dimensionless
-    agn: Union[float, pd.Series] = None  # agnostic
+    w: tools.unit.Q_ | pd.Series = None
+    q: tools.unit.Q_ | pd.Series = None
+    p: tools.unit.Q_ | pd.Series = None
+    r: tools.unit.Q_ | pd.Series = None
+    nodim: tools.unit.Q_ | pd.Series = None  # explicitly dimensionless
+    agn: float | pd.Series = None  # agnostic
 
     def __post_init__(self):
         # Add correct units and check type.
         object.__setattr__(self, "w", _set_unit(self.w, "w"))
         object.__setattr__(self, "q", _set_unit(self.q, "q"))
         object.__setattr__(self, "p", _set_unit(self.p, "p"))
         object.__setattr__(self, "r", _set_unit(self.r, "r"))
@@ -112,15 +112,17 @@
         # If we land here, there is no self.agn, and all other attributes are timeseries (or None).
 
         w, q, p, r, nodim = self.w, self.q, self.p, self.r, self.nodim
 
         # Volumes.
         if w is not None and q is not None:
             try:
-                testing.assert_series_equal(w, q / q.index.duration, check_names=False)
+                tools.testing.assert_series_equal(
+                    w, q / q.index.duration, check_names=False
+                )
             except AssertionError as e:
                 raise ValueError("Values for w and q are not consistent.") from e
         elif w is not None and q is None:
             q = w * w.index.duration
         elif w is None and q is not None:
             w = q / q.index.duration
         elif w is None and q is None and p is not None and r is not None:
@@ -153,15 +155,15 @@
             # Check for consistency, but ignore edge cases:
             # - p unknown (nan or inf) and q==0 --> ignore
             # - q unknown (nan or inf) and p==0 --> ignore
             ign1 = np.isclose(q.pint.m, 0) & (p.isna() | np.isinf(p.pint.m))
             ign2 = np.isclose(p.pint.m, 0) & (q.isna() | np.isinf(q.pint.m))
             ignore = ign1 | ign2
             try:
-                testing.assert_series_equal(
+                tools.testing.assert_series_equal(
                     r[~ignore], p[~ignore] * q[~ignore], check_names=False
                 )
             except AssertionError as e:
                 raise ValueError("Values for r, p, and q are not consistent.") from e
 
         return InOp(w=w, q=q, p=p, r=r, nodim=nodim)
 
@@ -213,16 +215,16 @@
     __ror__ = __or__
 
     def __eq__(self, other) -> bool:
         return _equal(self, other)
 
 
 def _set_unit(
-    v: Union[float, int, tools.unit.Q_, pd.Series], attr: str
-) -> Union[float, tools.unit.Q, pd.Series]:
+    v: float | int | tools.unit.Q_ | pd.Series, attr: str
+) -> float | tools.unit.Q | pd.Series:
     """Set unit (if none set yet) or convert to unit."""
     if v is None:
         return None
 
     unit = tools.unit.from_name(attr) if attr else None
 
     if unit is None:  # should be unit-agnostic
@@ -299,15 +301,15 @@
     attr = tools.unit.to_name(unit)  # Error if dimension unknown
     if attr not in _ATTRIBUTES:
         raise NotImplementedError(f"Cannot handle data with this unit ({unit}).")
     return attr
 
 
 def _from_data(
-    data: Union[float, tools.unit.Q_, pd.Series, Dict, pd.DataFrame, Iterable, Mapping]
+    data: float | tools.unit.Q_ | pd.Series | Dict | pd.DataFrame | Iterable | Mapping,
 ) -> InOp:
     """Turn ``data`` into a InterOp object."""
 
     if data is None:
         return InOp()
 
     elif isinstance(data, int) or isinstance(data, float):
@@ -395,25 +397,25 @@
         return False
     for attr in _ATTRIBUTES:
         val1, val2 = getattr(inop1, attr), getattr(inop2, attr)
         if type(val1) is not type(val2):
             return False
         if isinstance(val1, pd.Series):
             try:
-                testing.assert_series_equal(val1, val2, check_names=False)
+                tools.testing.assert_series_equal(val1, val2, check_names=False)
             except AssertionError:
                 return False
         elif val1 != val2:
             return False
     return True
 
 
 def pfline_or_nodimseries(
     data: Any, ref_index: pd.DatetimeIndex, agn_default: str = None
-) -> Union[None, pd.Series, FlatPfLine]:
+) -> None | pd.Series | FlatPfLine:
     """Turn ``data`` into PfLine if dimension-aware. If not, turn into Series."""
 
     # Already a PfLine.
     if isinstance(data, classes.PfLine):
         return data
 
     # Can be turned into a PfLine.
```

### Comparing `portfolyo-0.5.8/portfolyo/core/pfline/nested_helper.py` & `portfolyo-0.6.0/portfolyo/core/pfline/nested_helper.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/core/pfline/prices.py` & `portfolyo-0.6.0/portfolyo/core/pfline/flat_methods.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,134 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 import pandas as pd
 
 from ... import tools
-from ...prices import convert, hedge
-from ...prices.utils import duration_bpo
+from ...tools.peakconvert import tseries2poframe
 from . import classes
-from .enums import Kind, Structure
+from .enums import Kind
 
 if TYPE_CHECKING:
-    from .classes import FlatPfLine, NestedPfLine, PfLine, PricePfLine
+    from .classes import FlatPfLine, PfLine, PricePfLine
 
 
-class Flat:
-    def po(self: FlatPfLine, freq: str = "MS") -> pd.DataFrame:
-        if self.index.freq not in ["15T", "H"]:
-            raise ValueError(
-                "Only PfLines with (quarter)hourly values can be turned into peak and offpeak values."
-            )
-        if freq not in ["MS", "QS", "AS"]:
-            raise ValueError(
-                f"Value of paramater ``freq`` must be one of {'MS', 'QS', 'AS'} (got: {freq})."
-            )
+def flatten(self: FlatPfLine) -> FlatPfLine:
+    return self
 
-        prods = ("peak", "offpeak")
 
-        # Get values.
-        dfs = []
-        for col in ("w", "p"):
-            if col in self.kind.available:
-                vals = convert.tseries2bpoframe(self.df[col], freq)
-                vals.columns = pd.MultiIndex.from_product([vals.columns, [col]])
-                dfs.append(vals)
-        df = pd.concat(dfs, axis=1)
-
-        # Add duration.
-        durs = duration_bpo(df.index)
-        durs.columns = pd.MultiIndex.from_product([durs.columns, ["duration"]])
-        df = pd.concat([df, durs], axis=1)
-
-        # Add additional values and sort.
-        for prod in prods:
-            if "q" in self.kind.available:
-                df[(prod, "q")] = df[(prod, "w")] * df[(prod, "duration")]
-            if "r" in self.kind.available:
-                df[(prod, "r")] = (
-                    df[(prod, "q")] * df[(prod, "p")]
-                ).pint.to_base_units()
-        colidx = pd.MultiIndex.from_product([prods, ("duration", *self.kind.available)])
-        return df[colidx]
-
-    def hedge_with(
-        self: FlatPfLine,
-        p: PricePfLine,
-        how: str = "val",
-        freq: str = "MS",
-        po: bool = None,
-    ) -> FlatPfLine:
-        if self.kind is Kind.PRICE:
-            raise ValueError(
-                "Cannot hedge a PfLine that does not contain volume information."
-            )
-        if self.index.freq not in ["15T", "H", "D"]:
-            raise ValueError(
-                "Can only hedge a PfLine with daily or (quarter)hourly information."
-            )
-        if po is None:
-            po = self.index.freq in ["15T", "H"]  # default: peak/offpeak if possible
-        if po and self.index.freq not in ["15T", "H"]:
+def po(
+    self: PfLine, peak_fn: tools.peakfn.PeakFunction, freq: str = "MS"
+) -> pd.DataFrame:
+    df_dict = {}
+
+    # Always include duration.
+    duration = tools.duration.index(self.df.index)
+    df_dict["duration"] = tseries2poframe(duration, peak_fn, freq, True)
+
+    # Add volume.
+    if self.kind in [Kind.VOLUME, Kind.COMPLETE]:
+        df_dict["q"] = tseries2poframe(self.q, peak_fn, freq, True)
+        df_dict["w"] = df_dict["q"] / df_dict["duration"]
+
+    # Add revenue.
+    if self.kind in [Kind.REVENUE, Kind.COMPLETE]:
+        df_dict["r"] = tseries2poframe(self.r, peak_fn, freq, True)
+
+    # Add price.
+    if self.kind is Kind.PRICE:
+        df_dict["p"] = tseries2poframe(self.p, peak_fn, freq, False)
+    elif self.kind is Kind.COMPLETE:
+        df_dict["p"] = df_dict["r"] / df_dict["q"]
+
+    # Turn into dataframe.
+    return pd.DataFrame({k: df.stack() for k, df in df_dict.items()})
+
+
+def hedge_with(
+    self: PfLine,
+    prices: PricePfLine,
+    how: str = "val",
+    peak_fn: tools.peakfn.PeakFunction = None,
+    freq: str = "MS",
+) -> FlatPfLine:
+    if self.kind not in [Kind.VOLUME, Kind.COMPLETE]:
+        raise ValueError(
+            "Cannot hedge a PfLine that does not contain volume information."
+        )
+    if self.index.freq not in ["15T", "H", "D"]:
+        raise ValueError(
+            "Can only hedge a PfLine with daily or (quarter)hourly information."
+        )
+
+    wout, pout = tools.hedge.hedge(self.w, prices.p, how, peak_fn, freq)
+    df = pd.DataFrame({"w": wout, "p": pout})
+    df["q"] = df["w"] * tools.duration.index(df.index)
+    df["r"] = df["p"] * df["q"]
+    return classes.FlatCompletePfLine(df)
+
+
+def __eq__(self: FlatPfLine, other: Any) -> bool:
+    if not isinstance(other, self.__class__):
+        return False
+    try:
+        tools.testing.assert_frame_equal(self.df, other.df, rtol=1e-7)
+        return True
+    except AssertionError:
+        return False
+
+
+def __getitem__(self: FlatPfLine, *args, **kwargs):
+    raise TypeError("Flat portfolio line is not subscriptable (has no children).")
+
+
+@property
+def loc(self: FlatPfLine) -> LocIndexer:
+    return LocIndexer(self)
+
+
+@property
+def slice(self: FlatPfLine) -> SliceIndexer:
+    return SliceIndexer(self)
+
+
+class LocIndexer:
+    """Helper class to obtain FlatPfLine instance, whose index is subset of original index."""
+
+    def __init__(self, pfl: FlatPfLine):
+        self.pfl = pfl
+
+    def __getitem__(self, arg) -> FlatPfLine:
+        newdf = self.pfl.df.loc[arg]
+        try:
+            tools.standardize.assert_frame_standardized(newdf)
+        except AssertionError as e:
             raise ValueError(
-                "Can only hedge with peak and offpeak products if PfLine has (quarter)hourly information."
-            )
+                "Timeseries not in expected form. See ``portfolyo.standardize()`` for more information."
+            ) from e
 
-        wout, pout = hedge.hedge(self.w, p.p, how, freq, po)
-        df = pd.DataFrame({"w": wout, "p": pout})
-        df["q"] = df["w"] * tools.duration.index(df.index)
-        df["r"] = df["p"] * df["q"]
-        constructor = classes.constructor(Structure.FLAT, Kind.COMPLETE)
-        return constructor(df)
-        # TODO: move to tools or elsewhere, and reference from there.
-
-
-class Nested:
-    def po(self: NestedPfLine, freq: str = "MS") -> pd.DataFrame:
-        return self.flatten().po(freq)
-
-    def hedge_with(
-        self: NestedPfLine,
-        p: PfLine,
-        how: str = "val",
-        freq: str = "MS",
-        po: bool = None,
-    ) -> FlatPfLine:
-        return self.flatten().hedge_with(p, how, freq, po)
+        return self.pfl.__class__(newdf)  # use same (leaf) class
+
+
+class SliceIndexer:
+    """Helper class to obtain FlatPfLine instance, whose index is subset of original index.
+    Exclude end point from the slice."""
+
+    def __init__(self, pfl: FlatPfLine):
+        self.pfl = pfl
+
+    def __getitem__(self, arg) -> FlatPfLine:
+        mask = pd.Index([True] * len(self.pfl.df))
+        if arg.start is not None:
+            mask &= self.pfl.index >= arg.start
+        if arg.stop is not None:
+            mask &= self.pfl.index < arg.stop
+
+        newdf = self.pfl.df.loc[mask]
+        try:
+            tools.standardize.assert_frame_standardized(newdf)
+        except AssertionError as e:
+            raise ValueError(
+                "Timeseries not in expected form. See ``portfolyo.standardize()`` for more information."
+            ) from e
+        return self.pfl.__class__(newdf)  # use same (leaf) class
```

### Comparing `portfolyo-0.5.8/portfolyo/core/pfstate/arithmatic.py` & `portfolyo-0.6.0/portfolyo/core/pfstate/arithmatic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """Add arithmatic to PfState classes."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Union
+from typing import TYPE_CHECKING, Any
 
 import pandas as pd
 
 from ... import tools
 from ..pfline import PfLine, create
 from . import pfstate
 
 if TYPE_CHECKING:  # needed to avoid circular imports
     from . import PfState
 
-from ... import testing
-
 
 class Prep:
     def assert_objects_indexcompatibility(fn):
         """Indices must have same frequency and same start-of-day; if not, raise Error."""
 
         def wrapper(o1, o2, *args, **kwargs):
             try:
-                testing.assert_indices_compatible(o1.index, o2.index)
+                tools.testing.assert_indices_compatible(o1.index, o2.index)
             except AssertionError as e:
                 raise NotImplementedError from e
             return fn(o1, o2, *args, **kwargs)
 
         return wrapper
 
     def standardize_other(fn):
@@ -34,17 +32,15 @@
 
         def wrapper(pfs: PfState, other: Any):
             other = Prep._prep_data(other, pfs.index)
             return fn(pfs, other)
 
         return wrapper
 
-    def _prep_data(
-        value, refindex: pd.DatetimeIndex
-    ) -> Union[pd.Series, PfLine, PfState]:
+    def _prep_data(value, refindex: pd.DatetimeIndex) -> pd.Series | PfLine | PfState:
         """Turn ``value`` into PfLine or PfState if possible. If not, turn into (normal or unit-aware) Series."""
 
         # None.
         if value is None:
             return None
 
         # Already a PfState.
```

### Comparing `portfolyo-0.5.8/portfolyo/core/pfstate/pfstate.py` & `portfolyo-0.6.0/portfolyo/core/pfstate/pfstate.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 import dataclasses
 import warnings
 from typing import Iterable, Optional
 
 import pandas as pd
 
 from ... import tools
-from ..mixins import ExcelClipboardOutput, PfStatePlot, PfStateText
-from ..ndframelike import NDFrameLike
 from ..pfline import PfLine, create
+from ..shared.excelclipboard import ExcelClipboardOutput
+from ..shared.ndframelike import NDFrameLike
 from . import pfstate_helper
 from .arithmatic import PfStateArithmatic
+from .plot import PfStatePlot
+from .text import PfStateText
 
 
 @dataclasses.dataclass(frozen=True, repr=False)
 class PfState(
     NDFrameLike, PfStateText, PfStatePlot, ExcelClipboardOutput, PfStateArithmatic
 ):
     """Class to hold timeseries information of an energy portfolio, at a specific moment.
@@ -218,44 +220,74 @@
         # pu resampling is most important, so that prices are correctly weighted.
         offtakevolume = self.offtakevolume.asfreq(freq)
         unsourcedprice = self.unsourced.asfreq(freq).price  # ensures weighted avg
         sourced = self.sourced.asfreq(freq)
         return PfState(offtakevolume, unsourcedprice, sourced)
 
     def hedge_of_unsourced(
-        self: PfState, how: str = "val", freq: str = "MS", po: bool = None
+        self: PfState,
+        how: str = "val",
+        peak_fn: tools.peakfn.PeakFunction = None,
+        freq: str = "MS",
     ) -> PfLine:
         """Hedge the unsourced volume, at unsourced prices in the portfolio.
 
+        Parameters
+        ----------
+        how : str, optional (Default: 'val')
+            Hedge-constraint. 'vol' for volumetric hedge, 'val' for value hedge.
+        peak_fn : PeakFunction, optional (default: None)
+            To hedge with peak and offpeak products: function that returns boolean
+            Series indicating if timestamps in index lie in peak period.
+            If None, hedge with base products.
+        freq : {'D' (days), 'MS' (months, default), 'QS' (quarters), 'AS' (years)}
+            Frequency of hedging products. E.g. 'QS' to hedge with quarter products.
+
         See also
         --------
-        PfLine.hedge
+        PfLine.hedge_with
+        portfolyo.create_peakfn
+        portfolyo.germanpower_peakfn
 
         Returns
         -------
         PfLine
             Hedge (volumes and prices) of unsourced volume.
         """
-        return self.unsourced.volume.hedge_with(self.unsourcedprice, how, freq, po)
+        return self.unsourced.volume.hedge_with(self.unsourcedprice, how, peak_fn, freq)
 
     def source_unsourced(
-        self: PfState, how: str = "val", freq: str = "MS", po: bool = None
+        self: PfState,
+        how: str = "val",
+        peak_fn: tools.peakfn.PeakFunction = None,
+        freq: str = "MS",
     ) -> PfState:
         """Simulate PfState if unsourced volume is hedged and sourced at market prices.
 
+        Parameters
+        ----------
+        how : str, optional (Default: 'val')
+            Hedge-constraint. 'vol' for volumetric hedge, 'val' for value hedge.
+        peak_fn : PeakFunction, optional (default: None)
+            To hedge with peak and offpeak products: function that returns boolean
+            Series indicating if timestamps in index lie in peak period.
+            If None, hedge with base products.
+        freq : {'D' (days), 'MS' (months, default), 'QS' (quarters), 'AS' (years)}
+            Frequency of hedging products. E.g. 'QS' to hedge with quarter products.
+
         See also
         --------
         .hedge_of_unsourced()
 
         Returns
         -------
         PfState
-            which is fully hedged at time scales of `freq` or longer.
+            which is fully hedged at time scales of ``freq`` or longer.
         """
-        tosource = self.hedge_of_unsourced(how, freq, po)
+        tosource = self.hedge_of_unsourced(how, peak_fn, freq)
         return self.__class__(
             self.offtakevolume, self.unsourcedprice, self.sourced + tosource
         )
 
     def mtm_of_sourced(self) -> PfLine:
         """Mark-to-Market value of sourced volume."""
         return self.sourced.volume * (self.unsourcedprice - self.sourced.price)
@@ -276,19 +308,37 @@
     def __bool__(self):
         return True
 
     @property
     def loc(self) -> _LocIndexer:  # from ABC
         return _LocIndexer(self)
 
+    @property
+    def slice(self) -> _SliceIndexer:  # from ABC
+        return _SliceIndexer(self)
+
 
 class _LocIndexer:
     """Helper class to obtain PfState instance, whose index is subset of original index."""
 
     def __init__(self, pfs):
         self.pfs = pfs
 
     def __getitem__(self, arg) -> PfState:
         offtakevolume = self.pfs.offtake.volume.loc[arg]
         unsourcedprice = self.pfs.unsourcedprice.loc[arg]
         sourced = self.pfs.sourced.loc[arg]
         return PfState(offtakevolume, unsourcedprice, sourced)
+
+
+class _SliceIndexer:
+    """Helper class to obtain PfState instance, whose index is subset of original index.
+    Exclude end index from the slice"""
+
+    def __init__(self, pfs):
+        self.pfs = pfs
+
+    def __getitem__(self, arg) -> PfState:
+        offtakevolume = self.pfs.offtake.volume.slice[arg]
+        unsourcedprice = self.pfs.unsourcedprice.slice[arg]
+        sourced = self.pfs.sourced.slice[arg]
+        return PfState(offtakevolume, unsourcedprice, sourced)
```

### Comparing `portfolyo-0.5.8/portfolyo/core/pfstate/pfstate_helper.py` & `portfolyo-0.6.0/portfolyo/core/pfstate/pfstate_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Prepare/verify input data for PfState initialisation."""
 
-
 import warnings
 from typing import Any, Iterable
 
 import pandas as pd
 
-from ... import testing, tools
+from ... import tools
 from ..pfline import Kind, PfLine, create
 
 
 def make_pflines(
     offtakevolume: Any, unsourcedprice: Any, sourced: Any = None
 ) -> Iterable[PfLine]:
     """Take offtake, unsourced, sourced information. Do some data massaging and return
@@ -51,15 +50,15 @@
         raise ValueError("Parameter ``unsourcedprice`` does not contain prices.")
     elif unsourcedprice.kind is Kind.COMPLETE:
         warnings.warn(
             "Parameter ``unsourcedprice``: also contains volume infomation; this is discarded."
         )
         unsourcedprice = unsourcedprice.price
     try:
-        testing.assert_indices_compatible(ref_idx, unsourcedprice.index)
+        tools.testing.assert_indices_compatible(ref_idx, unsourcedprice.index)
     except AssertionError as e:
         raise ValueError from e
     if len(tools.intersect.indices(ref_idx, unsourcedprice.index)) < len(ref_idx):
         raise ValueError(
             "Parameter ``unsourcedprice`` does not cover entire delivery period of"
             " ``offtakevolume``."
         )
@@ -70,15 +69,15 @@
     if sourced is None:
         return create.flatpfline(pd.DataFrame({"q": 0, "r": 0}, ref_idx))
 
     sourced = create.pfline(sourced)
     if sourced.kind is not Kind.COMPLETE:
         raise ValueError("Parameter ``sourced`` does not contain price and volume.")
     try:
-        testing.assert_indices_compatible(ref_idx, sourced.index)
+        tools.testing.assert_indices_compatible(ref_idx, sourced.index)
     except AssertionError as e:
         raise ValueError from e
     # HACK: Workaround for error in pandas intersection (#46702):
     if len(tools.intersect.indices(ref_idx, sourced.index)) < len(ref_idx):
         raise ValueError(
             "Parameter ``sourced``: does not cover entire delivery period of"
             " ``offtakevolume``."
```

### Comparing `portfolyo-0.5.8/portfolyo/dev/develop.py` & `portfolyo-0.6.0/portfolyo/dev/develop.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Code to quickly get objects for testing.
 """
 
 import datetime as dt
-from typing import Dict, Union, Callable, Tuple
+from typing import Callable, Dict, Tuple
 
 import numpy as np
 import pandas as pd
 
 from .. import tools
 from ..core.pfline import FlatPfLine, Kind, NestedPfLine, PfLine, create
 from ..core.pfstate import PfState
@@ -24,43 +24,55 @@
     startdate: str = None,
     periods: int = None,
     start_of_day: dt.time = None,
     *,
     _seed: int = None,
 ) -> pd.DatetimeIndex:
     """Get index."""
+    # Prepare values.
     if _seed:
         np.random.seed(_seed)
     if not periods:
         standard_len = INDEX_LEN.get(freq, 10)
         periods = np.random.randint(standard_len // 2, standard_len * 2)
-        if tools.freq.up_or_down(freq, "H") <= 0 and tz is None:
-            # Shorten index to not include timestamp that do not exist in Europe/Berlin.
-            periods = min(periods, 4000)
     if not startdate:
-        a, m, d = 2020, 1, 1
-        a += np.random.randint(-4, 4) if _seed else (periods % 20 - 10)
+        a, m, d = 2016, 1, 1  # earliest possible
+        a += np.random.randint(0, 8) if _seed else (periods % 8)
         if tools.freq.up_or_down(freq, "MS") <= 0:
             m += np.random.randint(0, 12) if _seed else (periods % 12)
         if tools.freq.up_or_down(freq, "D") <= 0:
             d += np.random.randint(0, 28) if _seed else (periods % 28)
-        if tools.freq.up_or_down(freq, "H") <= 0 and tz is None:
-            # Start index after DST-start to not include timestamps that do not exist in Europe/Berlin.
-            m, d = 4, 2
         startdate = f"{a}-{m}-{d}"
     if not start_of_day:
         start_of_day = dt.time(hour=0, minute=0)
-    starttime = f"{start_of_day.hour:02}:{start_of_day.minute:02}:00"
-    start = f"{startdate} {starttime}"
-    return pd.date_range(start, freq=freq, periods=periods, tz=tz)
+    # Create index.
+    start = tools.stamp.create(startdate, tz, start_of_day)
+    i = pd.date_range(start, periods=periods, freq=freq)  # tz included in start
+    # Some checks.
+    if tools.freq.up_or_down(freq, "H") <= 0:
+        i = _shorten_index_if_necessary(i, start_of_day)
+    return i
+
+
+def _shorten_index_if_necessary(i, start_of_day) -> pd.DatetimeIndex:
+    """Shorten index with (quarter)hourly values if necessary to ensure that an integer
+    number of calendar days is included."""
+    if (i[-1] - i[0]).total_seconds() < 23 * 3600:
+        raise ValueError("Index must contain at least one full day")
+    # Must ensure that index is integer number of days.
+    for _ in range(0, 100):  # max 100 quarterhours in a day (@ end of DST)
+        if tools.right.stamp(i[-1], i.freq).time() == start_of_day:
+            return i
+        i = i[:-1]
+    raise ValueError("Can't find timestamp to end index on.")
 
 
 def get_value(
     name: str = None, has_unit: bool = True, magn: float = None, *, _seed: int = None
-) -> Union[float, tools.unit.Q_]:
+) -> float | tools.unit.Q_:
     """Get a single value."""
     if _seed:
         np.random.seed(_seed)
     if magn is None:
         magn = np.random.random() * 200
     if not has_unit:
         return magn
@@ -194,15 +206,15 @@
         Datetimeindex to use for the portfolio line.
     kind : Kind, optional (default: COMPLETE)
     nlevels : int (default: 1)
         Number of levels. Must be >=1 If 1, return flat portfolio line.
     childcount : int, optional (default: 2)
         Number of children on each level. (Ignored if `nlevels` == 1)
     positive : bool, optional (default: False)
-        If True, return only positive values. If False, make 1/3 of pflines negative.
+        If True, return only positive values. If False, make 1/2 of pflines negative.
     _ancestornames : Tuple[str], optional (default: ())
         Text to start the childrens' names with (concatenated with '-')
     _seed : int, optional (default: no seed value)
         Seed value for the randomizer.
 
     Returns
     -------
@@ -218,15 +230,15 @@
         columns = {
             Kind.VOLUME: "q",
             Kind.PRICE: "p",
             Kind.REVENUE: "r",
             Kind.COMPLETE: "qr",
         }[kind]
         df = get_dataframe(i, columns, _seed=_seed)
-        if not positive and np.random.rand() < 0.33:
+        if not positive and np.random.randint(1, 4) == 1:
             df = -1 * df  # HACK: `-df` leads to error in pint. Maybe fixed in future
         return create.flatpfline(df)
     # Create nested PfLine.
     if childcount < 1:
         raise ValueError("Nested PfLine must have at least 1 child.")
     namefn = _get_namefn(nlevels)
     children = {}
```

### Comparing `portfolyo-0.5.8/portfolyo/dev/mockup.py` & `portfolyo-0.6.0/portfolyo/dev/mockup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Create somewhat realistic curves."""
+
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
 
-from ..prices.utils import is_peak_hour
 from ..tools import unit  # noqa # ensure we use current ureg
+from ..tools.product import germanpower_peakfn
 
 
 def w_offtake(
     i: pd.DatetimeIndex,
     avg: float = 100.0,
     year_amp: float = 0.20,
     week_amp: float = 0.10,
@@ -102,15 +103,15 @@
     wa = i.map(lambda ts: ts.weekday() + 1) / 7 * np.pi * 2
     # peak fraction: -1 (middle of offpeak hours) .. 1 (middle of peak hours)
     if i.freq in ["H", "15T"]:
         b = np.array([0.5, 0.8, 1, 0.8, 0.5])
         if i.freq == "15T":  # repeat every value 4 times
             b = np.array([[bb, bb, bb, bb] for bb in b]).flatten()
         b = b[: len(i)]  # slice in case i is very short
-        pa = np.convolve(-1 + 2 * is_peak_hour(i), b / sum(b), mode="same")
+        pa = np.convolve(-1 + 2 * germanpower_peakfn(i), b / sum(b), mode="same")
     else:
         pa = np.zeros(len(i))
     # Values
     yv = year_amp * np.cos(ya - 0.35)  # max in feb
     wv = week_amp * np.cos(wa - 1.07)  # max on tuesday
     pv = peak_amp * pa
     s = pd.Series(avg * (1 + yv + wv + pv), i, name="p")
@@ -163,15 +164,15 @@
         pval = p_avg * (1 + rand_amp * np.random.uniform(-1, 1))
         return pd.DataFrame({"p": pval, "w": wval}, sub_s.index)
 
     def group_and_calc(s):
         return s.resample(freq, group_keys=False).apply(calc_wp)
 
     if sin.index.freq in ["15T", "H"]:
-        is_peak = is_peak_hour(sin.index)  # avoid running on each ts individually
+        is_peak = germanpower_peakfn(sin.index)  # avoid running on each ts individually
         df = sin.groupby(is_peak, group_keys=False).apply(group_and_calc)
     else:
         df = group_and_calc(sin)
     w, p = df.w, df.p
 
     # Add unit if wanted.
     if has_unit:
```

### Comparing `portfolyo-0.5.8/portfolyo/prices/convert.py` & `portfolyo-0.6.0/portfolyo/tools/peakconvert.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,151 +1,67 @@
-"""
-Convert volume [MW] and price [Eur/MWh] timeseries using base, peak, offpeak times.
+"""Module to convert between timeseries and base/peak/offpeak-values."""
 
-. Conversions without loss of information:
-.. Base and peak values <--> Peak and offpeak values
-.. Peak and offpeak values in dataframe with yearly/quarterly/monthly index <-->
-   peak and offpeak values in series with hourly (or shorter) index
-
-. Conversions with information loss:
-.. Hourly varying values --> Peak and offpeak values.
-"""
-
-import datetime as dt
 import warnings
-from typing import Iterable, Union
 
-import numpy as np
 import pandas as pd
 
-from .. import tools
-from . import utils
-
-Stamp = Union[dt.datetime, pd.Timestamp]
-Value = Union[float, int, tools.unit.Q_]
-
-BPO = ("base", "peak", "offpeak")
-
-
-def group_function(freq: str, po: bool = False):
-    """Function to group all rows that belong to same 'product'."""
+from . import changefreq as tools_changefreq
+from . import duration as tools_duration
+from . import freq as tools_freq
+from . import peakfn as tools_peakfn
+from . import trim as tools_trim
+from . import wavg as tools_wavg
+
+BPO = ["base", "peak", "offpeak"]
+
+
+def group_index(
+    i: pd.DatetimeIndex, peak_fn: tools_peakfn.PeakFunction, freq: str
+) -> pd.MultiIndex:
+    """Multiindex, that is the same for all rows that belong to same delivery period."""
+    # Grouping due to delivery period.
+    groups = [i.year]
     if freq == "MS":
-        if po:
-            return lambda ts: (ts.year, ts.month, utils.is_peak_hour(ts))
-        else:
-            return lambda ts: (ts.year, ts.month)
+        groups.append(i.month)
     elif freq == "QS":
-        if po:
-            return lambda ts: (ts.year, ts.quarter, utils.is_peak_hour(ts))
-        else:
-            return lambda ts: (ts.year, ts.quarter)
+        groups.append(i.quarter)
     elif freq == "AS":
-        if po:
-            return lambda ts: (ts.year, utils.is_peak_hour(ts))
-        else:
-            return lambda ts: (ts.year,)
-
-    raise ValueError(
-        f"Parameter ``freq`` must be one of 'MS', 'QS', 'AS'; got '{freq}'."
-    )
+        pass
+    else:
+        raise ValueError(
+            f"Parameter ``freq`` must be one of 'MS', 'QS', 'AS'; got '{freq}'."
+        )
 
+    # Add grouping due to peak.
+    if peak_fn is not None:
+        groups.append(peak_fn(i))
 
-def offpeak(
-    base: Union[Value, Iterable[Value]],
-    peak: Union[Value, Iterable[Value]],
-    ts_left: Union[Stamp, Iterable[Stamp]],
-    freq: str = None,
-) -> Union[Value, pd.Series]:
-    """Offpeak value, given base and peak value and time interval they apply to.
+    return pd.MultiIndex.from_arrays(groups)
 
-    Parameters
-    ----------
-    base : Union[Value, Iterable[Value]]
-        Base value
-    peak : Union[Value, Iterable[Value]]
-        Peak value
-    ts_left : Union[Stamp, Iterable[Stamp]]
-        (Left-bound) timestamp of period.
-    freq : {'MS' (month), 'QS' (quarter), 'AS' (year)}, optional
-        Length of delivery period. If none specified, use ``.freq`` attribute of
-        ``ts_left``.
 
-    Returns
-    -------
-    offpeak value(s)
-    """
-    fr = utils.duration_bpo(ts_left, freq)  # Series or DataFrame
-    b, p, o = fr["base"], fr["peak"], fr["offpeak"]
-    if isinstance(fr, pd.DataFrame):
-        b, p, o = b.values, p.values, o.values
-    return (base * b - peak * p) / o
-
-
-def peak(
-    base: Union[Value, Iterable[Value]],
-    offpeak: Union[Value, Iterable[Value]],
-    ts_left: Union[Stamp, Iterable[Stamp]],
-    freq: str = None,
-) -> Union[Value, pd.Series]:
-    """Peak value, given base and offpeak value and time interval they apply to.
-
-    See also
-    --------
-    .offpeak
-    """
-    fr = utils.duration_bpo(ts_left, freq)  # Series or DataFrame
-    b, p, o = fr["base"], fr["peak"], fr["offpeak"]
-    if isinstance(fr, pd.DataFrame):
-        b, p, o = b.values, p.values, o.values
-
-    return (base * b - offpeak * o) / p
-
-
-def base(
-    peak: Union[Value, Iterable[Value]],
-    offpeak: Union[Value, Iterable[Value]],
-    ts_left: Union[Stamp, Iterable[Stamp]],
-    freq: str = None,
-) -> Union[Value, pd.Series]:
-    """Base value, given peak and offpeak value and time interval they apply to.
-
-    See also
-    --------
-    .offpeak
-    """
-    fr = utils.duration_bpo(ts_left, freq)  # Series or DataFrame
-    b, p, o = fr["base"], fr["peak"], fr["offpeak"]
-    if isinstance(fr, pd.DataFrame):
-        b, p, o = b.values, p.values, o.values
-    return (peak * p + offpeak * o) / b
-
-
-def complete_bpoframe(partial_bpoframe: pd.DataFrame, prefix: str = "") -> pd.DataFrame:
-    """
-    Add missing information to bpoframe (Dataframe with base, peak, offpeak values).
+def complete_bpoframe(
+    df: pd.DataFrame, peak_fn: tools_peakfn.PeakFunction, is_summable: bool = False
+) -> pd.DataFrame:
+    """Complete a dataframe so it contains arbitrage-free base, peak, and offpeak values.
 
     Parameters
     ----------
-    partial_bpoframe : DataFrame
-        Dataframe with at least 2 columns with names in {'base', 'peak', 'offpeak'}.
-        Datetimeindex with frequency in {'MS', 'QS', 'AS'}.
-    prefix : str, optional (default: '')
-        If specified, add this to the column names to search for in the provided dataframe
-        (and to the column names in the returned dataframes).
+    df : DataFrame
+        With at least 2 of following columns: {'base', 'peak', 'offpeak'}. If all 3 are
+        present, no verification is done. Additional columns are dropped. DatetimeIndex
+        with freq in {'MS', 'QS', 'AS'}.
+    peak_fn : PeakFunction
+        Function that returns boolean Series indicating if timestamps in index lie in peak period.
+    is_summable : bool, optional (default: False)
+        True if data is summable, False if it is averagable.
 
     Returns
     -------
     DataFrame
-        If exactly one of {'base', 'peak', 'offpeak'} is missing, calculate value
-        of missing column from other two columns and return complete dataframe.
-
-    Notes
-    -----
-    Can only be used for values that are 'averagable' over a time period, like power [MW]
-    and price [Eur/MWh]. Not for e.g. energy [MWh], revenue [Eur], and duration [h].
+        Same as ``df``, with all 3 columns ('base', 'peak', 'offpeak').
 
     In:
 
                                 peak        offpeak
     ts_left
     2020-01-01 00:00:00+01:00   42.530036   30.614701
     2020-02-01 00:00:00+01:00   33.295167   15.931557
@@ -161,56 +77,56 @@
     2020-01-01 00:00:00+01:00   35.034906   42.530036   30.614701
     2020-02-01 00:00:00+01:00   21.919009   33.295167   15.931557
                                 ...         ...         ...
     2020-11-01 00:00:00+01:00   38.785706   49.110873   33.226004
     2020-12-01 00:00:00+01:00   43.519745   57.872246   35.055449
     12 rows × 3 columns
     """
-    col2bpo = {f"{prefix}{bpo}": bpo for bpo in BPO}
-    series = {col2bpo[c]: s for c, s in partial_bpoframe.iteritems() if c in col2bpo}
-
-    if len(series) > 2:  # i.e., 3
-        return partial_bpoframe
-    if len(series) < 2:
+    # Guard clauses.
+    found = [c for c in df if c in BPO]
+    if len(found) <= 1:  # too few present
         raise ValueError(
-            f"At least 2 of {', '.join(col2bpo.keys())} must be present as columns."
+            f"At least 2 of 'base', 'peak', 'offpeak' must be in columns; found {found}."
         )
-    df = partial_bpoframe.copy()
-    durations = utils.duration_bpo(df.index)
-    b, p, o = durations["base"], durations["peak"], durations["offpeak"]
-    if "offpeak" not in series:
-        df[f"{prefix}offpeak"] = (series["base"] * b - series["peak"] * p) / o
-    elif "peak" not in series:
-        df[f"{prefix}peak"] = (series["base"] * b - series["offpeak"] * o) / p
+    elif len(found) == 3:  # all present, nothing to do
+        return df[BPO]  # correct order
+
+    # Make copy of relevant columns, and fill.
+    df = df[found].copy()
+    if is_summable:
+        # Solve: peak + offpeak = base
+        if "peak" not in df:
+            df["peak"] = df["base"] - df["offpeak"]
+        elif "offpeak" not in df:
+            df["offpeak"] = df["base"] - df["peak"]
+        else:  # 'base' not in df
+            df["base"] = df["peak"] + df["offpeak"]
     else:
-        df[f"{prefix}base"] = (series["peak"] * p + series["offpeak"] * o) / b
+        # Solve: peak * duration_peak + offpeak * duration_offpeak = base * duration_base
+        # (with: duration_offpeak = duration_base - duration_peak)
+        b = tools_duration.index(df.index).pint.m  # as float
+        p = tools_peakfn.peak_duration(df.index, peak_fn).pint.m  # as float
+        if "peak" not in df:
+            # df["peak"] = (df["base"] * b - df["offpeak"] * (b - p)) / p
+            df["peak"] = (df["base"] - df["offpeak"]) * b / p + df["offpeak"]
+        elif "offpeak" not in df:
+            df["offpeak"] = (df["base"] * b - df["peak"] * p) / (b - p)
+        else:  # 'base' not in df
+            # df["base"] = (df["peak"] * p + df["offpeak"] * (b - p)) / b
+            df["base"] = (df["peak"] - df["offpeak"]) * p / b + df["offpeak"]
 
-    return df[col2bpo.keys()]  # correct order
+    return df[BPO]  # correct order
 
 
-def tseries2singlebpo(s: pd.Series, prefix: str = "") -> pd.Series:
+def _tseries2po(
+    s: pd.Series, peak_fn: tools_peakfn.PeakFunction, is_summable: bool
+) -> pd.Series:
     """
-    Aggregate timeseries with varying values to a single base, peak and offpeak value.
-
-    Parameters
-    ----------
-    s : Series
-        Timeseries with hourly or quarterhourly frequency.
-    prefix : str, optional (default: '')
-        If specified, add this to the index of the returned Series.
-
-    Returns
-    -------
-    Series
-        Index: base, peak, offpeak.
-
-    Notes
-    -----
-    Can only be used for values that are 'averagable' over a time period, like power [MW]
-    and price [Eur/MWh]. Not for e.g. energy [MWh], revenue [Eur], and duration [h].
+    Aggregate timeseries with varying (float) values to a single base, peak and offpeak
+    (float) value.
 
     In:
 
     ts_left
     2020-01-01 00:00:00+01:00    41.88
     2020-01-01 01:00:00+01:00    38.60
     2020-01-01 02:00:00+01:00    36.55
@@ -218,134 +134,131 @@
     2020-12-31 21:00:00+01:00    52.44
     2020-12-31 22:00:00+01:00    51.86
     2020-12-31 23:00:00+01:00    52.26
     Freq: H, Name: p, Length: 8784, dtype: float64
 
     Out:
 
-    base       31.401369
     peak       51.363667
     offpeak    20.311204
     dtype: float64
     """
-    # Handle possible units.
-    sin, units = (s.pint.magnitude, s.pint.units) if hasattr(s, "pint") else (s, None)
-
-    # Do calculations. Use normal mean, because all rows have same duration.
-    is_peak = utils.is_peak_hour(sin.index)
-    sout = pd.Series(
-        {
-            f"{prefix}base": sin.mean(),
-            f"{prefix}peak": sin[is_peak].mean(),
-            f"{prefix}offpeak": sin[~is_peak].mean(),
-        }
-    )
-
-    # Handle possible units.
-    if units is not None:
-        sout = sout.astype(f"pint[{units}]")
-    return sout
+    is_peak = peak_fn(s.index)
+    duration = tools_duration.index(s.index).pint.m  # floats
+    if is_summable:
+        return pd.Series(
+            {
+                "peak": s[is_peak].sum(),
+                "offpeak": s[~is_peak].sum(),
+            }
+        )
+    else:
+        return pd.Series(
+            {
+                "peak": tools_wavg.series(s[is_peak], duration[is_peak]),
+                "offpeak": tools_wavg.series(s[~is_peak], duration[~is_peak]),
+            }
+        )
 
 
-def tseries2bpoframe(s: pd.Series, freq: str = "MS", prefix: str = "") -> pd.DataFrame:
+def tseries2poframe(
+    s: pd.Series,
+    peak_fn: tools_peakfn.PeakFunction,
+    freq: str = "MS",
+    is_summable: bool = False,
+) -> pd.DataFrame:
     """
-    Aggregate timeseries with varying values to a dataframe with base, peak and offpeak
-    timeseries, grouped by provided time interval.
+    Aggregate timeseries with varying values to a dataframe with peak and offpeak
+    timeseries, grouped by specified frequency.
 
     Parameters
     ----------
     s : Series
         Timeseries with hourly or quarterhourly frequency.
-    freq : {'MS' (month, default) 'QS' (quarter), 'AS' (year)}
-        Target frequency.
-    prefix : str, optional (default: '')
-        If specified, add this to the column names of the returned dataframe.
+    peak_fn : PeakFunction
+        Function that returns boolean Series indicating if timestamps in index lie in peak period.
+    freq : str, optional (default: 'MS')
+        Target frequency; monthly-or-longer.
+    is_summable : bool, optional (default: False)
+        True if data is summable, False if it is averagable.
 
     Returns
     -------
     DataFrame
         Dataframe with base, peak and offpeak values (as columns). Index: downsampled
         timestamps at provided frequency.
 
-    Notes
-    -----
-    Can only be used for values that are 'averagable' over a time period, like power [MW]
-    and price [Eur/MWh]. Not for e.g. energy [MWh], revenue [Eur], and duration [h].
-
     In:
 
     ts_left
     2020-01-01 00:00:00+01:00    41.88
     2020-01-01 01:00:00+01:00    38.60
     2020-01-01 02:00:00+01:00    36.55
                                  ...
     2020-12-31 21:00:00+01:00    52.44
     2020-12-31 22:00:00+01:00    51.86
     2020-12-31 23:00:00+01:00    52.26
     Freq: H, Name: p, Length: 8784, dtype: float64
 
     Out:
 
-                                base        peak        offpeak
+                                peak        offpeak
     ts_left
-    2020-01-01 00:00:00+01:00   35.034906   42.530036   30.614701
-    2020-02-01 00:00:00+01:00   21.919009   33.295167   15.931557
-                                ...         ...         ...
-    2020-11-01 00:00:00+01:00   38.785706   49.110873   33.226004
-    2020-12-01 00:00:00+01:00   43.519745   57.872246   35.055449
+    2020-01-01 00:00:00+01:00   42.530036   30.614701
+    2020-02-01 00:00:00+01:00   33.295167   15.931557
+                                ...         ...
+    2020-11-01 00:00:00+01:00   49.110873   33.226004
+    2020-12-01 00:00:00+01:00   57.872246   35.055449
     12 rows × 3 columns
     """
-    if freq not in ("MS", "QS", "AS"):
-        raise ValueError(
-            f"Parameter ``freq`` must be one of 'MS', 'QS', 'AS'; got '{freq}'."
-        )
+    if tools_freq.up_or_down(freq, "MS") < 0:
+        raise ValueError(f"Parameter ``freq`` be monthly-or-longer; got '{freq}'.")
 
-    # Remove partial data
-    s = tools.trim.frame(s, freq)
+    # Remove partial data.
+    s = tools_trim.frame(s, freq)
 
     # Handle possible units.
     sin, units = (s.pint.magnitude, s.pint.units) if hasattr(s, "pint") else (s, None)
 
-    # Do calculations. Use normal mean, because all rows have same duration.
+    # Do calculations.
     sout = sin.resample(freq, group_keys=True).apply(
-        lambda s: tseries2singlebpo(s, prefix)
+        lambda s: _tseries2po(s, peak_fn, is_summable)
     )
 
     # Handle possible units.
     if units is not None:
         sout = sout.astype(f"pint[{units}]")
-    return sout.unstack()
+    return sout.unstack()  # peak, offpeak as columns
 
 
-def bpoframe2tseries(
-    bpoframe: pd.DataFrame, freq: str = "H", prefix: str = ""
+def poframe2tseries(
+    df: pd.DataFrame,
+    peak_fn: tools_peakfn.PeakFunction,
+    freq: str = "H",
+    is_summable: bool = False,
 ) -> pd.Series:
     """
-    Convert a dataframe with base, peak and/or offpeak values, to a single (quarter)hourly
-    timeseries.
+    Convert a dataframe with peak and offpeak values, to a single timeseries.
 
     Parameters
     ----------
-    bpoframe : DataFrame
-        Dataframe with values. Columns must include at least 2 of {'peak', 'offpeak',
-        'base'}. Datetimeindex with frequency in {'MS', 'QS', 'AS'}.
-    freq : {'H' (hour, default) '15T' (quarterhour)}
-        Target frequency.
-    prefix : str, optional (default: '')
-        If specified, add this to the column names to search for in the provided dataframe.
+    df : DataFrame
+        Dataframe with values. Columns must include at least {'peak', 'offpeak'}.
+        Datetimeindex with monthly-or-longer frequency.
+    peak_fn : PeakFunction
+        Function that returns boolean Series indicating if timestamps in index lie in peak period.
+    freq : str
+        Target frequency; short enough for ``peak_fn``.
+    is_summable : bool, optional (default: False)
+        True if data is summable, False if it is averagable.
 
     Returns
     -------
     Series
-        Timeseries with values as provided in `bpoframe`.
-
-    Notes
-    -----
-    Can only be used for values that are 'averagable' over a time period, like power [MW]
-    and price [Eur/MWh]. Not for e.g. energy [MWh], revenue [Eur], and duration [h].
+        Timeseries with values as provided in ``df``.
 
     In:
 
                                 peak        offpeak
     ts_left
     2020-01-01 00:00:00+01:00   42.530036   30.614701
     2020-02-01 00:00:00+01:00   33.295167   15.931557
@@ -362,141 +275,152 @@
     2020-01-01 02:00:00+01:00    30.614701
                                  ...
     2020-12-31 21:00:00+01:00    35.055449
     2020-12-31 22:00:00+01:00    35.055449
     2020-12-31 23:00:00+01:00    35.055449
     Freq: H, Length: 8784, dtype: float64
     """
-    if freq not in ("H", "15T"):
-        raise ValueError(f"Parameter ``freq`` must be 'H' or '15T'; got '{freq}'.")
-
-    df = bpoframe.rename({f"{prefix}{bpo}": bpo for bpo in BPO}, axis=1)  # remove prefx
-    df = complete_bpoframe(df)  # make sure we have peak and offpeak columns
-    df = tools.changefreq.averagable(df[["peak", "offpeak"]], freq)
-    df["ispeak"] = utils.is_peak_hour(df.index)
-
-    return df["offpeak"].where(df["ispeak"], df["peak"])
-
-
-def tseries2tseries(s: pd.Series, freq: str = "MS") -> pd.Series:
-    """
-    Transform timeseries (with possibly variable values) to one with (at certain
-    frequency) uniform peak and offpeak values.
-
-    Parameters
-    ----------
-    s : Series
-        Timeseries with hourly or quarterhourly frequency.
-    freq : {'MS' (month, default) 'QS' (quarter), 'AS' (year)}
-        Target frequency within which peak and offpeak values will be uniform.
-
-    Returns
-    -------
-    Series
-        Timeseries where each peak hour within the target frequency has the same
-        value. Idem for offpeak hours. Index: as original series.
-
-    Notes
-    -----
-    Can only be used for values that are 'averagable' over a time period, like power [MW]
-    and price [Eur/MWh]. Not for e.g. energy [MWh], revenue [Eur], and duration [h].
-
-    In:
-
-    ts_left
-    2020-01-01 00:00:00+01:00    41.88
-    2020-01-01 01:00:00+01:00    38.60
-    2020-01-01 02:00:00+01:00    36.55
-                                 ...
-    2020-12-31 21:00:00+01:00    52.44
-    2020-12-31 22:00:00+01:00    51.86
-    2020-12-31 23:00:00+01:00    52.26
-    Freq: H, Name: p, Length: 8784, dtype: float64
-
-    Out:
-
-    ts_left
-    2020-01-01 00:00:00+01:00    30.614701
-    2020-01-01 01:00:00+01:00    30.614701
-    2020-01-01 02:00:00+01:00    30.614701
-                                ...
-    2020-12-31 21:00:00+01:00    35.055449
-    2020-12-31 22:00:00+01:00    35.055449
-    2020-12-31 23:00:00+01:00    35.055449
-    Freq: H, Name: p, Length: 8784, dtype: float64
-    """
-    if s.index.freq not in ("H", "15T"):
-        raise ValueError(
-            f"Frequency of provided timeseries must be hourly or quarterhourly; got '{s.index.freq}'."
-        )
-
-    # Handle possible units.
-    sin, units = (s.pint.magnitude, s.pint.units) if hasattr(s, "pint") else (s, None)
-
-    # Return normal mean, because all rows have same duration.
-    sout = sin.groupby(group_function(freq, True)).transform(np.mean)
+    # Prep.
+    if "peak" not in df or "offpeak" not in df:  # ensure peak and offpeak available
+        df = complete_bpoframe(df, peak_fn)
+    df = df[["peak", "offpeak"]]
+
+    # Stretch the dataframe to higher frequency
+    if is_summable:
+        df2 = tools_changefreq.summable(df, freq)
+    else:
+        df2 = tools_changefreq.averagable(df, freq)
+    df2["ispeak"] = peak_fn(df2.index)  # will raise error if frequency not short enough
 
-    # Handle possible units.
-    if units is not None:
-        sout = sout.astype(f"pint[{units}]")
-    return sout
+    return df2["offpeak"].where(df2["ispeak"], df2["peak"])
 
 
-def bpoframe2bpoframe(
-    bpoframe: pd.DataFrame, freq: str = "AS", prefix: str = ""
+# def tseries2tseries(
+#     s: pd.Series,
+#     peak_fn: tools_peakfn.PeakFunction,
+#     freq: str = "MS",
+#     is_summable: bool = False,
+# ) -> pd.Series:
+#     """
+#     Transform timeseries (with possibly variable values) to one with (at certain
+#     frequency) uniform peak and offpeak values.
+#
+#     Parameters
+#     ----------
+#     s : Series
+#         Timeseries with hourly or quarterhourly frequency.
+#     peak_fn : PeakFunction, optional (default: None)
+#         Function that returns boolean Series indicating if timestamps in index lie in peak period.
+#     freq : {'MS' (month, default) 'QS' (quarter), 'AS' (year)}
+#         Target frequency within which peak and offpeak values will be uniform.
+#     is_summable : bool, optional (default: False)
+#         True if data is summable, False if it is averagable.
+#
+#     Returns
+#     -------
+#     Series
+#         Timeseries where each peak hour within the target frequency has the same
+#         value. Idem for offpeak hours. Index: as original series.
+#
+#     In:
+#
+#     ts_left
+#     2020-01-01 00:00:00+01:00    41.88
+#     2020-01-01 01:00:00+01:00    38.60
+#     2020-01-01 02:00:00+01:00    36.55
+#                                  ...
+#     2020-12-31 21:00:00+01:00    52.44
+#     2020-12-31 22:00:00+01:00    51.86
+#     2020-12-31 23:00:00+01:00    52.26
+#     Freq: H, Name: p, Length: 8784, dtype: float64
+#
+#     Out:
+#
+#     ts_left
+#     2020-01-01 00:00:00+01:00    30.614701
+#     2020-01-01 01:00:00+01:00    30.614701
+#     2020-01-01 02:00:00+01:00    30.614701
+#                                 ...
+#     2020-12-31 21:00:00+01:00    35.055449
+#     2020-12-31 22:00:00+01:00    35.055449
+#     2020-12-31 23:00:00+01:00    35.055449
+#     Freq: H, Name: p, Length: 8784, dtype: float64
+#     """
+#     # Remove partial data.
+#     s = tools_trim.frame(s, freq)
+#
+#     # Handle possible units.
+#     sin, units = (s.pint.magnitude, s.pint.units) if hasattr(s, "pint") else (s, None)
+#
+#     # Calculate.
+#     # grouping will raise error if frequency not short enough
+#     grouping = group_arrays(sin.index, freq, peak_fn)
+#     fn = tools_changefreq.summable if is_summable else tools_changefreq.averagable
+#     sout = sin.groupby(grouping).transform(
+#
+#     # Handle possible units.
+#     if units is not None:
+#         sout = sout.astype(f"pint[{units}]")
+#     return sout
+#
+
+
+def poframe2poframe(
+    df: pd.DataFrame,
+    peak_fn: tools_peakfn.PeakFunction,
+    freq: str = "AS",
+    is_summable: bool = False,
 ) -> pd.DataFrame:
     """
-    Convert a dataframe with base, peak and/or offpeak values to a similar dataframe
+    Convert a dataframe with peak and offpeak values to a similar dataframe
     with a different frequency.
 
     Parameters
     ----------
-    bpoframe : DataFrame
-        Columns must include at least 2 of {'peak', 'offpeak', 'base'}. Datetimeindex
-        with frequency in {'MS', 'QS', 'AS'}.
-    freq : {'MS' (month), 'QS' (quarter), 'AS' (year, default)}
-        Target frequency.
-    prefix : str, optional (default: '')
-        If specified, add this to the column names to search for in the provided dataframe
-        (and to the column names in the returned dataframes).
+    df : DataFrame
+        Columns must include at least {'peak', 'offpeak'}. Datetimeindex with monthly-
+        or-longer frequency.
+    peak_fn : PeakFunction
+        Function that returns boolean Series indicating if timestamps in index lie in peak period.
+    freq : str, optional (default: 'AS')
+        Target frequency; monthly-or-longer.
+    is_summable : bool, optional (default: False)
+        True if data is summable, False if it is averagable.
 
     Returns
     -------
     DataFrame
         Dataframe with base, peak and offpeak values (as columns). Index: timestamps at
-        provided frequency.
-
-    Notes
-    -----
-    Can only be used for values that are 'averagable' over a time period, like power [MW]
-    and price [Eur/MWh]. Not for e.g. energy [MWh], revenue [Eur], and duration [h].
+        specified frequency.
 
     In:
 
-                                base        peak        offpeak
+                                peak        offpeak
     ts_left
-    2020-01-01 00:00:00+01:00   35.034906   42.530036   30.614701
-    2020-02-01 00:00:00+01:00   21.919009   33.295167   15.931557
-                                ...         ...         ...
-    2020-11-01 00:00:00+01:00   38.785706   49.110873   33.226004
-    2020-12-01 00:00:00+01:00   43.519745   57.872246   35.055449
+    2020-01-01 00:00:00+01:00   42.530036   30.614701
+    2020-02-01 00:00:00+01:00   33.295167   15.931557
+                                ...         ...
+    2020-11-01 00:00:00+01:00   49.110873   33.226004
+    2020-12-01 00:00:00+01:00   57.872246   35.055449
     12 rows × 3 columns
 
     Out:
 
-                                base        peak        offpeak
+                                peak        offpeak
     ts_left
-    2020-01-01 00:00:00+01:00   30.490036   38.003536   26.312894
-    2020-04-01 00:00:00+02:00   25.900919   35.295167   20.681892
-    2020-07-01 00:00:00+02:00   32.706785   44.033511   26.371498
-    2020-10-01 00:00:00+02:00   39.455197   54.468722   31.063728
+    2020-01-01 00:00:00+01:00   38.003536   26.312894
+    2020-04-01 00:00:00+02:00   35.295167   20.681892
+    2020-07-01 00:00:00+02:00   44.033511   26.371498
+    2020-10-01 00:00:00+02:00   54.468722   31.063728
     """
-    if freq not in ("MS", "QS", "AS"):
-        raise ValueError(
-            f"Parameter ``freq`` must be one of 'MS', 'QS', 'AS'; got {freq}."
-        )
-    if tools.freq.up_or_down(bpoframe.index.freq, freq) == 1:
+    if tools_freq.up_or_down(freq, "MS") < 0:
+        raise ValueError(f"Parameter ``freq`` be monthly-or-longer; got '{freq}'.")
+
+    if tools_freq.up_or_down(df.index.freq, freq) == 1:
         warnings.warn(
             "This conversion includes upsampling, e.g. from yearly to monthly values."
+            " The result will be uniform at the frequency of the original frame ``df``."
         )
 
-    return tseries2bpoframe(bpoframe2tseries(bpoframe, "H", prefix), freq, prefix)
+    upsampled = poframe2tseries(df, peak_fn, "H", is_summable)
+    downsampled = tseries2poframe(upsampled, peak_fn, freq, is_summable)
+    return downsampled
```

### Comparing `portfolyo-0.5.8/portfolyo/prices/hedge.py` & `portfolyo-0.6.0/portfolyo/tools/hedge.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,105 +1,68 @@
 """Functionality to hedge an offtake profile with a price profile."""
 
 from typing import Tuple
 
 import pandas as pd
 
-from .. import tools
-from . import convert, utils
+from . import duration as tools_duration
+from . import intersect as tools_intersect
+from . import peakconvert as tools_peakconvert
+from . import peakfn as tools_peakfn
+from . import trim as tools_trim
+from . import wavg as tools_wavg
+
+
+def one_hedge(df: pd.DataFrame, how: str) -> pd.Series:
+    """Hedge over all timestamps in dataframe. Dataframe must have columns
+    'w', 'p', 'duration'. Returns Series with index 'w', 'p', with hedge values.
+    for the entire period."""
+    # Prepare weights.
+    if how == "val":  # value hedge
+        # solve for w_hedge: sum(w * duration * p) == w_hedge * sum(duration * p)
+        # so: w_hedge = sum(w * duration * p) / sum(duration * p)
+        weights = df["p"] * df["duration"]
+    else:  # how == "vol":  # volume hedge
+        # solve for w_hedge: sum(w * duration) == w_hedge * sum(duration)
+        # so: w_hedge = sum(w * duration) / sum(duration)
+        weights = df["duration"]
 
-
-def _hedge(df: pd.DataFrame, how: str, po: bool) -> pd.Series:
-    """
-    Hedge a power timeseries, for given price timeseries.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        with 'w' [MW] and 'p' [Eur/MWh] columns.
-    how : str. One of {'vol', 'val'}
-        Hedge-constraint. 'vol' for volumetric hedge, 'val' for value hedge.
-    po : bool
-        Set to True to split hedge into peak and offpeak values. (Only sensible
-        for timeseries with freq=='H' or shorter.)
-
-    Returns
-    -------
-    pd.Series
-        With float values or quantities.
-        If po==False, Series with index ['w', 'p'] (power and price in entire period).
-        If po==True, Series with multiindex ['peak', 'offpeak'] x ['w', 'p'] (power and
-        price, split between peak and offpeak intervals in the period.)
-
-    Notes
-    -----
-    If the index of `df` doesn't have a .duration attribute, all rows are assumed to be
-    of equal duration.
-    """
-
-    # Split into peak and offpeak.
-
-    if po:
-        apply_f = lambda df: _hedge(df, how, po=False)  # noqa
-        # s = df.groupby(utils.is_peak_hour).apply(apply_f) # calls group_f on EACH ts
-        is_peak_hour = utils.is_peak_hour(df.index)
-        s = df.groupby(is_peak_hour).apply(apply_f)  # calls group_f on index
-        return s.rename(index={True: "peak", False: "offpeak"}).stack()
-
-    # Don't split into peak and offpeak.
-
-    if df.index.freq:
-        # Use magnitude only, so that, if w and p are float series, their return
-        # series are also floats (instead of dimensionless Quantities).
-        df["dur"] = df.index.duration.pint.m
-    else:
-        df["dur"] = 1
-
-    # Get single power and price values.
-    p_hedge = (df.p * df.dur).sum() / df.dur.sum()
-    if how == "vol":  # volume hedge
-        # solve for w_hedge: sum (w * duration) == w_hedge * sum (duration)
-        w_hedge = (df.w * df.dur).sum() / df.dur.sum()
-    elif how == "val":  # value hedge
-        # solve for w_hedge: sum (w * duration * p) == w_hedge * sum (duration * p)
-        w_hedge = (df.w * df.dur * df.p).sum() / (df.dur * df.p).sum()
-    else:
-        raise ValueError(f"Parameter `how` must be 'val' or 'vol'; got {how}.")
+    p_hedge = tools_wavg.series(df["p"], df["duration"])
+    w_hedge = tools_wavg.series(df["w"], weights)
     return pd.Series({"w": w_hedge, "p": p_hedge})
 
 
 def hedge(
     w: pd.Series,
     p: pd.Series,
     how: str = "val",
+    peak_fn: tools_peakfn.PeakFunction = None,
     freq: str = "MS",
-    po: bool = None,
-) -> Tuple[pd.Series]:
+) -> Tuple[pd.Series, pd.Series]:
     """
     Make hedge of power timeseries, for given price timeseries.
 
     Parameters
     ----------
     w : Series
-        Power timeseries with hourly or quarterhourly frequency.
+        Power timeseries with spot market frequency.
     p: Series
         Price timeseries with same frequency.
     how : str, optional (Default: 'val')
         Hedge-constraint. 'vol' for volumetric hedge, 'val' for value hedge.
-    freq : {'D' (days), 'MS' (months, default), 'QS' (quarters), 'AS' (years)}
+    peak_fn : PeakFunction, optional (default: None)
+        Function that returns boolean Series indicating if timestamps in index lie in peak period.
+        If None, hedge with base products.
+    freq : {'D' (days), 'MS' (months), 'QS' (quarters), 'AS' (years)}, optional (default: 'MS')
         Frequency of hedging products. E.g. 'QS' to hedge with quarter products.
-    po : bool, optional
-        Type of hedging products. Set to True to split hedge into peak and offpeak.
-        (Default: split if volume timeseries has hourly values or shorter and hedging
-        products have monthly frequency or longer.)
 
     Returns
     -------
-    Tuple[pd.Series]
-        Power timeseries and price timeseries with hedge of `w` (with same index).
+    Tuple[Series, Series]
+        Power timeseries and price timeseries with hedge of ``w`` (with same index).
     """
     if w.index.freq is None or p.index.freq is None:
         raise ValueError(
             "Parameters ``w`` and ``p`` must have a DatetimeIndex with a set frequency attribute."
         )
     if w.index.freq != p.index.freq:
         raise ValueError(
@@ -107,40 +70,45 @@
         )
     if w.index.freq not in ["15T", "H", "D"]:
         raise ValueError("Can only hedge a timeseries with daily (or shorter) values.")
     if freq not in ["D", "MS", "QS", "AS"]:
         raise ValueError(
             f"Parameter ``freq`` must be one of 'D', 'MS', 'QS', 'AS'; got '{freq}'."
         )
-    if po is None:  # default: split in peak/offpeak if frequency is short enough
-        po = w.index.freq in ["15T", "H"] and freq != "D"
-    if po and not (w.index.freq in ["15T", "H"] and freq != "D"):
+    if peak_fn is not None and not (w.index.freq in ["15T", "H"] and freq != "D"):
         raise ValueError(
             "Split into peak and offpeak only possible when (a) hedging with monthly (or "
             "longer) products, and (b) if timeseries have hourly (or shorter) values."
         )
+    if how not in ["vol", "val"]:
+        raise ValueError(f"Parameter `how` must be 'val' or 'vol'; got {how}.")
 
     # Handle possible units.
     win, wunits = (w.pint.magnitude, w.pint.units) if hasattr(w, "pint") else (w, None)
     pin, punits = (p.pint.magnitude, p.pint.units) if hasattr(p, "pint") else (p, None)
 
     # Only keep full periods of overlapping timestamps.
-    i = win.index.intersection(pin.index)
-    df = tools.trim.frame(pd.DataFrame({"w": win, "p": pin}).loc[i, :], freq)
-    if len(df) == 0:
-        return df["w"], df["p"]  # No full periods; don't do hedge; return empty series
+
+    win, pin = tools_intersect.frames(win, pin)
+    dfin = tools_trim.frame(pd.DataFrame({"w": win, "p": pin}), freq)
+    if len(dfin) == 0:
+        return (
+            dfin["w"],
+            dfin["p"],
+        )  # No full periods; don't do hedge; return empty series
 
     # Do actual hedge.
-    group_f = convert.group_function(freq, po)
-    grouped_i = pd.MultiIndex.from_arrays(group_f(df.index))  # calls group_f on index
-    apply_f = lambda df: _hedge(df, how, False)  # noqa
-    # vals = df.groupby(group_f).apply(apply_f) # calls group_f on EACH ts
-    vals = df.groupby(grouped_i).apply(apply_f)
+    # . helper values
+    dfin["duration"] = tools_duration.index(dfin.index)
+    grouping = tools_peakconvert.group_index(dfin.index, peak_fn, freq)
+    # . calculation
+    vals = dfin.groupby(grouping).apply(lambda subdf: one_hedge(subdf, how))
     vals.index = pd.MultiIndex.from_tuples(vals.index)
-    for c in ["w", "p"]:
-        df[c] = df[c].groupby(grouped_i).transform(lambda gr: vals.loc[gr.name, c])
+    # . broadcast to original timeseries
+    dfout = vals.loc[grouping, :].set_axis(dfin.index)
+    wout, pout = dfout["w"], dfout["p"]
 
     # Handle possible units.
     if wunits or punits:
-        df = df.astype({"w": f"pint[{wunits:P}]", "p": f"pint[{punits:P}]"})
+        wout, pout = wout.astype(f"pint[{wunits}]"), pout.astype(f"pint[{punits}]")
 
-    return df["w"], df["p"]
+    return wout, pout
```

### Comparing `portfolyo-0.5.8/portfolyo/testing/testing.py` & `portfolyo-0.6.0/portfolyo/tools/testing.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import functools
 from typing import Any
 
 import numpy as np
 import pandas as pd
 import pint
-from .. import tools
-from ..tools.unit import Q_
+
+from . import unit as tools_unit
 
 
 def assert_value_equal(left: Any, right: Any):
     try:
         if np.isnan(left) and np.isnan(right):
             return
         assert np.isclose(left, right)
@@ -31,16 +31,16 @@
         assert coll == colr
         # Series must match.
         assert_series_equal(sl, sr, *args, **kwargs)
 
 
 @functools.wraps(pd.testing.assert_series_equal)
 def assert_series_equal(left: pd.Series, right: pd.Series, *args, **kwargs):
-    leftm, leftu = tools.unit.split_magn_unit(left)
-    rightm, rightu = tools.unit.split_magn_unit(right)
+    leftm, leftu = tools_unit.split_magn_unit(left)
+    rightm, rightu = tools_unit.split_magn_unit(right)
 
     # Magnitudes must be the same.
     leftm = leftm.replace([np.inf, -np.inf], np.nan)
     rightm = rightm.replace([np.inf, -np.inf], np.nan)
     pd.testing.assert_series_equal(leftm, rightm, *args, **kwargs)
 
     # Units must be the same.
@@ -61,29 +61,29 @@
     if (lf := left[0].time()) != (r := right[0].time()):
         raise AssertionError(f"Indices that have unequal start-of-day; {lf} and {r}.")
 
 
 def assert_w_q_compatible(freq: str, w: pd.Series, q: pd.Series):
     """Assert if timeseries with power- and energy-values are consistent."""
     if freq == "15T":
-        assert_series_equal(q, w * Q_(0.25, "h"), check_names=False)
+        assert_series_equal(q, w * tools_unit.Q_(0.25, "h"), check_names=False)
     elif freq == "H":
-        assert_series_equal(q, w * Q_(1.0, "h"), check_names=False)
+        assert_series_equal(q, w * tools_unit.Q_(1.0, "h"), check_names=False)
     elif freq == "D":
-        assert (q >= w * Q_(22.99, "h")).all()
-        assert (q <= w * Q_(25.01, "h")).all()
+        assert (q >= w * tools_unit.Q_(22.99, "h")).all()
+        assert (q <= w * tools_unit.Q_(25.01, "h")).all()
     elif freq == "MS":
-        assert (q >= w * 27 * Q_(24.0, "h")).all()
-        assert (q <= w * 32 * Q_(24.0, "h")).all()
+        assert (q >= w * 27 * tools_unit.Q_(24.0, "h")).all()
+        assert (q <= w * 32 * tools_unit.Q_(24.0, "h")).all()
     elif freq == "QS":
-        assert (q >= w * 89 * Q_(24.0, "h")).all()
-        assert (q <= w * 93 * Q_(24.0, "h")).all()
+        assert (q >= w * 89 * tools_unit.Q_(24.0, "h")).all()
+        assert (q <= w * 93 * tools_unit.Q_(24.0, "h")).all()
     elif freq == "AS":
-        assert (q >= w * Q_(8759.9, "h")).all()
-        assert (q <= w * Q_(8784.1, "h")).all()
+        assert (q >= w * tools_unit.Q_(8759.9, "h")).all()
+        assert (q <= w * tools_unit.Q_(8784.1, "h")).all()
     else:
         raise ValueError(f"Uncaught value for freq: {freq}.")
 
 
 def assert_p_q_r_compatible(r: pd.Series, p: pd.Series, q: pd.Series):
     """Assert if timeseries with revenue-, power-, and energy-values are consistent."""
     assert_series_equal(r, q * p, check_names=False)
```

### Comparing `portfolyo-0.5.8/portfolyo/todo.txt` & `portfolyo-0.6.0/portfolyo/todo.txt`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/tools/ceil.py` & `portfolyo-0.6.0/portfolyo/tools/ceil.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/tools/changefreq.py` & `portfolyo-0.6.0/portfolyo/tools/changefreq.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Functions to change frequency of a pandas dataframe."""
 
-from typing import Any, Union
+from typing import Any
 
 import pandas as pd
 
-
-from . import startofday as tools_startofday
+from . import duration as tools_duration
 from . import freq as tools_freq
 from . import right as tools_right
+from . import startofday as tools_startofday
 from . import trim as tools_trim
+from .types import Series_or_DataFrame
 
 
 def _astype(s: pd.Series, dtype: Any) -> pd.Series:
     """Convert dtype of series ``s`` to ``dtype``."""
     # HACK: s.astype(float) results in incorrect datatype (see https://github.com/hgrecco/pint-pandas/issues/203).
     # therefore: workaround taking the magnitude if wanted dtype is float (in this case, s.dtype should be 'pint[dimensionless]')
     if dtype == float and s.dtype == "pint[dimensionless]":
@@ -24,17 +25,19 @@
     i = pd.DatetimeIndex([], freq=freq, tz=s_ref.index.tz)
     return pd.Series([], i, dtype=s_ref.dtype, name=s_ref.name)
 
 
 def _downsample_avgable(s: pd.Series, freq: str) -> pd.Series:
     """Downsample averagble series."""
     # For averagable series: first make summable.
-    summable = s.mul(s.index.duration, axis=0)  # now has a pint dtype
+    duration = tools_duration.frame(s)
+    summable = s.mul(duration, axis=0)  # now has a pint dtype
     summable2 = _downsample_summable(summable, freq)
-    s2 = summable2.div(summable2.index.duration, axis=0)
+    duration2 = tools_duration.frame(summable2)
+    s2 = summable2.div(duration2, axis=0)
     s2 = _astype(s2, s.dtype)
     return s2.rename(s.name)
 
 
 def _downsample_summable(s: pd.Series, freq: str) -> pd.Series:
     """Downsample summable series."""
     # Downsampling is easiest for summable series: sum child values.
@@ -65,17 +68,19 @@
         s2.index.freq = freq  # ...(c) and set the frequency manually as well.
     return s2.rename(s.name)
 
 
 def _upsample_summable(s: pd.Series, freq: str) -> pd.Series:
     """Upsample summable series."""
     # For summable series: first make averagable.
-    avgable = s.div(s.index.duration, axis=0)  # now has a pint dtype
+    duration = tools_duration.frame(s)
+    avgable = s.div(duration, axis=0)  # now has a pint dtype
     avgable2 = _upsample_avgable(avgable, freq)
-    s2 = avgable2.mul(avgable2.index.duration, axis=0)
+    duration2 = tools_duration.frame(avgable2)
+    s2 = avgable2.mul(duration2, axis=0)
     s2 = _astype(s2, s.dtype)
     return s2.rename(s.name)
 
 
 def _upsample_avgable(s: pd.Series, freq: str) -> pd.Series:
     """Upsample averagable series."""
     # Upsampling is easiest for averagable series: duplicate value to all children.
@@ -186,30 +191,28 @@
         return _downsample_summable(pd.Series(0, i), freq).index
 
     # Must upsample.
     else:  # up_or_down == 1
         return _upsample_avgable(pd.Series(0, i), freq).index
 
 
-def summable(
-    fr: Union[pd.Series, pd.DataFrame], freq: str = "MS"
-) -> Union[pd.Series, pd.DataFrame]:
+def summable(fr: Series_or_DataFrame, freq: str = "MS") -> Series_or_DataFrame:
     f"""
     Resample and aggregate a DataFrame or Series with 'time-summable' quantities.
 
     Parameters
     ----------
-    fr : pd.Series or pd.DataFrame
+    fr : Series or DataFrame
         Pandas Series or DataFrame to be resampled.
     freq : {{{', '.join(tools_freq.FREQUENCIES)}}}, optional (default: 'MS')
         Target frequency.
 
     Returns
     -------
-    DataFrame or Series
+    Series or DataFrame
 
     Notes
     -----
     A 'time-summable' quantity is one that can be summed to get to an aggregate
     value, like revenue [Eur] or energy [MWh]. Prices [Eur/MWh] and powers [MW]
     are not time-summable.
     See https://portfolyo.readthedocs.io/en/latest/specialized_topics/resampling.html
@@ -224,30 +227,28 @@
     if isinstance(fr, pd.DataFrame):
         # Turn into series, change frequency, and turn back into dataframe.
         return pd.DataFrame({key: summable(s, freq) for key, s in fr.items()})
 
     return _general(True, fr, freq)
 
 
-def averagable(
-    fr: Union[pd.Series, pd.DataFrame], freq: str = "MS"
-) -> Union[pd.Series, pd.DataFrame]:
+def averagable(fr: Series_or_DataFrame, freq: str = "MS") -> Series_or_DataFrame:
     f"""
     Resample and aggregate a DataFrame or Series with 'time-averagable' quantities.
 
     Parameters
     ----------
-    fr : pd.Series or pd.DataFrame
+    fr : Series or DataFrame
         Pandas Series or DataFrame to be resampled.
     freq : {{{', '.join(tools_freq.FREQUENCIES)}}}, optional (default: 'MS')
         Target frequency.
 
     Returns
     -------
-    DataFrame or Series
+    Series or DataFrame
 
     Notes
     -----
     A 'time-averagable' quantity is one that can be averaged to an aggregate value,
     like power [MW]. When downsampling, the values are weighted with their duration.
     See https://portfolyo.readthedocs.io/en/latest/specialized_topics/resampling.html
     for more information.
```

### Comparing `portfolyo-0.5.8/portfolyo/tools/changeyear.py` & `portfolyo-0.6.0/portfolyo/tools/changeyear.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 same calender month (but different year)."""
 
 # Three difficulties when changing the year:
 # . Feb 29 might be present in one of the years but not in the other.
 # . Daylight-savings time will likely start and end at a different day.
 # . Weekdays and holidays are not at the same date.
 
-from typing import Callable, Union
+from typing import Callable
 
 import holidays
 import pandas as pd
 
 from . import changefreq as tools_changefreq
 from . import freq as tools_freq
 from . import right as tools_right
 from . import unit as tools_unit
+from .types import Series_or_DataFrame
 
 docstringliteral_notes = """
 * Function is meant for data that spans full months. Using partial months may lead
   to unexpected behavior.
 * No values are recalculated; they are simply 'reshuffled' to obey the rules below.
 * The mapping is always between the same calendar month (e.g., April to April).
 * The mapping is between fixed year-month pairs (e.g., all values for 2025-April are
@@ -360,18 +361,18 @@
 
 
 # ---
 
 
 @additional_notes
 def map_frame_to_index(
-    source: Union[pd.Series, pd.DataFrame],
+    source: Series_or_DataFrame,
     idx_target: pd.DatetimeIndex,
     holiday_country: str = None,
-) -> Union[pd.Series, pd.DataFrame]:
+) -> Series_or_DataFrame:
     """Transfer the data in a Series or DataFrame to a hypothetical other index
     according to certain rules (see Notes). What would the data have looked like if it
     had occured in a different year?
 
     Parameters
     ----------
     source: pd.Series or pd.DataFrame
@@ -402,18 +403,18 @@
     else:
         series = {col: s[mapping].values for col, s in source.items()}
         return pd.DataFrame(series, mapping.index)
 
 
 @additional_notes
 def map_frame_to_year(
-    source: Union[pd.Series, pd.DataFrame],
+    source: Series_or_DataFrame,
     target_year: int,
     holiday_country: str = None,
-) -> Union[pd.Series, pd.DataFrame]:
+) -> Series_or_DataFrame:
     """Transfer the data in a Series or DataFrame to a hypothetical other year
     according to certain rules (see Notes). What would the data have looked like if it
     had occured in a different year?
 
     Parameters
     ----------
     source: pd.Series or pd.DataFrame
```

### Comparing `portfolyo-0.5.8/portfolyo/tools/duration.py` & `portfolyo-0.6.0/portfolyo/tools/duration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-"""
-Duration of delivery periods.
-"""
-
+"""Duration of delivery periods."""
 
 import pandas as pd
 
 from . import freq as tools_freq
 from . import right as tools_right
 from . import unit as tools_unit
 
@@ -37,27 +34,43 @@
         h = 1.0 if freq == "H" else 0.25
     else:
         h = (tools_right.stamp(ts, freq) - ts).total_seconds() / 3600
     return tools_unit.Q_(h, "h")
 
 
 def index(i: pd.DatetimeIndex) -> pd.Series:
-    """Duration of a timestamp.
+    """Duration of the timestamps in an index.
 
     Parameters
     ----------
-    i : pd.DatetimeIndex
+    i : DatetimeIndex
         Index for which to calculate the duration.
 
     Returns
     -------
     pint-Series
         With ``i`` as its index, and the corresponding duration as the values.
     """
     if i.freq in ["15T", "H"]:
         # Speed-up things for fixed-duration frequencies.
         h = 1.0 if i.freq == "H" else 0.25
     else:
         # Individual calculations for non-fixed-duration frequencies.
         h = (tools_right.index(i) - i).map(lambda td: td.total_seconds() / 3600)
 
-    return pd.Series(h, i).astype("pint[h]").rename("duration")
+    return pd.Series(h, i, dtype="pint[h]").rename("duration")
+
+
+def frame(fr: pd.Series | pd.DataFrame) -> pd.Series:
+    """Duration of the timestamps in the index of a Series or DataFrame.
+
+    Parameters
+    ----------
+    fr : Series or DataFrame
+        Object with index for which to calculate the duration.
+
+    Returns
+    -------
+    pint-Series
+        With ``i`` as its index, and the corresponding duration as the values.
+    """
+    return index(fr.index)
```

### Comparing `portfolyo-0.5.8/portfolyo/tools/floor.py` & `portfolyo-0.6.0/portfolyo/tools/floor.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/tools/frame.py` & `portfolyo-0.6.0/portfolyo/tools/frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Tools for working with pandas series and dataframes.
 """
 
 import functools
-from typing import Any, Iterable, Union
+from typing import Any, Iterable
 
 import numpy as np
 import pandas as pd
 
+from .types import Series_or_DataFrame
 
-def fill_gaps(
-    fr: Union[pd.Series, pd.DataFrame], maxgap: int = 2
-) -> Union[pd.Series, pd.DataFrame]:
+
+def fill_gaps(fr: Series_or_DataFrame, maxgap: int = 2) -> Series_or_DataFrame:
     """Fill gaps in series by linear interpolation.
 
     Parameters
     ----------
     fr : pd.Series or pd.DataFrame
     maxgap : int, optional
         Maximum number of rows that are filled. Larger gaps are kept. Default: 2.
```

### Comparing `portfolyo-0.5.8/portfolyo/tools/freq.py` & `portfolyo-0.6.0/portfolyo/tools/freq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Tools for dealing with frequencies.
 """
 
-from typing import Union
-
 import numpy as np
 import pandas as pd
 
+from .types import Series_or_DataFrame
+
 # Allowed frequencies.
 # Perfect containment; a short-frequency time period always entirely falls within a single high-frequency time period.
 # AS -> 4 QS; QS -> 3 MS; MS -> 28-31 D; D -> 23-25 H; H -> 4 15T
 FREQUENCIES = ["AS", "QS", "MS", "D", "H", "15T"]
 
 
 def up_or_down(
@@ -49,60 +49,27 @@
     >>> freq.up_or_down('MS', 'MS')
     0
     """
     standard_common_ts = pd.Timestamp("2020-01-01 0:00")
     backup_common_ts = pd.Timestamp("2020-02-03 04:05:06")
     if common_ts is None:
         common_ts = standard_common_ts
+
     ts1 = common_ts + pd.tseries.frequencies.to_offset(freq_source)
     ts2 = common_ts + pd.tseries.frequencies.to_offset(freq_target)
     if ts1 > ts2:
         return 1
     elif ts1 < ts2:
         return -1
     if common_ts == standard_common_ts:
         # If they are the same, try with another timestamp.
         return up_or_down(freq_source, freq_target, backup_common_ts)
     return 0  # only if both give the same answer.
 
 
-def longer_or_shorter(freq: str, freq_ref: str, common_ts: pd.Timedelta = None) -> int:
-    """
-    Compare frequency with reference frequency to see if it is longer or shorter.
-
-    Parameters
-    ----------
-    freq, freq_ref : frequencies to compare.
-    common_ts : timestamp, optional
-        Timestamp to use as anchor from which to compare the two.
-
-    Returns
-    -------
-    * 1 if frequency ``freq`` is longer than the reference frequency ``freq_ref``.
-    * 0 if frequencies are the same.
-    * -1 if frequency ``freq`` is shorter than the reference frequency ``freq_ref``.
-
-    Notes
-    -----
-    Arbitrarily using a time point as anchor to calculate the length of the time period
-    from. May have influence on the ratio (duration of a month, quarter, year etc are
-    influenced by this), but, for most common frequencies, not on which is longer.
-
-    Examples
-    --------
-    >>> freq.longer_or_shorter('D', 'MS')
-    -1
-    >>> freq.longer_or_shorter('MS', 'D')
-    1
-    >>> freq.longer_or_shorter('MS', 'MS')
-    0
-    """
-    return up_or_down(freq, freq_ref, common_ts)
-
-
 def _longestshortest(shortest: bool, *freqs: str):
     """Determine which frequency denotes the shortest or longest time period."""
     common_ts = pd.Timestamp("2020-01-01")
     ts = [common_ts + pd.tseries.frequencies.to_offset(fr) for fr in freqs]
     i = (np.argmin if shortest else np.argmax)(ts)
     return freqs[i]
 
@@ -143,15 +110,15 @@
     --------
     >>> freq.longest('MS', 'H', 'AS', 'D')
     'AS'
     """
     return _longestshortest(False, *freqs)
 
 
-def to_offset(freq: str) -> Union[pd.Timedelta, pd.DateOffset]:
+def to_offset(freq: str) -> pd.Timedelta | pd.DateOffset:
     """Object that can be added to a left-bound timestamp to find corresponding right-bound timestamp.
 
     Parameters
     ----------
     freq : str
         Frequency denoting the length of the time period.
 
@@ -226,15 +193,15 @@
     i: pd.DatetimeIndex, wanted: str = None, strict: bool = False
 ) -> pd.DatetimeIndex:
     """Try to read, infer, or force frequency of index.
 
     Parameters
     ----------
     i : pd.DatetimeIndex
-    wanted : str, optional
+    wanted : str, optional (default: None)
         Frequency to set. If none provided, try to infer.
     strict : bool, optional (default: False)
         If True, raise ValueError if a valid frequency is not found.
 
     Returns
     -------
     pd.DatetimeIndex
@@ -266,33 +233,32 @@
             raise ValueError(
                 f"The data has a non-allowed frequency. Must be one of {', '.join(FREQUENCIES)}; found '{freq}'."
             )
     return i
 
 
 def set_to_frame(
-    fr: Union[pd.Series, pd.DataFrame], wanted: str = None, strict: bool = False
-) -> Union[pd.Series, pd.DataFrame]:
+    fr: Series_or_DataFrame, wanted: str = None, strict: bool = False
+) -> Series_or_DataFrame:
     """Try to read, infer, or force frequency of frame's index.
 
     Parameters
     ----------
     fr : pd.Series or pd.DataFrame
     wanted : str, optional
         Frequency to set. If none provided, try to infer.
     strict : bool, optional (default: False)
         If True, raise ValueError if a valid frequency is not found.
 
     Returns
     -------
-    Union[pd.Series, pd.DataFrame]
+    pd.Series | pd.DataFrame
         Same type as ``fr``, with, if possible, a valid value for ``fr.index.freq``.
     """
     # Handle non-datetime-indices.
     if not isinstance(fr.index, pd.DatetimeIndex):
         raise ValueError(
             "The data does not have a datetime index and can therefore not have a frequency."
         )
 
-    fr = fr.copy()
-    fr.index = set_to_index(fr.index, wanted, strict)
-    return fr
+    i = set_to_index(fr.index, wanted, strict)
+    return fr.set_axis(i, axis=0)
```

### Comparing `portfolyo-0.5.8/portfolyo/tools/isboundary.py` & `portfolyo-0.6.0/portfolyo/tools/isboundary.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,79 @@
 """
 Check if timestamp is delivery period start (or end).
 """
 
 import datetime as dt
-from typing import Union
+from typing import overload
 
 import numpy as np
 import pandas as pd
 
 from . import freq as tools_freq
 from . import startofday as tools_startofday
 
 
 # Necessary because pd.DatetimeIndex.is_year_start is broken.
 # e.g.
 # i = pd.date_range('2020-01-01', freq='MS', periods=12)
 # i.is_year_start
 # array([False, False, False, False, False, False, False, False, False, False, False, True])
-def is_year_start(i: Union[pd.Timestamp, pd.DatetimeIndex]) -> Union[bool, np.ndarray]:
+@overload
+def is_year_start(i: pd.Timestamp) -> bool:
+    ...
+
+
+@overload
+def is_year_start(i: pd.DatetimeIndex) -> np.ndarray:
+    ...
+
+
+def is_year_start(i: pd.Timestamp | pd.DatetimeIndex) -> bool | np.ndarray:
     return (i.day == 1) & (i.month == 1)
 
 
-def is_quarter_start(
-    i: Union[pd.Timestamp, pd.DatetimeIndex]
-) -> Union[bool, np.ndarray]:
+@overload
+def is_quarter_start(i: pd.Timestamp) -> bool:
+    ...
+
+
+@overload
+def is_quarter_start(i: pd.DatetimeIndex) -> np.ndarray:
+    ...
+
+
+def is_quarter_start(i: pd.Timestamp | pd.DatetimeIndex) -> bool | np.ndarray:
     return (i.day == 1) & ((i.month - 1) % 3 == 0)
 
 
-def is_month_start(i: Union[pd.Timestamp, pd.DatetimeIndex]) -> Union[bool, np.ndarray]:
+@overload
+def is_month_start(i: pd.Timestamp) -> bool:
+    ...
+
+
+@overload
+def is_month_start(i: pd.DatetimeIndex) -> np.ndarray:
+    ...
+
+
+def is_month_start(i: pd.Timestamp | pd.DatetimeIndex) -> bool | np.ndarray:
     return i.day == 1
 
 
-def is_X_start(
-    i: Union[pd.Timestamp, pd.DatetimeIndex], freq: str
-) -> Union[bool, np.ndarray]:
+@overload
+def is_X_start(i: pd.Timestamp) -> bool:
+    ...
+
+
+@overload
+def is_X_start(i: pd.DatetimeIndex) -> np.ndarray:
+    ...
+
+
+def is_X_start(i: pd.Timestamp | pd.DatetimeIndex, freq: str) -> bool | np.ndarray:
     if freq == "MS":
         return is_month_start(i)
     elif freq == "QS":
         return is_quarter_start(i)
     elif freq == "AS":
         return is_year_start(i)
     else:
```

### Comparing `portfolyo-0.5.8/portfolyo/tools/leftandright.py` & `portfolyo-0.6.0/portfolyo/tools/leftandright.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/tools/right.py` & `portfolyo-0.6.0/portfolyo/tools/right.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/tools/righttoleft.py` & `portfolyo-0.6.0/portfolyo/tools/righttoleft.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/tools/round.py` & `portfolyo-0.6.0/portfolyo/tools/round.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/tools/stamp.py` & `portfolyo-0.6.0/portfolyo/tools/stamp.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/tools/standardize.py` & `portfolyo-0.6.0/portfolyo/tools/standardize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,164 @@
 """
 Standardizing series and dataframes to use as input for PfLine.
 """
 
-from typing import Union
-
 import pandas as pd
 from pytz import AmbiguousTimeError, NonExistentTimeError
 
 from . import freq as tools_freq
+from . import right as tools_right
 from . import righttoleft as tools_righttoleft
 from . import tzone as tools_tzone
+from .types import Series_or_DataFrame
 
 
-# TODO: remove 'Europe/Berlin' as default for ``tz``, use None instead.
 def frame(
-    fr: Union[pd.Series, pd.DataFrame],
+    fr: Series_or_DataFrame,
     force: str = None,
     bound: str = "left",
     *,
-    tz: str = "Europe/Berlin",
+    tz: str = None,
     floating: bool = True,
-    index_col: str = None,
-    force_freq: str = None,
-) -> Union[pd.Series, pd.DataFrame]:
+) -> Series_or_DataFrame:
     """Standardize a series or dataframe.
 
     Parameters
     ----------
     fr : pd.Series or pd.DataFrame
     force : {'aware', 'agnostic'}, optional (default: None)
-        Force ``fr`` to be timezone aware or timezone agnostic. If None: keep index
-        as-is.
+        Force returned frame to be timezone aware or timezone agnostic. Timezone aware
+        means that the index has a timezone, like UTC or Europe/Berlin. Timezone agnostic
+        means that the index shows wall time with 24h days without DST. If None: keep
+        timezone as-is.
     bound : {'left', 'right'}, optional (default: 'left')
-        If 'left' ('right'), specifies that input timestamps are left-(right-)bound.
+        If 'right', specifies that input timestamps are right-bound, and will change to
+        left-bound.
     tz : str, optional (default: None)
-        The timezone in which to interpret non-localized values. If ``force`` ==
-        'aware': also the timezone to localize to. Ignored if ``force`` is None.
+        Timezone. Timezone to convert the values into and/or to interpret values in.
+        - If ``force`` is None, this argument is ignored.
+        - If the index is timezone agnostic and ``force`` is 'aware', the frame values
+          are interpreted as being in this timezone. E.g., if 'Europe/Berlin', the final
+          Sunday in March already has 23h; all that's needed is to set the timezone.
+        - If the index is timezone agnostic and ``force`` is 'agnostic', the same is
+          done, but followed with a conversion to timezone-agnostic frame.
+        - If the index is timezone aware and ``force`` is 'aware', the values are
+          converted to timezone ``tz``. See parameter ``floating``.
+        - If the index is timezone aware and ``force`` is 'agnostic', this argument is
+          ignored.
     floating : bool, optional (default: True)
         If ``force`` == 'aware': how to convert to ``tz`` if ``fr`` has other timezone.
         Keep local time (``floating`` == True) or keep universal time (``floating`` ==
         False). Ignored if ``force`` == 'agnostic' or None.
-    index_col : str, optional
-        Column to create the timestamp from. Use existing index if none specified.
-        Ignored if ``fr`` is not a DataFrame.
-    force_freq : str, optional
-        If a frequency cannot be inferred from the data (e.g. due to gaps), it is
-        resampled at this frequency. Default: raise Exception.
 
     Returns
     -------
-    Union[pd.Series, pd.DataFrame]
+    pd.Series | pd.DataFrame
         Same type as ``fr``, with a left-bound DatetimeIndex, a valid frequency, and
         wanted timezone.
 
     Notes
     -----
     It is assumed that we are dealing with "time-averable" data, such as values in [MW]
     or [Eur/MWh]. This is especially important when converting daily (and longer) values
-    between a tz-agnostic context and a tz-aware context with DST-transitions.
+    between a tz-agnostic context and a tz-aware context with DST-transitions. The value
+    on a 23-hour day is used as-is when convertintg to a 24-hour day.
 
     See also
     --------
     ``portfolyo.force_aware``
     ``portfolyo.force_agnostic``
     """
-    kwargs = {"tz": tz, "floating": floating, "force_freq": force_freq}
-
     # Set index.
-    if index_col and isinstance(fr, pd.DataFrame):
-        fr = fr.set_index(index_col)
-    else:
-        fr = fr.copy()  # don't change passed-in fr
-    fr.index = pd.DatetimeIndex(fr.index)  # turn / try to turn into datetime
+    fr = fr.set_axis(pd.DatetimeIndex(fr.index))  # turn / try to turn into datetime
 
     # We want to cover 2 additional cases for convenience sake:
     # a. The user passes a frame that still needs to be localized (--> freq unknown)
     # b. The user passes a frame that is not left-bound (--> freq needed)
 
     # Make sure it has a frequency, i.e., make sure it is tz-aware or tz-agnostic.
     # Pipeline if frequency not yet found: right -> left -> localize -> tz-aware -> freq
     fr = tools_freq.set_to_frame(fr)
     freq_input, tz_input = fr.index.freq, fr.index.tz
 
     # The data may be right-bound.
 
     if bound == "right":  # right -> left
-        for how in ["A", "B"]:
-            try:
-                fr_left = fr.set_axis(tools_righttoleft.index(fr.index, how))
-                return frame(fr_left, force, "left", **kwargs)
-            except ValueError as e:
-                if how == "B":
-                    raise ValueError("Cannot make this frame left-bound.") from e
-                pass
+        return _fix_rightbound(fr, force, tz, floating)
 
     # Now the data is left-bound.
     # If the frequency is not found, and it is tz-naive, the index may need to be localized.
 
     if not freq_input and not tz_input and tz:  # left -> tz-aware (try)
         # fr is tz-agnostic.
         try:
             fr_aware = fr.tz_localize(tz, ambiguous="infer")
         except (AmbiguousTimeError, NonExistentTimeError):
             pass  # fr did not need / cound not be localized. Continue with fr as-is.
         else:
             # Could be localized. Again remove localization if force == 'agnostic' or None.
             force_to = force or "agnostic"
-            return frame(fr_aware, force_to, "left", **kwargs)
+            return frame(fr_aware, force_to, "left", tz=tz, floating=floating)
 
     # All options to infer frequency have been exhausted. One may or may not have been found.
     # Does the user want to force a frequency?
 
-    if not freq_input and force_freq:
-        # No freq has been found, but user specifies which freq it should be.
-        fr_withfreq = fr.asfreq(force_freq)
-        return frame(fr_withfreq, force, "left", tz=tz, floating=floating)
-
-    elif not freq_input and not force_freq:
+    if not freq_input:
         # No freq has been bound, and user specifies no freq either.
         raise ValueError(
-            "A frequency could not be inferred for this data. Force a frequency (by passing the"
-            " ``force_freq`` parameter), or localize the data in advance (with ``fr.tz_localize()``)."
-        )
-
-    elif freq_input and force_freq and force_freq != freq_input:
-        # Freq has been found, but user specifies it should be a different freq.
-        raise ValueError(
-            f"This data seems to have a frequency {freq_input}, which is different from the frequency"
-            f" the user wants to force on it {force_freq}. Note that the ``force_freq`` parameter is"
-            " for filling gaps in the input data. It should not be used for resampling! If the"
-            " data has e.g. daily values but you want monthly values, use ``force_freq='D'``, and"
-            " pass the return value to one of the functions in the ``portfolyo.tools.changefreq`` module."
+            "A frequency could not be inferred for this data. This can be because there are"
+            " gaps in the data (use ``fr.asfreq()`` to replace gaps with NaN), or because"
+            " the index must be localized (with ``fr.tz_localize()``)."
         )
 
-    # Now the data has frequency set. It is tz-aware (possibly with wrong tz) or tz-agnostic.
+        # Now the data has frequency set. It is tz-aware (possibly with wrong tz) or tz-agnostic.
 
     # Fix timezone.
-    if force == "aware":
-        fr = tools_tzone.force_aware(fr, tz, floating=floating)
-    elif force == "agnostic" or force == "naive":
-        fr = tools_tzone.force_agnostic(fr)
-    elif force is None:  # don't try to fix timezone.
-        pass
-    else:
-        raise ValueError(
-            f"Parameter ``force`` must be one of 'aware', 'agnostic'; got {force}."
-        )
+    fr = _fix_timezone(fr, force, tz, floating)
 
     # Check if index is OK; otherwise raise error.
     try:
         assert_frame_standardized(fr)
     except AssertionError as e:
         raise ValueError("Could not standardize this frame") from e
 
     # Standardize index name.
-    fr.index.name = "ts_left"
+    fr = _standardize_index_name(fr)
     # After standardizing timezone, the frequency should have been set.
-    return tools_freq.set_to_frame(fr, freq_input, strict=force_freq)
+    return tools_freq.set_to_frame(fr, freq_input, strict=True)
+
+
+def _fix_rightbound(fr, force, tz, floating):
+    for how in ["A", "B"]:
+        try:
+            i_left = tools_righttoleft.index(fr.index, how)
+            fr_left = fr.set_axis(i_left)
+            return frame(fr_left, force, "left", tz=tz, floating=floating)
+        except ValueError:
+            pass
+    raise ValueError("Cannot make this frame left-bound.")
+
+
+def _fix_timezone(fr, force, tz, floating):
+    if force is None:
+        return fr
+    elif force == "aware":
+        return tools_tzone.force_aware(fr, tz, floating=floating)
+    elif force == "agnostic" or force == "naive":
+        return tools_tzone.force_agnostic(fr)
+    raise ValueError(
+        f"Parameter ``force`` must be None, 'aware' or 'agnostic'; got {force}."
+    )
 
 
-def assert_frame_standardized(fr: Union[pd.Series, pd.DataFrame]):
+def _standardize_index_name(fr: Series_or_DataFrame) -> Series_or_DataFrame:
+    return fr.rename_axis(index="ts_left")
+
+
+def assert_frame_standardized(fr: Series_or_DataFrame) -> None:
     """Assert that series or dataframe is standardized."""
     assert_index_standardized(fr.index)
 
 
 def assert_index_standardized(i: pd.DatetimeIndex, __right: bool = False):
     """Assert that index is standardized."""
 
@@ -185,15 +180,15 @@
 
     # Check hour and minute.
     if tools_freq.up_or_down(freq, "15T") <= 0:  # quarterhour
         startminute = 15 if __right else 0
         if i[0].minute != startminute:
             err = ("right-bound", "15 min past the") if __right else ("", "at a full")
             raise AssertionError(
-                f"An index with {err[0]} quarterhourly values must start {err[1]} hour; found {i[0]}."
+                f"The first element in an index with {err[0]} quarterhourly values must be {err[1]} hour; found {i[0]}."
             )
 
         if any(not_ok := [ts.minute not in (0, 15, 30, 45) for ts in i]):
             raise AssertionError(
                 "In an index with quarterhourly values, all timestamps (all periods) should"
                 f" start at a full quarter-hour; found {i[not_ok]}."
             )
@@ -201,15 +196,28 @@
         if any(not_ok := i.minute != 0):
             raise AssertionError(
                 "In an index with hourly-or-longer values, all timestamps (all periods) should"
                 f" start at a full hour; found {i[not_ok]}."
             )
 
     # Check time-of-day.
-    if tools_freq.up_or_down(freq, "D") >= 0:
+    if tools_freq.up_or_down(freq, "H") <= 0:  # hour or shorter
+        if not __right:
+            start = i[0]
+            end = tools_right.stamp(i[-1], i.freq)
+        else:
+            start = tools_righttoleft.index(i)[0]
+            end = i[-1]
+        if start.time() != end.time():
+            raise AssertionError(
+                "An index must contain full days. For hourly-or-shorter values, this means "
+                f"that the start time of the first period ({start}) must equal the end time of the "
+                f"last period ({end}), which is not the case."
+            )
+    else:  # days or longer
         if not len(times := set(i.time)) == 1:
             raise AssertionError(
                 "In an index with daily-or-longer values, all timestamps (all periods) should"
                 f" start at the same time. Found multiple times: {times}."
             )
 
     # Check day-of-X.
```

### Comparing `portfolyo-0.5.8/portfolyo/tools/startofday.py` & `portfolyo-0.6.0/portfolyo/tools/startofday.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,88 @@
 """
 Tools to get/set start-of-day.
 """
 
+import datetime as dt
 
 import pandas as pd
+
 from . import freq as tools_freq
-import datetime as dt
-from typing import Union
+from . import right as tools_right
 
 
-def get(
-    i: pd.DatetimeIndex, returntype: str = "time"
-) -> Union[dt.time, str, dt.timedelta]:
+def get(i: pd.DatetimeIndex, returntype: str = "time") -> dt.time | str | dt.timedelta:
     """Get start-of-day of an index.
 
     Parameters
     ----------
     i : pd.DatetimeIndex
     returntype : {'time', 'str', 'timedelta'}, optional (default: 'time')
         If 'time', return as datetime.time object.
         If 'str', return as HH:MM:SS string.
         If 'timedelta', return as datetime.timedelta object with timedelta to previous
         midnight (24h day).
 
     Returns
     -------
-    Union[dt.time, str]
+    dt.time | str | dt.timedelta
     """
     start_of_day = i[0].time()
     if returntype == "time":
         return start_of_day
     elif returntype == "str":
         return f"{start_of_day.hour:02}:{start_of_day.minute:02}:00"
     elif returntype == "timedelta":
         return dt.timedelta(hours=start_of_day.hour, minutes=start_of_day.minute)
     raise ValueError(
         f"Unknown value for parameter 'returntype'. Expected one of {'time', 'str', 'timedelta'}, got {returntype}."
     )
 
 
-def set(i: pd.DatetimeIndex, start_of_day: dt.time = None) -> pd.DatetimeIndex:
-    """Set the start-of-day of an index by changing the time-part of the index elements.
+def set(i: pd.DatetimeIndex, start_of_day: dt.time) -> pd.DatetimeIndex:
+    """Set the start-of-day of an index. Done by changing the time-part of the index
+    elements (if index has daily-or-longer frequency) or by trimming the index (if index
+    has hourly-or-shorter frequency).
 
     Parameters
     ----------
     i : pd.DatetimeIndex
-        Index; must have a daily (or longer) frequency.
-    start_of_day : dt.time, optional (default: midnight)
-        The new time that replaces the time-part of index elements.
+    start_of_day : dt.time
 
     Returns
     -------
     pd.DatetimeIndex
-        With adjusted time-part. Date-part is unchanged, so new timestamps are on same
-        calendar day as original timestamps.
+        With wanted start-of-day.
     """
-    if tools_freq.up_or_down(i.freq, "D") < 0:
-        raise ValueError(
-            "Can only set the start-of-day of an index with daily (or longer) frequency."
-        )
-
-    if start_of_day is None:
-        start_of_day = dt.time(hour=0, minute=0, second=0)
-    elif start_of_day.second != 0 or start_of_day.minute % 15 != 0:
+    if start_of_day.second != 0 or start_of_day.minute % 15 != 0:
         raise ValueError("Start of day must coincide with a full quarterhour.")
 
+    if tools_freq.up_or_down(i.freq, "D") >= 0:
+        return _set_to_longfreq(i, start_of_day)
+    else:
+        return _set_to_shortfreq(i, start_of_day)
+
+
+def _set_to_longfreq(i: pd.DatetimeIndex, start_of_day: dt.time) -> pd.DatetimeIndex:
+    """Set start-of-day of index with daily-or-longer frequency."""
     tss = (ts.replace(hour=start_of_day.hour, minute=start_of_day.minute) for ts in i)
     return pd.DatetimeIndex(tss, freq=i.freq, tz=i.tz)
+
+
+def _set_to_shortfreq(i: pd.DatetimeIndex, start_of_day: dt.time) -> pd.DatetimeIndex:
+    """Set start-of-day of index with hourly-or-shorter frequency. Destructive; values
+    at start and/or end of index are removed to get wanted start_of_day."""
+    # Remove from start if necessary.
+    for _ in range(0, 100):  # max 100 quarterhours in a day (@ end of DST)
+        if i[0].time() == start_of_day:
+            break
+        i = i[1:]
+    else:
+        raise ValueError("Did not find any timestamp with correct time at index start.")
+    # Remove from end if necessary.
+    for _ in range(0, 100):  # max 100 quarterhours in a day (@ end of DST)
+        if tools_right.stamp(i[-1], i.freq).time() == start_of_day:
+            break
+        i = i[:-1]
+    else:
+        raise ValueError("Did not find any timestamp with correct time at index end.")
+    return i
```

### Comparing `portfolyo-0.5.8/portfolyo/tools/trim.py` & `portfolyo-0.6.0/portfolyo/tools/trim.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Trim objects to only contain 'full' delivery periods.
 """
 
-from typing import Union
+from typing import overload
 
 import pandas as pd
 
 from . import ceil as tools_ceil
 from . import floor as tools_floor
 from . import freq as tools_freq
-from . import startofday as tools_startofday
 from . import right as tools_right
+from . import startofday as tools_startofday
 
 
 def index(i: pd.DatetimeIndex, freq: str) -> pd.DatetimeIndex:
     f"""Trim index to only keep full periods of certain frequency.
 
     Parameters
     ----------
@@ -43,29 +43,37 @@
     # Trim on both sides.
     mask_start = i >= tools_ceil.stamp(i[0], freq, 0, start_of_day)
     i_right = tools_right.index(i)
     mask_end = i_right <= tools_floor.stamp(i_right[-1], freq, 0, start_of_day)
     return i[mask_start & mask_end]
 
 
-def frame(
-    fr: Union[pd.Series, pd.DataFrame], freq: str
-) -> Union[pd.Series, pd.DataFrame]:
+@overload
+def frame(fr: pd.Series, freq: str) -> pd.Series:
+    ...
+
+
+@overload
+def frame(fr: pd.DataFrame, freq: str) -> pd.DataFrame:
+    ...
+
+
+def frame(fr: pd.Series | pd.DataFrame, freq: str) -> pd.Series | pd.DataFrame:
     f"""Trim index of series or dataframe to only keep full periods of certain frequency.
 
     Parameters
     ----------
-    fr : Union[pd.Series, pd.DataFrame]
+    fr : Series or DataFrame
         The (untrimmed) pandas series or dataframe.
     freq : {{{', '.join(tools_freq.FREQUENCIES)}}}
         Frequency to trim to. E.g. 'MS' to only keep full months.
 
     Returns
     -------
-    Union[pd.Series, pd.DataFrame]
+    Series or DataFrame
         Subset of ``fr``, with same frequency.
 
     Notes
     -----
     For shorter-than-daily indices, it is assumed that the index starts with a full day.
     I.e., the time-of-day of the first element is assumed to be the start time for the
     day-or-longer delivery periods. (E.g., if the index has hourly values and starts with
```

### Comparing `portfolyo-0.5.8/portfolyo/tools/tzone.py` & `portfolyo-0.6.0/portfolyo/tools/tzone.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Tools to deal with timezones."""
 
-from typing import Union
-
 import pandas as pd
 import pytz
 
 from . import freq as tools_freq
+from .types import Series_or_DataFrame
 
 """
 (hourly means: hourly or shorter)
 (daily means: daily or longer)
 
 We consider 3 types of gapless datetime indices:
 A: tz-aware indices. These are never ambiguous, and a freq can always be set.
@@ -52,16 +51,16 @@
 . a type C with gaps.
 . a type C with hourly values which do include a DST-transition.
 It's therefore hard to determine, which it is.
 """
 
 
 def force_aware(
-    fr: Union[pd.Series, pd.DataFrame], tz: str, *, floating: bool = True
-) -> Union[pd.Series, pd.DataFrame]:
+    fr: Series_or_DataFrame, tz: str, *, floating: bool = True
+) -> Series_or_DataFrame:
     """Convert/set series or dataframe to a specific timezone.
 
     Parameters
     ----------
     fr : pd.Series or pd.DataFrame
         with tz-aware or (standardized) tz-agnostic index.
     tz : str
@@ -132,17 +131,15 @@
         fr_out = _B_to_A(fr, tz=tz)
 
     # Return: set frequency.
     fr_out = tools_freq.set_to_frame(fr_out, freq_input)
     return fr_out
 
 
-def force_agnostic(
-    fr: Union[pd.Series, pd.DataFrame]
-) -> Union[pd.Series, pd.DataFrame]:
+def force_agnostic(fr: Series_or_DataFrame) -> Series_or_DataFrame:
     """Turn a frame (series or dataframe) into timezone-agnostic frame.
 
     Parameters
     ----------
     fr : pd.Series or pd.DataFrame
         with tz-aware or (standardized) tz-agnostic index.
 
@@ -191,17 +188,15 @@
         fr_out = fr
 
     # Return: set frequency.
     fr_out = tools_freq.set_to_frame(fr_out, freq_input)
     return fr_out
 
 
-def _A_to_A(
-    fr: Union[pd.Series, pd.DataFrame], *, tz, floating
-) -> Union[pd.Series, pd.DataFrame]:
+def _A_to_A(fr: Series_or_DataFrame, *, tz: str, floating: bool) -> Series_or_DataFrame:
     if isinstance(tz, str):  # convert to make comparison (below) possible
         tz = pytz.timezone(tz)
 
     if fr.index.tz == tz:
         # input already has wanted tz; no conversion necessary
         return fr
 
@@ -211,40 +206,36 @@
 
     else:
         # conversion by keeping local time
         # Defer to A -> B -> A
         return _B_to_A(_A_to_B(fr), tz=tz)
 
 
-def _A_to_B(fr: Union[pd.Series, pd.DataFrame]) -> Union[pd.Series, pd.DataFrame]:
+def _A_to_B(fr: Series_or_DataFrame) -> Series_or_DataFrame:
     return _aware_to_agnostic(fr)
 
 
-def _B_to_A(
-    fr: Union[pd.Series, pd.DataFrame], *, tz
-) -> Union[pd.Series, pd.DataFrame]:
+def _B_to_A(fr: Series_or_DataFrame, *, tz) -> Series_or_DataFrame:
     return _agnostic_to_aware(fr, tz)
 
 
-def _idx_after_conversion(fr: Union[pd.Series, pd.DataFrame], tz) -> pd.DatetimeIndex:
+def _idx_after_conversion(fr: Series_or_DataFrame, tz) -> pd.DatetimeIndex:
     fr = tools_freq.set_to_frame(fr)
     freq_input = fr.index.freq
     if not freq_input:
         raise ValueError("Cannot recalculate values if frequency is not known.")
 
     # Index of output frame.
     start, end = fr.index[0].tz_localize(tz), fr.index[-1].tz_localize(tz)
     idx = pd.date_range(start, end, freq=freq_input, tz=tz)
 
     return idx
 
 
-def _agnostic_to_aware(
-    fr: Union[pd.Series, pd.DataFrame], tz: str
-) -> Union[pd.Series, pd.DataFrame]:
+def _agnostic_to_aware(fr: Series_or_DataFrame, tz: str) -> Series_or_DataFrame:
     """Recalculate values in tz-agnostic series or dataframe, to get a tz-aware one.
     (i.e., B to A)."""
     if tz_input := fr.index.tz:
         raise ValueError(f"``fr`` must be tz-agnostic; found timezone '{tz_input}'.")
     if not tz:
         raise ValueError("Must specify timezone ``tz`` to convert into.")
 
@@ -259,17 +250,15 @@
     # Convert hourly or shorter.
     # There may be multiple timestamps in output receiving same input value. (And some
     # that are lost). But importantly: each timestamp in output exists in input.
     mapping_onto_input_index = idx_out.tz_localize(None)
     return fr.loc[mapping_onto_input_index].set_axis(idx_out)
 
 
-def _aware_to_agnostic(
-    fr: Union[pd.Series, pd.DataFrame]
-) -> Union[pd.Series, pd.DataFrame]:
+def _aware_to_agnostic(fr: Series_or_DataFrame) -> Series_or_DataFrame:
     """Recalculate values in tz-aware series or dataframe, to get a tz-agnostic one.
     (i.e., A to B)."""
     if not fr.index.tz:
         raise ValueError("``fr`` must be tz-aware.")
 
     idx_out = _idx_after_conversion(fr, None)
```

### Comparing `portfolyo-0.5.8/portfolyo/tools/unit.py` & `portfolyo-0.6.0/portfolyo/tools/unit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Working with pint units.
 """
 
 from pathlib import Path
-from typing import Tuple, Union
+from typing import Tuple, overload
 
 import pandas as pd
 import pint
 import pint_pandas
 
 path = Path(__file__).parent / "unitdefinitions.txt"
 
@@ -49,17 +49,37 @@
 def from_name(name: str) -> pint.Unit:
     """Find standard unit belonging to a column name."""
     if name in NAMES_AND_UNITS:
         return NAMES_AND_UNITS[name]
     raise ValueError(f"No standard unit found for name '{name}'.")
 
 
+@overload
+def defaultunit(val: int | float) -> float:
+    ...
+
+
+@overload
+def defaultunit(val: pint.Quantity) -> pint.Quantity:
+    ...
+
+
+@overload
+def defaultunit(val: pd.Series) -> pd.Series:
+    ...
+
+
+@overload
+def defaultunit(val: pd.DataFrame) -> pd.DataFrame:
+    ...
+
+
 def defaultunit(
-    val: Union[int, float, pint.Quantity, pd.Series, pd.DataFrame],
-) -> Union[float, pint.Quantity, pd.Series, pd.DataFrame]:
+    val: int | float | pint.Quantity | pd.Series | pd.DataFrame,
+) -> float | pint.Quantity | pd.Series | pd.DataFrame:
     """Convert ``val`` to base units. Also turns dimensionless values into floats.
 
     Parameters
     ----------
     val : int, float, pint.Quantity, pd.Series, or pd.DataFrame
         The value to convert to base units.
 
@@ -97,23 +117,34 @@
         else:  # series of floats, bools, timestamps, ...
             return val
     elif isinstance(val, pd.DataFrame):
         return pd.DataFrame({col: defaultunit(s) for col, s in val.items()})
     raise TypeError("``val`` must be an int, float, Quantity, Series, or DataFrame.")
 
 
+@overload
+def split_magn_unit(val: int | float) -> Tuple[float, None]:
+    ...
+
+
+@overload
+def split_magn_unit(val: pint.Quantity) -> Tuple[float, None | pint.Unit]:
+    ...
+
+
+@overload
+def split_magn_unit(
+    val: pd.Series,
+) -> Tuple[pd.Series, None | pint.Unit | pd.Series]:
+    ...
+
+
 def split_magn_unit(
-    val: Union[int, float, pint.Quantity, pd.Series]
-) -> Union[
-    Tuple[float, None],
-    Tuple[float, pint.Unit],
-    Tuple[pd.Series, None],
-    Tuple[pd.Series, pint.Unit],
-    Tuple[pd.Series, pd.Series],
-]:
+    val: int | float | pint.Quantity | pd.Series,
+) -> Tuple[float, None | pint.Unit] | Tuple[pd.Series, None | pint.Unit | pd.Series]:
     """Split ``val`` into magnitude and units. If ``val`` is a Series with uniform
     dimension, the unit is returned as a pint Unit. If not, it is returned as a Series.
     """
     val = defaultunit(val)
     if isinstance(val, pint.Quantity):
         return val.magnitude, val.units
     elif isinstance(val, pd.Series):
```

### Comparing `portfolyo-0.5.8/portfolyo/tools/unitdefinitions.txt` & `portfolyo-0.6.0/portfolyo/tools/unitdefinitions.txt`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.8/portfolyo/tools/wavg.py` & `portfolyo-0.6.0/portfolyo/tools/wavg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,109 +1,125 @@
-from typing import Iterable, Mapping, Union
+from typing import Iterable, Mapping, overload
 
 import numpy as np
 import pandas as pd
 
 from . import unit as tools_unit
 
 # Developer notes:
 # HACK: for speed:
 # meaning: for series and dataframes with pint quantities, .sum() does not work,
 # and .apply(np.sum) is really slow. The workaround is fast also for pint quantities.
 
 # Developer notes:
 # The following behaviour is wanted in calculating the weighted average:
 
-# weights            values              rule | result
+# weights            values              rule                           result
 
 # sum of weights != 0
-# 1, -1, 2           10, 20, 30          normal | (10*1 + 20*-1 + 30*2 ) / (1 + -1 + 2)
-# 1, -1, 2           10, NaN, 30         NaN if values include NaN | NaN
-# 1, 0, 2            10, NaN, 30         ignore NaN if weight = 0 | (10*1 + 30*2) / (1 + 2)
+# 1, -1, 2           10, 20, 30          "normal"                       (10*1 + 20*-1 + 30*2 ) / (1 + -1 + 2)
+# 1, -1, 2           10, NaN, 30         NaN if values include NaN      NaN
+# 1, 0, 2            10, NaN, 30         ignore NaN if weight = 0       (10*1 + 30*2) / (1 + 2)
 # --> Remove all values for which weight == 0.
 # --> If remaining values conain NaN --> result is NaN.
 # --> Otherwise, calculate the result normally.
 
 # sum of weights == 0 but not all 0
-# 1, 1, -2           10, 20, 30          Inf if values distinct | Inf
-# 1, 1, -2           10, 10, 10          value if values identical | 10
-# 1, -1, 0           10, 10, 30          ignore value if weight = 0 | 10
-# 1, 1, -2           10, 10, NaN         NaN if values include NaN | NaN (done)
-# 1, -1, 0           10, 10, NaN         ignore NaN if weight = 0 | 10
-# 1, -1, 0           NaN, NaN, NaN       NaN if values are all NaN | NaN
+# 1, 1, -2           10, 20, 30          NaN if values distinct         NaN
+# 1, 1, -2           10, 10, 10          value if values identical      10
+# 1, -1, 0           10, 10, 30          ignore value if weight = 0     10
+# 1, 1, -2           10, 10, NaN         NaN if values include NaN      NaN
+# 1, -1, 0           10, 10, NaN         ignore NaN if weight = 0       10
+# 1, -1, 0           NaN, NaN, NaN       NaN if values are all NaN      NaN
 # --> Remove all values for which weight == 0.
 # --> If remaining values contain NaN --> result is NaN
 # --> Otherwise, if remaining values are identical --> result is that value
 # --> Otherwise, result is Inf.
 
 # all weights are 0
-# 0, 0, 0            10, 20, 30          Inf if values distinct | Inf
-# 0, 0, 0            10, 10, 10          value if values identical | 10
-# 0, 0, 0            10, 10, NaN         NaN if values include NaN | NaN
+# 0, 0, 0            10, 20, 30          NaN if values distinct         NaN
+# 0, 0, 0            10, 10, 10          Value if values identical      10
+# 0, 0, 0            10, 10, NaN         NaN if values include NaN      NaN
 # --> If values contain NaN --> result is NaN
 # --> Otherwise, if values are identical --> result is that value
-# --> Otherwise, result is Inf.
+# --> Otherwise, result is NaN.
 
 RESULT_IF_WEIGHTSUM0_VALUESNOTUNIFORM = np.nan
 
 
+@overload
+def general(
+    fr: pd.Series, weights: Iterable | Mapping | pd.Series = None, axis: int = 0
+) -> float:
+    ...
+
+
+@overload
+def general(
+    fr: pd.DataFrame,
+    weights: Iterable | Mapping | pd.Series | pd.DataFrame = None,
+    axis: int = 0,
+) -> pd.Series:
+    ...
+
+
 def general(
-    fr: Union[pd.Series, pd.DataFrame],
-    weights: Union[Iterable, pd.Series, pd.DataFrame] = None,
+    fr: pd.Series | pd.DataFrame,
+    weights: Iterable | Mapping | pd.Series | pd.DataFrame = None,
     axis: int = 0,
-) -> Union[pd.Series, float]:
+) -> float | tools_unit.Q_ | pd.Series:
     """
     Weighted average of series or dataframe.
 
     Parameters
     ----------
-    fr : Union[pd.Series, pd.DataFrame]
+    fr : pd.Series | pd.DataFrame
         The input values.
-    weights : Union[Iterable, pd.Series, pd.DataFrame], optional
-        The weights. If provided as a Series, the weights and values are aligned along
-        its index. If no weights are provided, the normal (unweighted) average is returned
-        instead.
+    weights : Iterable | Mapping | pd.Series | pd.DataFrame, optional
+        The weights. If provided as a Mapping or Series, the weights and values
+        are aligned along its index. If no weights are provided, the normal
+        (unweighted) average is returned instead.
     axis : int, optional
         Calculate each column's average over all rows (if axis==0, default) or
         each row's average over all columns (if axis==1). Ignored for Series.
 
     Returns
     -------
-    Union[pd.Series, float]
-        The weighted average. A single float if `fr` is a Series; a Series if
-        `fr` is a Dataframe.
+    float | Q_ | pd.Series
+        The weighted average. A single float or single Quantitiy if ``fr`` is a Series;
+        a Series if ``fr`` is a Dataframe.
     """
     if isinstance(fr, pd.DataFrame):
         return dataframe(fr, weights, axis)
     elif isinstance(fr, pd.Series):
         return series(fr, weights)
     else:
         raise TypeError(
             f"Parameter ``fr`` must be Series or DataFrame; got {type(fr)}."
         )
 
 
 def series(
-    s: pd.Series, weights: Union[Iterable, Mapping, pd.Series] = None
-) -> Union[float, tools_unit.Q_]:
+    s: pd.Series, weights: Iterable | Mapping | pd.Series = None
+) -> float | tools_unit.Q_:
     """
     Weighted average of series.
 
     Parameters
     ----------
     s : pd.Series
         The input values.
-    weights : Union[Iterable, Mapping, pd.Series], optional
+    weights : Iterable | Mapping | pd.Series, optional
         The weights. If provided as a Mapping or Series, the weights and values are
         aligned along their indices/keys. If no weights are provided, the normal
         (unweighted) average is returned instead.
 
     Returns
     -------
-    Union[float, Quantity]
+    float | Quantity
         The weighted average.
 
     Notes
     -----
     Will raise Error if values in ``s`` have distinct units.
     """
     # Unweighted average if no weights provided.
@@ -113,14 +129,19 @@
     # Prep: ensure weights is also a Series.
     weights = weights_as_series(weights, s.index)
     # Keep only relevant section.
     try:
         s = s.loc[weights.index]
     except KeyError as e:  # more weights than values
         raise ValueError("No values found for one or more weights.") from e
+
+    # Unweighted average if all weights the same but not all 0.
+    if weights.nunique() == 1 and not np.isclose(weights.iloc[0], 0):
+        return s.mean()
+
     # Replace NaN with 0 in locations where it doesn't change the result.
     replaceable = s.isna() & (weights == 0.0)
     s[replaceable] = 0.0
 
     # If we arrive here, ``s`` only has NaN on locations where weight != 0.
 
     # Check if ALL weights are 0.
@@ -149,25 +170,25 @@
     factors = weights.div(weightsum).astype(float)
     scaled_values = s * factors  # fast, even with quantities
     return sum(scaled_values)
 
 
 def dataframe(
     df: pd.DataFrame,
-    weights: Union[Iterable, Mapping, pd.Series, pd.DataFrame] = None,
+    weights: Iterable | Mapping | pd.Series | pd.DataFrame = None,
     axis: int = 0,
 ) -> pd.Series:
     """
     Weighted average of dataframe.
 
     Parameters
     ----------
     df : pd.DataFrame
         The input values.
-    weights : Union[Iterable, Mapping, pd.Series, pd.DataFrame], optional
+    weights : Iterable | Mapping | pd.Series | pd.DataFrame, optional
         The weights. If provided as a Series or Mapping, its index are is used for
         alignment (with ``df``'s index if axis==0, or its columns if axis==1). If no
         weights are provided, the normal (unweighted) average is returned instead.
     axis : int, optional (default: 0)
         - if 0, calculate average over all rows (for each column);
         - if 1, calculate average over all columns (for each row).
 
@@ -302,29 +323,29 @@
 
     # Every index value of weights is now in exactly one series.
     return concatseries(series, originalindex)
 
 
 def _dataframe_columnwavg_with_weightssumnot0(
     df: pd.DataFrame,
-    weights: Union[pd.Series, pd.DataFrame],
-    weightssum: Union[float, tools_unit.Q_, pd.Series],
+    weights: pd.Series | pd.DataFrame,
+    weightssum: float | tools_unit.Q_ | pd.Series,
 ) -> Iterable[pd.Series]:
     # Calculate the weighted average if sum of weights != 0.
     weight_is0 = weights == 0.0
     value_isna = df.isna()
     df = df.where(~(weight_is0 & value_isna), other=0.0)  # to ignore NaN if allowed
     factors = weights.div(weightssum, axis=0).astype(float)
     scaled_values = df * factors  # fast, even with quantities
     result = sum(s for _, s in scaled_values.items())  # HACK: for speed
     return [result]
 
 
 def _dataframe_columnwavg_with_weightssum0notall0(
-    df: pd.DataFrame, weights: Union[pd.Series, pd.DataFrame]
+    df: pd.DataFrame, weights: pd.Series | pd.DataFrame
 ) -> Iterable[pd.Series]:
     # Calculate the weighted average if sum of weights == 0, but not all weights are 0.
 
     series = []
 
     if len(df.index) == 0:
         return series
@@ -395,15 +416,15 @@
     # - Observe second column. Ignore NaN. For not-NaN: if buffer is empty, put in buffer.
     #   If buffer is not empty, compare. If not same, put uniform-flag to False.
     # - Continue for other columns.
     # Uniform flag is now set to False for non-uniform rows. For rows with uniform values
     # or uniform NaN, this value/NaN is found in buffer.
     uniform = pd.Series(True, df.index)
     buffer = pd.Series(np.nan, df.index)  # define to ensure exists even if df empty
-    for i, (c, s) in enumerate(df.items()):
+    for i, (_, s) in enumerate(df.items()):
         if i == 0:
             # define here to ensure ``values`` has pint dtype if df does too
             to_type = float if pd.api.types.is_integer_dtype(s.dtype) else s.dtype
             buffer = pd.Series(np.nan, s.index).astype(to_type)
         must_compare = s.notna() & buffer.notna()
         if must_compare.any():
             # HACK: cannot use ``uniform & (...)`` because must_compare has partial index, and missing values are set to False
@@ -412,17 +433,15 @@
         if must_replace.any():
             buffer = buffer.fillna(s[must_replace])
 
     buffer[~uniform] = RESULT_IF_WEIGHTSUM0_VALUESNOTUNIFORM
     return buffer
 
 
-def weights_as_series(
-    weights: Union[Iterable, Mapping], refindex: Iterable
-) -> pd.Series:
+def weights_as_series(weights: Iterable | Mapping, refindex: Iterable) -> pd.Series:
     if isinstance(weights, pd.Series):
         return weights
     if isinstance(weights, Mapping):
         return pd.Series(weights)
     if isinstance(weights, Iterable):
         return pd.Series(weights, refindex)
     raise TypeError("``weights`` must be iterable or mapping.")
```

### Comparing `portfolyo-0.5.8/portfolyo/visualize/categories.py` & `portfolyo-0.6.0/portfolyo/tools/visualize/categories.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
-from typing import Any, Iterable, Union
+from typing import Any, Iterable
 
 import numpy as np
 import pandas as pd
 
-from .. import tools
+from .. import unit as tools_unit
 
 
 @dataclass
 class Category:
     """Class to store characteristics of a category on a categorical datetime axis."""
 
     x: int
@@ -31,24 +31,24 @@
         while len(categories) > max_count:
             prio = max(cat.prio for cat in categories)
             categories = [cat for cat in categories if cat.prio < prio]
         return categories
 
     def _get_subset(self, attr: str, max_count: int = None) -> Iterable:
         values = [getattr(cat, attr) for cat in self.categories(max_count)]
-        if not isinstance(values[0], tools.unit.Q_):
+        if not isinstance(values[0], tools_unit.Q_):
             return np.array(values)
         unit = values[0].units
         magnitudes = [value.to(unit).m for value in values]
-        return tools.unit.PA_(magnitudes, unit)
+        return tools_unit.PA_(magnitudes, unit)
 
     def x(self, max_count: int = None) -> Iterable[int]:
         return self._get_subset("x", max_count)
 
-    def y(self, max_count: int = None) -> Iterable[Union[float, tools.unit.Q_]]:
+    def y(self, max_count: int = None) -> Iterable[float | tools_unit.Q_]:
         return self._get_subset("y", max_count)
 
     def ts(self, max_count: int = None) -> Iterable[pd.Timestamp]:
         return self._get_subset("ts", max_count)
 
     def labels(self, max_count: int = None) -> Iterable[str]:
         return self._get_subset("label", max_count)
```

### Comparing `portfolyo-0.5.8/portfolyo/visualize/colors.py` & `portfolyo-0.6.0/portfolyo/tools/visualize/colors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Creating colors for use in plotting."""
 
 import colorsys
 from collections import namedtuple
+from enum import Enum
 
 import matplotlib as mpl
 import numpy as np
 
 
 class Color(namedtuple("RGB", ["r", "g", "b"])):
     """Class to create an rgb color tuple, with additional methods."""
@@ -14,33 +15,35 @@
         """Lighten the color by fraction ``value`` (between 0 and 1). If < 0, darken."""
         hu, li, sa = np.array(colorsys.rgb_to_hls(*mpl.colors.to_rgb(self)))
         li += value * ((1 - li) if value > 0 else li)
         return Color(*[min(max(p, 0), 1) for p in colorsys.hls_to_rgb(hu, li, sa)])
 
     def darken(self, value):
         """Darken the color by fraction ``value`` (between 0 and 1)."""
-        return self.lighten(self, -value)
+        return self.lighten(-value)
 
     light = property(lambda self: self.lighten(0.3))
     xlight = property(lambda self: self.lighten(0.6))
     dark = property(lambda self: self.lighten(-0.3))
     xdark = property(lambda self: self.lighten(-0.6))
 
 
 class Colors:
-    class General:
-        PURPLE = Color(0.549, 0.110, 0.706)
-        GREEN = Color(0.188, 0.463, 0.165)
-        BLUE = Color(0.125, 0.247, 0.600)
-        ORANGE = Color(0.961, 0.533, 0.114)
-        RED = Color(0.820, 0.098, 0.114)
-        YELLOW = Color(0.945, 0.855, 0.090)
-        LBLUE = Color(0.067, 0.580, 0.812)
-        LGREEN = Color(0.325, 0.773, 0.082)
-        BLACK = Color(0, 0, 0)
-        WHITE = Color(1, 1, 1)
+    class General(Enum):
+        DARK_BURGUNDY = Color(0.2667, 0.0000, 0.0745)
+        BROWN_SUGAR = Color(0.3765, 0.2902, 0.1804)
+        DUSTY_GRAY = Color(0.5529, 0.5176, 0.3765)
+        MOONSTONE = Color(0.7647, 0.7569, 0.6118)
+        CORAL = Color(0.9608, 0.3412, 0.4980)
+        ORANGE = Color(0.9608, 0.5098, 0.1140)
+        RED = Color(0.8196, 0.0980, 0.1137)
+        YELLOW = Color(0.9451, 0.8549, 0.0902)
+        LBLUE = Color(0.0667, 0.5804, 0.8118)
+        LGREEN = Color(0.3255, 0.7725, 0.0824)
+        BLACK = Color(0.0000, 0.0000, 0.0000)
+        WHITE = Color(1.0000, 1.0000, 1.0000)
 
     class Wqpr:  # Standard colors when plotting a portfolio
         w = Color(*mpl.colors.to_rgb("#0E524F")).lighten(0.15)
         q = Color(*mpl.colors.to_rgb("#0E524F"))
         r = Color(*mpl.colors.to_rgb("#8B7557"))
-        p = Color(*mpl.colors.to_rgb("#E53454"))
+        p = Color(*mpl.colors.to_rgb("#cd3759"))
```

### Comparing `portfolyo-0.5.8/portfolyo/visualize/plot.py` & `portfolyo-0.6.0/portfolyo/tools/visualize/plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Visualize portfolio lines, etc.
 """
 
+from typing import Callable
+
 import matplotlib as mpl
-import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
-from .. import tools
-from .categories import Categories, Category  # noqa
+from .. import freq as tools_freq
+from .. import unit as tools_unit
+from .categories import Categories
+from .colors import Colors
 
 mpl.style.use("seaborn-v0_8")
 
 # Plotting philosophy for timeseries:
 # Not all plot types (bar, line, step, etc.) are suitable for all quantities.
 #
 # Data dimensionality vs plot type
@@ -48,217 +51,169 @@
 #
 #
 # This module is able to plot all graph types on both timeline x-axis and on categorical
 # x-axis, and add the data labels if there are not too many. It is up to the caller to
 # pick the correct graph type.
 #
 
-MAX_XLABELS = 20
+MAX_XLABELS = 15
+
+
+class ContinuousValuesNotSupported(Exception):
+    pass
+
 
+class CategoricalValuesNotSupported(Exception):
+    pass
 
-def use_categories(ax: plt.Axes, s: pd.Series, cat: bool = None) -> bool:
-    """Determine if plot should be made with category axis (True) or datetime axis (False)."""
-    # We use categorical data if...
-    if (ax.lines or ax.collections or ax.containers) and ax.xaxis.have_units():
-        return True  # ...ax already has category axis; or
-    elif cat is None and tools.freq.shortest(s.index.freq, "MS") == "MS":
-        return True  # ...it's the default for the given frequency; or
-    elif cat is True:
-        return True  # ...user wants it.
-    return False
 
+PlotTimeseriesToAxFunction = Callable[[plt.Axes, pd.Series, ...], None]
 
 docstringliteral_plotparameters = """
 Other parameters
 ----------------
 labelfmt : str, optional (default: '')
     Labels are added to each datapoint in the specified format. ('' to add no labels)
-cat : bool, optional
-    If False, plots x-axis as timeline with timestamps spaced according to their
-    duration. If True, plots x-axis categorically, with timestamps spaced equally.
-    Disregarded if ``ax`` already has values (then: use whatever is already set).
-    Default: use True if ``s`` has a monthly frequency or longer, False if the frequency
-    is shorter than monthly.
 **kwargs : any formatting are passed to the Axes plot method being used."""
 
 
 def append_to_doc(text):
     def decorator(fn):
         fn.__doc__ += f"\n{text}"
         return fn
 
     return decorator
 
 
 @append_to_doc(docstringliteral_plotparameters)
-def plot_timeseries_as_jagged(
-    ax: plt.Axes, s: pd.Series, labelfmt: str = "", cat: bool = None, **kwargs
-) -> None:
-    """Plot timeseries ``s`` to axis ``ax``, as jagged line and/or as markers. Use kwargs
-    ``linestyle`` and ``marker`` to specify line style and/or marker style. (Default: line only).
-    """
-    s = prepare_ax_and_s(ax, s)  # ensure unit compatibility (if possible)
-
-    if use_categories(ax, s, cat):
-        categories = Categories(s)
-        ax.plot(categories.x(), categories.y(), **kwargs)
-        ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
-        set_data_labels(ax, categories.x(), categories.y(), labelfmt, False)
-
-    else:
-        ax.plot(s.index, s.values, **kwargs)
-        set_data_labels(ax, s.index, s.values, labelfmt, False)
-
-
-@append_to_doc(docstringliteral_plotparameters)
 def plot_timeseries_as_bar(
-    ax: plt.Axes, s: pd.Series, labelfmt: str = "", cat: bool = None, **kwargs
+    ax: plt.Axes,
+    s: pd.Series,
+    labelfmt: str = "",
+    width: float = 0.8,
+    **kwargs,
 ) -> None:
-    """Plot timeseries ``s`` to axis ``ax``, as bars. Ideally, only used for plots with
-    categorical (i.e, non-time) x-axis."""
+    """Plot timeseries ``s`` to axis ``ax``, as bars.
+    On plots with categorical (i.e, non-continuous) time axis."""
+    if not is_categorical(s):
+        raise ContinuousValuesNotSupported(
+            "This plot is not compatible with continous values"
+        )
+    check_ax_s_compatible(ax, s)
     s = prepare_ax_and_s(ax, s)  # ensure unit compatibility (if possible)
 
-    if use_categories(ax, s, cat):
-        categories = Categories(s)
-        ax.bar(categories.x(), categories.y(), 0.8, **kwargs)
-        ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
-        set_data_labels(ax, categories.x(), categories.y(), labelfmt, True)
-
-    else:
-        # Bad combination: bar graph on time-axis. But allow anyway.
-
-        # This is slow if there are many elements.
-        # x = s.index + 0.5 * (s.index.right - s.index)
-        # width = pd.Timedelta(hours=s.index.duration.median().to("h").magnitude * 0.8)
-        # ax.bar(x.values, s.values, width, **kwargs)
-
-        # This is faster.
-        delta = s.index.right - s.index
-        x = np.array(list(zip(s.index + 0.1 * delta, s.index + 0.9 * delta))).flatten()
-        magnitudes = np.array([[v, 0] for v in s.values.quantity.magnitude]).flatten()
-        values = tools.unit.PA_(magnitudes, s.values.quantity.units)
-        ax.fill_between(x, 0, values, step="post", **kwargs)
-
-        set_data_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, True)
+    categories = Categories(s)
+    ax.bar(categories.x(), categories.y(), width=width, **kwargs)
+    ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
+    set_data_labels(
+        ax, categories.x(MAX_XLABELS), categories.y(MAX_XLABELS), labelfmt, True
+    )
+    ax.autoscale()
 
 
 @append_to_doc(docstringliteral_plotparameters)
 def plot_timeseries_as_area(
-    ax: plt.Axes, s: pd.Series, labelfmt: str = "", cat: bool = None, **kwargs
+    ax: plt.Axes,
+    s: pd.Series,
+    labelfmt: str = "",
+    **kwargs,
 ) -> None:
-    """Plot timeseries ``s`` to axis ``ax``, as stepped area between 0 and value. Ideally,
-    only used for plots with time (i.e., non-categorical) axis."""
+    """Plot timeseries ``s`` to axis ``ax``, as stepped area between 0 and value.
+    On plots with continuous (i.e., non-categorical) time axis."""
+    if is_categorical(s):
+        raise CategoricalValuesNotSupported(
+            "This plot is not compatible with categorical values"
+        )
+    check_ax_s_compatible(ax, s)
     s = prepare_ax_and_s(ax, s)  # ensure unit compatibility (if possible)
 
     splot = s.copy()  # modified with additional (repeated) datapoint
     splot[splot.index.right[-1]] = splot.values[-1]
 
-    if use_categories(ax, s, cat):
-        # Bad combination: area graph on categorical axis. But allow anyway.
-
-        categories = Categories(s)
-        ctgr_extra = Categories(splot)
-        # Center around x-tick:
-        ax.fill_between(ctgr_extra.x() - 0.5, 0, ctgr_extra.y(), step="post", **kwargs)
-        ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
-        set_data_labels(ax, categories.x(), categories.y(), labelfmt, True)
-
-    else:
-        ax.fill_between(splot.index, 0, splot.values, step="post", **kwargs)
-        delta = s.index.right - s.index
-        set_data_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, True)
+    bottom = [0.0 for i in range(0, splot.size)]
+    # make bottom into pintarray
+    bottom = bottom * splot.values[0].units
+
+    ax.fill_between(
+        splot.index,
+        bottom,
+        [sum(x) for x in zip(bottom, splot.values)],
+        step="post",
+        **kwargs,
+    )
+    delta = s.index.right - s.index
+    set_data_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, True)
+    ax.autoscale()
 
 
 @append_to_doc(docstringliteral_plotparameters)
 def plot_timeseries_as_step(
-    ax: plt.Axes, s: pd.Series, labelfmt: str = "", cat: bool = None, **kwargs
+    ax: plt.Axes, s: pd.Series, labelfmt: str = "", **kwargs
 ) -> None:
     """Plot timeseries ``s`` to axis ``ax``, as stepped line (horizontal and vertical lines).
-    Ideally, only used for plots with time (i.e., non-categorical) axis."""
+    On plots with continuous (i.e., non-categorical) time axis."""
+    if is_categorical(s):
+        raise CategoricalValuesNotSupported(
+            "This plot is not compatible with categorical values"
+        )
+    check_ax_s_compatible(ax, s)
     s = prepare_ax_and_s(ax, s)  # ensure unit compatibility (if possible)
 
     splot = s.copy()  # modified with additional (repeated) datapoint
     splot[splot.index.right[-1]] = splot.values[-1]
 
-    if use_categories(ax, s, cat):
-        # Bad combination: step graph on categorical axis. But allow anyway.
-
-        categories = Categories(s)
-        ctgr_extra = Categories(splot)
-        # Center around x-tick:
-        ax.step(ctgr_extra.x() - 0.5, ctgr_extra.y(), where="post", **kwargs)
-        ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
-        set_data_labels(ax, categories.x(), categories.y(), labelfmt, True)
-
-    else:
-        ax.step(splot.index, splot.values, where="post", **kwargs)
-        delta = s.index.right - s.index
-        set_data_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, True)
+    ax.step(splot.index, splot.values, where="mid", **kwargs)
+    delta = s.index.right - s.index
+    set_data_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, True)
+    ax.autoscale()
 
 
 @append_to_doc(docstringliteral_plotparameters)
 def plot_timeseries_as_hline(
-    ax: plt.Axes, s: pd.Series, labelfmt: str = "", cat: bool = None, **kwargs
+    ax: plt.Axes, s: pd.Series, labelfmt: str = "", **kwargs
 ) -> None:
-    """Plot timeseries ``s`` to axis ``ax``, as horizontal lines. Ideally, only used for
-    plots with time (i.e., non-categorical) axis."""
+    """Plot timeseries ``s`` to axis ``ax``, as horizontal lines.
+    On plots with categorical (i.e., non-continuous) time axis."""
+    if not is_categorical(s):
+        raise ContinuousValuesNotSupported(
+            "This plot is not compatible with continous time axis"
+        )
+    check_ax_s_compatible(ax, s)
     s = prepare_ax_and_s(ax, s)  # ensure unit compatibility (if possible)
+    categories = Categories(s)
+    # Center around x-tick:
+    ax.hlines(categories.y(), categories.x() - 0.4, categories.x() + 0.4, **kwargs)
+    ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
+    set_data_labels(ax, categories.x(), categories.y(), labelfmt, True)
+    ax.autoscale()
+    # Adjust the margins around the plot
+    ax.margins(x=0.2, y=0.2)
 
-    if use_categories(ax, s, cat):
-        # Bad combination: hline graph on categorical axis. But allow anyway.
 
-        categories = Categories(s)
-        # Center around x-tick:
-        ax.hlines(categories.y(), categories.x() - 0.5, categories.x() + 0.5, **kwargs)
-        ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
-        set_data_labels(ax, categories.x(), categories.y(), labelfmt, True)
+def set_portfolyo_attr(ax, name, val):
+    """
+    Sets attribute ax._portfolyo which is a dictionary: ._portfolyo = {'unit': ..., 'freq': ..., ...}
+    If dictionary doesn't exist yet, creates an empty dictionary
+    """
+    pattr = getattr(ax, "_portfolyo", {})
+    pattr[name] = val
+    setattr(ax, "_portfolyo", pattr)
 
-    else:
-        delta = s.index.right - s.index
-        ax.hlines(s.values, s.index, s.index.right, **kwargs)
-        set_data_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, False)
 
+def get_portfolyo_attr(ax, name, default_val=None):
+    """
+    Gets values from dictionary ax._portfolyo, if it doesn't exist returns None.
+    """
+    pattr = getattr(ax, "_portfolyo", {})
+    return pattr.get(name, default_val)
 
-def plot_timeseries(
-    ax: plt.Axes,
-    s: pd.Series,
-    how: str = "jagged",
-    labelfmt: str = None,
-    cat: bool = None,
-    **kwargs,
-) -> None:
-    """Plot timeseries to given axis.
 
-    Parameters
-    ----------
-    ax : plt.Axes
-        Axes to plot to.
-    s : pd.Series
-        Timeseries to plot
-    how : str, optional (default: 'jagged')
-        How to plot the data; one of {'jagged', 'bar', 'area', 'step', 'hline'}.
-    labelfmt : str, optional (default: '')
-        Labels are added to each datapoint in the specified format. ('' to add no labels)
-    cat : bool, optional (default: True if frequency is monthly or larger)
-        Plot as categorical x-axis.
-    """
-    if how == "jagged":
-        plot_timeseries_as_jagged(ax, s, labelfmt, cat, **kwargs)
-    elif how == "bar":
-        plot_timeseries_as_bar(ax, s, labelfmt, cat, **kwargs)
-    elif how == "area":
-        plot_timeseries_as_area(ax, s, labelfmt, cat, **kwargs)
-    elif how == "step":
-        plot_timeseries_as_step(ax, s, labelfmt, cat, **kwargs)
-    elif how == "hline":
-        plot_timeseries_as_hline(ax, s, labelfmt, cat, **kwargs)
-    else:
-        raise ValueError(
-            f"Parameter ``how`` must be one of 'jagged', 'bar', 'area', 'step', 'hline'; got {how}."
-        )
+def is_categorical(s: pd.Series) -> bool:
+    """The function checks whether frequency of panda Series falls into continous or categorical group"""
+    return tools_freq.up_or_down(s.index.freq, "D") == 1
 
 
 def prepare_ax_and_s(ax: plt.Axes, s: pd.Series, unit=None) -> pd.Series:
     """Ensure axes ``ax`` has unit associated with it and checks compatibility with series
     ``s``. Also sets y label as unit abbreviation.
 
     Notes
@@ -271,42 +226,74 @@
     when calling this function for the first time for a given ``ax``. Ignored on subsequent
     calls and a unit is already associated with the axes.
     """
     # Make sure series has pint unit.
     if s.dtype == float or s.dtype == int:
         s = s.astype("pint[1]")
     # Find preexisting unit.
-    axunit = getattr(ax, "_unit", None)
+    axunit = get_portfolyo_attr(ax, "unit", None)
 
     # Axes already has unit. Convert series to that unit; ignore any supplied custom unit.
     if axunit is not None:
         if axunit.dimensionality != s.pint.dimensionality:  # check compatibilty
             raise ValueError(
                 f"Cannot plot series with units {s.pint.units} on axes with units {axunit}."
             )
-        return s.astype(axunit)
+        return s.astype(f"pint[{axunit}]")
 
     # Axes does not have unit.
     if unit is not None:
         # Custom unit is provided. Convert series to that unit.
         if unit.dimensionality != s.pint.dimensionality:  # check compatibility
             raise ValueError(
                 f"Cannot convert series with units {s.pint.units} to units {unit}."
             )
         s = s.astype(unit)
-        setattr(ax, "_unit", unit)
+        set_portfolyo_attr(ax, "unit", unit)
     else:
         # No custom unit provided. Convert series to base units.
         s = s.pint.to_base_units()
-        setattr(ax, "_unit", s.pint.units)
-
-    ax.set_ylabel(f"{ax._unit:~P}")
+        set_portfolyo_attr(ax, "unit", s.pint.units)
+    # Get unit attribute
+    unit = get_portfolyo_attr(ax, "unit")
+    name_unit = tools_unit.to_name(unit)
+    # Define color mapping based on 'Wqpr' class attributes
+    unit_colors = {
+        "w": Colors.Wqpr.w,
+        "q": Colors.Wqpr.q,
+        "r": Colors.Wqpr.r,
+        "p": Colors.Wqpr.p,
+    }
+    # Set default color if name_unit not found
+    default_color = "white"
+    # Get background color based on name_unit
+    background_color = unit_colors.get(name_unit, default_color)
+    ax.set_ylabel(f"{unit:~P}", backgroundcolor=background_color.lighten(0.3))
     return s
 
 
+def check_ax_s_compatible(ax: plt.Axes, s: pd.Series):
+    """Ensure axes ``ax`` has frequency associated with it and checks compatibility with series
+    ``s``.
+    If axes `ax`` has frequency, compare to pd.Series frequency. If they are equal, return s, if not equal, return error.
+    If axes `ax`` doesn't have frequency, assign frequency of s to it.
+    """
+    # Find preexisting frequency.
+    axfreq = get_portfolyo_attr(ax, "freq", None)
+    series_freq = s.index.freq
+    # Axes does not have frequency.
+    if axfreq is None:
+        set_portfolyo_attr(ax, "freq", series_freq)
+    else:
+        if get_portfolyo_attr(ax, "freq") != series_freq:
+            raise AttributeError(
+                "The frequency of PFLine is not compatible with current axes"
+            )
+
+
 def set_data_labels(
     ax: plt.Axes, xx, yy, labelfmt, outside: bool = False, maxcount: int = 24
 ):
     """Add labels to axis ``ax``, at locations (``xx``, ``yy``), formatted with
     ``labelfmt``. Don't add labels if more than ``maxcount`` datapoints. If ``outside``,
     put labels of negative values *below* the datapoint."""
     # Don't label if no formatting speficied.
@@ -316,16 +303,22 @@
     if len(xx) > maxcount:
         return
 
     # Add labels.
     for x, y in zip(xx, yy):
         lbl = labelfmt.format(y.magnitude).replace(",", " ")
         xytext = (0, -10) if outside and y.magnitude < 0 else (0, 10)
-        ax.annotate(lbl, (x, y), textcoords="offset points", xytext=xytext, ha="center")
+        ax.annotate(
+            lbl,
+            (x, y),
+            textcoords="offset points",
+            xytext=xytext,
+            ha="center",
+            va="top" if y.magnitude < 0 else "bottom",
+            rotation=90,
+        )
 
     # Increase axis range to give label space to stay inside box.
-    ylim = list(ax.get_ylim())
-    if not np.isclose(ylim[0], 0) and ylim[0] < 0:
-        ylim[0] *= 1.1
-    if not np.isclose(ylim[1], 0) and ylim[1] > 0:
-        ylim[1] *= 1.1
-    ax.set_ylim(*ylim)
+    miny, maxy = ax.get_ylim()
+    delta = 0.5
+    miny2, maxy2 = (1 + delta) * miny - delta * maxy, (1 + delta) * maxy - delta * miny
+    ax.set_ylim(miny2, maxy2)
```

### Comparing `portfolyo-0.5.8/pyproject.toml` & `portfolyo-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "portfolyo"
-version = "0.5.8"
+version = "0.6.0"
 description = "Analyse and manipulate timeseries related to power and gas offtake portfolios"
 authors = [
     "Ruud Wijtvliet <rwijtvliet@gmail.com>",
     "Sakshi Singh <sakshisingh1809@gmail.com>",
+    "Alina Voilova <voilova.alina@gmail.com>",
 ]
 license = "BSD-3"
 readme = "README.rst"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 pandas = "~2.0"       # pandas 2.1.0 doesn't play nice with pint-pandas. Update when new pint-pandas version is released (>0.5) 
 matplotlib = "^3.7.2"
 pint = "0.19.2"
 pint-pandas = "0.4"
 colorama = "^0.4.6"
 holidays = "^0.32"
 numpy = "^1.26.2"
@@ -31,19 +32,21 @@
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.2.6"
 sphinx-autobuild = "^2021.3.14"
 matplotlib = "^3.8.2"
 numpydoc = "^1.6.0"
 sphinx-copybutton = "^0.5.2"
-sphinx-exec-code = "^0.10"
+sphinx-exec-code = "^0.12"
 sphinx-rtd-theme = "^1.3.0"
 insegel = "^1.3.1"
 nbsphinx = "^0.9.3"
 pandoc = "^2.3"
+pip-tools = "^7.4.1"
+IPython = "^8.23.0"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.1.0"
 black = "^23.7.0"
 pre-commit = "^3.4.0"
 ipykernel = "^6.25.2"
```

### Comparing `portfolyo-0.5.8/PKG-INFO` & `portfolyo-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: portfolyo
-Version: 0.5.8
+Version: 0.6.0
 Summary: Analyse and manipulate timeseries related to power and gas offtake portfolios
 License: BSD-3
 Author: Ruud Wijtvliet
 Author-email: rwijtvliet@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: holidays (>=0.32,<0.33)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: pandas (>=2.0,<2.1)
 Requires-Dist: pint (==0.19.2)
 Requires-Dist: pint-pandas (==0.4)
 Description-Content-Type: text/x-rst
 
+=========
 portfolyo
 =========
 
 .. image:: https://img.shields.io/pypi/v/portfolyo
    :target: https://pypi.org/project/portfolyo
    :alt: Pypi
 
@@ -47,14 +47,16 @@
 .. image:: https://readthedocs.org/projects/portfolyo/badge/?version=latest
     :target: https://portfolyo.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 Portfolyo is a Python package to analyse and manipulate timeseries related to power 
 and gas offtake portfolios.
 
+
+------------
 Installation
 ------------
 
 .. code-block:: bash
 
    pip install portfolyo
 
@@ -64,43 +66,57 @@
 
    pip install portfolyo==x.y.z
 
    # or, in pyproject.toml
    portfolyo = "x.y.z"
 
 
+-------------
 Documentation
 -------------
 
 Documentation is hosted on readthedocs:
 
 https://portfolyo.readthedocs.io/
 
+
+----------
 Repository
 ----------
 
 The git repository is hosted on github:
 
 http://www.github.com/rwijtvliet/portfolyo
 
 
+----------
 Developing
 ----------
 
 This project uses ``black`` to format code and ``flake8`` for linting. We also support ``pre-commit`` to ensure
 these have been run. To configure your local environment please install these development dependencies and set up
 the commit hooks.
 
 .. code-block:: bash
 
    poetry install --with dev,test
    pre-commit install
 
 Feature branches are merged into the ``develop`` branch via pull request.
 
+
+Internal dependencies
+---------------------
+
+Inside the package, modules depend on each other in the following chain. A module may depend on another module if it is further to the left:
+
+tools >> pfline >> pfstate >> tools2
+
+
+----------
 Publishing
 ----------
 
 To publish a new release from ``develop``, create a new branch, increment the version number and push to github. For convenience, there is a ``create_release_branch.sh`` script that accomplishes the same, which takes one argument:
 
 .. code-block:: bash
```

