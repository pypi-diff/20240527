# Comparing `tmp/lensmc-24.5.1.tar.gz` & `tmp/lensmc-24.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lensmc-24.5.1.tar", last modified: Thu May 23 13:34:52 2024, max compression
+gzip compressed data, was "lensmc-24.5.2.tar", last modified: Mon May 27 13:14:22 2024, max compression
```

## Comparing `lensmc-24.5.1.tar` & `lensmc-24.5.2.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:34:52.503369 lensmc-24.5.1/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2024-05-23 13:33:17.000000 lensmc-24.5.1/COPYING
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-23 13:33:17.000000 lensmc-24.5.1/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-23 13:33:17.000000 lensmc-24.5.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-23 13:33:17.000000 lensmc-24.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1571 2024-05-23 13:34:52.503369 lensmc-24.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1964 2024-05-23 13:33:17.000000 lensmc-24.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:34:52.477370 lensmc-24.5.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      611 2024-05-23 13:33:17.000000 lensmc-24.5.1/docs/description.md
--rw-rw-rw-   0 root         (0) root         (0)      431 2024-05-23 13:33:17.000000 lensmc-24.5.1/environment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:34:52.481370 lensmc-24.5.1/lensmc/
--rw-r--r--   0 root         (0) root         (0)      331 2024-05-23 13:34:20.000000 lensmc-24.5.1/lensmc/INFO
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:34:52.494370 lensmc-24.5.1/lensmc/aux/
--rw-rw-rw-   0 root         (0) root         (0)  2133226 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/aux/cache_1x.bin
--rw-rw-rw-   0 root         (0) root         (0)  2133226 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/aux/cache_3x.bin
--rw-rw-rw-   0 root         (0) root         (0)  2133226 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/aux/cache_5x.bin
--rw-rw-rw-   0 root         (0) root         (0)  1312854 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/aux/cache_7x.bin
--rw-rw-rw-   0 root         (0) root         (0)     5799 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/aux/se++.config
--rw-rw-rw-   0 root         (0) root         (0)     3762 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/aux/se.config
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/aux/se.param
--rw-rw-rw-   0 root         (0) root         (0)     1244 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/aux/seg_filter.conv
--rw-rw-rw-   0 root         (0) root         (0)     7160 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/aux/swarp.config
--rw-rw-rw-   0 root         (0) root         (0)    23540 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/catalogue.py
--rw-rw-rw-   0 root         (0) root         (0)     1493 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/flags.py
--rw-rw-rw-   0 root         (0) root         (0)    54825 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/image.py
--rw-rw-rw-   0 root         (0) root         (0)    13450 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/likelihood.py
--rw-rw-rw-   0 root         (0) root         (0)    46023 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/measure_shear.py
--rw-rw-rw-   0 root         (0) root         (0)    12389 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/measure_shear_all.py
--rw-rw-rw-   0 root         (0) root         (0)     7808 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/models.py
--rw-rw-rw-   0 root         (0) root         (0)    20771 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/optimise.py
--rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/prior.py
--rw-rw-rw-   0 root         (0) root         (0)     6692 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/psf.py
--rw-rw-rw-   0 root         (0) root         (0)    12086 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/segmentation.py
--rw-rw-rw-   0 root         (0) root         (0)    15293 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/shear_bias.py
--rw-rw-rw-   0 root         (0) root         (0)    22676 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/shear_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:34:52.475370 lensmc-24.5.1/lensmc/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:34:52.494370 lensmc-24.5.1/lensmc/src/c/
--rw-rw-rw-   0 root         (0) root         (0)    18370 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/src/c/fast_fourier_model.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1114 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/src/c/fast_fourier_model.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:34:52.501369 lensmc-24.5.1/lensmc/src/cython/
--rw-r--r--   0 root         (0) root         (0)  1117108 2024-05-23 13:34:50.000000 lensmc-24.5.1/lensmc/src/cython/cross_product.c
--rw-rw-rw-   0 root         (0) root         (0)     2048 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/src/cython/cross_product.pyx
--rw-r--r--   0 root         (0) root         (0)  1067772 2024-05-23 13:34:50.000000 lensmc-24.5.1/lensmc/src/cython/galaxy_model.cpp
--rw-rw-rw-   0 root         (0) root         (0)      772 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/src/cython/galaxy_model.pxd
--rw-rw-rw-   0 root         (0) root         (0)    16958 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/src/cython/galaxy_model.pyx
--rw-r--r--   0 root         (0) root         (0)  1190020 2024-05-23 13:34:51.000000 lensmc-24.5.1/lensmc/src/cython/linear_fit.c
--rw-rw-rw-   0 root         (0) root         (0)     5668 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/src/cython/linear_fit.pyx
--rw-r--r--   0 root         (0) root         (0)   466044 2024-05-23 13:34:51.000000 lensmc-24.5.1/lensmc/src/cython/star_model.cpp
--rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/src/cython/star_model.pxd
--rw-rw-rw-   0 root         (0) root         (0)     2586 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/src/cython/star_model.pyx
--rw-rw-rw-   0 root         (0) root         (0)     3206 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:34:52.502369 lensmc-24.5.1/lensmc/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1261 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/tests/test_background.py
--rw-rw-rw-   0 root         (0) root         (0)     3116 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/tests/test_galaxy_runtime.py
--rw-rw-rw-   0 root         (0) root         (0)     8751 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/tests/test_measure_shear.py
--rw-rw-rw-   0 root         (0) root         (0)     4633 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/tests/test_measure_shear_all.py
--rw-rw-rw-   0 root         (0) root         (0)     6103 2024-05-23 13:33:17.000000 lensmc-24.5.1/lensmc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:34:52.503369 lensmc-24.5.1/lensmc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1571 2024-05-23 13:34:52.000000 lensmc-24.5.1/lensmc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1415 2024-05-23 13:34:52.000000 lensmc-24.5.1/lensmc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 13:34:52.000000 lensmc-24.5.1/lensmc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 13:34:22.000000 lensmc-24.5.1/lensmc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-23 13:34:52.000000 lensmc-24.5.1/lensmc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-23 13:34:52.000000 lensmc-24.5.1/lensmc.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-05-23 13:33:17.000000 lensmc-24.5.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-05-23 13:33:17.000000 lensmc-24.5.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 13:34:52.504369 lensmc-24.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5822 2024-05-23 13:33:17.000000 lensmc-24.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:14:22.656424 lensmc-24.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2024-05-27 13:12:52.000000 lensmc-24.5.2/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-27 13:12:52.000000 lensmc-24.5.2/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-27 13:12:52.000000 lensmc-24.5.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-27 13:12:52.000000 lensmc-24.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-05-27 13:14:22.655424 lensmc-24.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2024-05-27 13:12:52.000000 lensmc-24.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:14:22.631424 lensmc-24.5.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      611 2024-05-27 13:12:52.000000 lensmc-24.5.2/docs/description.md
+-rw-rw-rw-   0 root         (0) root         (0)      431 2024-05-27 13:12:52.000000 lensmc-24.5.2/environment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:14:22.634424 lensmc-24.5.2/lensmc/
+-rw-r--r--   0 root         (0) root         (0)      331 2024-05-27 13:13:52.000000 lensmc-24.5.2/lensmc/INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:14:22.646424 lensmc-24.5.2/lensmc/aux/
+-rw-rw-rw-   0 root         (0) root         (0)  2133226 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/aux/cache_1x.bin
+-rw-rw-rw-   0 root         (0) root         (0)  2133226 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/aux/cache_3x.bin
+-rw-rw-rw-   0 root         (0) root         (0)  2133226 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/aux/cache_5x.bin
+-rw-rw-rw-   0 root         (0) root         (0)  1312854 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/aux/cache_7x.bin
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/aux/se++.config
+-rw-rw-rw-   0 root         (0) root         (0)     3762 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/aux/se.config
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/aux/se.param
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/aux/seg_filter.conv
+-rw-rw-rw-   0 root         (0) root         (0)     7160 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/aux/swarp.config
+-rw-rw-rw-   0 root         (0) root         (0)     1493 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)    54841 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/image.py
+-rw-rw-rw-   0 root         (0) root         (0)    13450 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/likelihood.py
+-rw-rw-rw-   0 root         (0) root         (0)    46321 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/measure_shear.py
+-rw-rw-rw-   0 root         (0) root         (0)    12389 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/measure_shear_all.py
+-rw-rw-rw-   0 root         (0) root         (0)     7808 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    20771 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/optimise.py
+-rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/prior.py
+-rw-rw-rw-   0 root         (0) root         (0)     6692 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/psf.py
+-rw-rw-rw-   0 root         (0) root         (0)    12086 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/segmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)    15293 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/shear_bias.py
+-rw-rw-rw-   0 root         (0) root         (0)    22676 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/shear_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:14:22.628424 lensmc-24.5.2/lensmc/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:14:22.647424 lensmc-24.5.2/lensmc/src/c/
+-rw-rw-rw-   0 root         (0) root         (0)    18370 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/src/c/fast_fourier_model.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/src/c/fast_fourier_model.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:14:22.654424 lensmc-24.5.2/lensmc/src/cython/
+-rw-r--r--   0 root         (0) root         (0)  1117108 2024-05-27 13:14:20.000000 lensmc-24.5.2/lensmc/src/cython/cross_product.c
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/src/cython/cross_product.pyx
+-rw-r--r--   0 root         (0) root         (0)  1067772 2024-05-27 13:14:21.000000 lensmc-24.5.2/lensmc/src/cython/galaxy_model.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      772 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/src/cython/galaxy_model.pxd
+-rw-rw-rw-   0 root         (0) root         (0)    16958 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/src/cython/galaxy_model.pyx
+-rw-r--r--   0 root         (0) root         (0)  1190020 2024-05-27 13:14:21.000000 lensmc-24.5.2/lensmc/src/cython/linear_fit.c
+-rw-rw-rw-   0 root         (0) root         (0)     5668 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/src/cython/linear_fit.pyx
+-rw-r--r--   0 root         (0) root         (0)   466044 2024-05-27 13:14:21.000000 lensmc-24.5.2/lensmc/src/cython/star_model.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/src/cython/star_model.pxd
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/src/cython/star_model.pyx
+-rw-rw-rw-   0 root         (0) root         (0)     3206 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:14:22.655424 lensmc-24.5.2/lensmc/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/tests/test_background.py
+-rw-rw-rw-   0 root         (0) root         (0)     3116 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/tests/test_galaxy_runtime.py
+-rw-rw-rw-   0 root         (0) root         (0)     8751 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/tests/test_measure_shear.py
+-rw-rw-rw-   0 root         (0) root         (0)     4633 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/tests/test_measure_shear_all.py
+-rw-rw-rw-   0 root         (0) root         (0)     6103 2024-05-27 13:12:52.000000 lensmc-24.5.2/lensmc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:14:22.655424 lensmc-24.5.2/lensmc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-05-27 13:14:22.000000 lensmc-24.5.2/lensmc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1395 2024-05-27 13:14:22.000000 lensmc-24.5.2/lensmc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 13:14:22.000000 lensmc-24.5.2/lensmc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 13:13:55.000000 lensmc-24.5.2/lensmc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-27 13:14:22.000000 lensmc-24.5.2/lensmc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-27 13:14:22.000000 lensmc-24.5.2/lensmc.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-05-27 13:12:52.000000 lensmc-24.5.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-05-27 13:12:52.000000 lensmc-24.5.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 13:14:22.656424 lensmc-24.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5822 2024-05-27 13:12:52.000000 lensmc-24.5.2/setup.py
```

### Comparing `lensmc-24.5.1/COPYING` & `lensmc-24.5.2/COPYING`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/COPYING.LESSER` & `lensmc-24.5.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/LICENSE` & `lensmc-24.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/PKG-INFO` & `lensmc-24.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lensmc
-Version: 24.5.1
+Version: 24.5.2
 Summary: Python package for weak lensing shear measurements
 Home-page: https://gitlab.com/gcongedo/LensMC
 Author: Giuseppe Congedo
 Author-email: giuseppe.congedo@ed.ac.uk
 License: LGPL - Copyright (C) 2015 Giuseppe Congedo, University of Edinburgh on behalf of the Euclid Science Ground Segment
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lensmc-24.5.1/README.md` & `lensmc-24.5.2/README.md`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/docs/description.md` & `lensmc-24.5.2/docs/description.md`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/__init__.py` & `lensmc-24.5.2/lensmc/__init__.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/aux/cache_1x.bin` & `lensmc-24.5.2/lensmc/aux/cache_1x.bin`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/aux/cache_3x.bin` & `lensmc-24.5.2/lensmc/aux/cache_3x.bin`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/aux/cache_5x.bin` & `lensmc-24.5.2/lensmc/aux/cache_5x.bin`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/aux/cache_7x.bin` & `lensmc-24.5.2/lensmc/aux/cache_7x.bin`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/aux/se++.config` & `lensmc-24.5.2/lensmc/aux/se++.config`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/aux/se.config` & `lensmc-24.5.2/lensmc/aux/se.config`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/aux/seg_filter.conv` & `lensmc-24.5.2/lensmc/aux/seg_filter.conv`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/aux/swarp.config` & `lensmc-24.5.2/lensmc/aux/swarp.config`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/flags.py` & `lensmc-24.5.2/lensmc/flags.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/image.py` & `lensmc-24.5.2/lensmc/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,18 +407,23 @@
                             merged_blends[ii] += bb
                             merged_blends[ii] = list(set(merged_blends[ii]))
         return merged_blends
 
     def to_normalised_count_rate(self):
         if self._is_count_rate:
             raise LensMCError('Data has already been converted to normalised count rate')
-        if self.exposure_time is None or self.gain is None or self.zero_point is None:
-            raise LensMCError('Exposure time, gain and zero point must have all been set before image can be converted '
-                              'to normalised count rate.')
-        norm = self.gain / self.exposure_time / 10 ** ((self.zero_point - self.normalised_zero_point) / 2.5)
+        if self.exposure_time is None and self.gain is None and self.zero_point is None:
+            return
+        norm = 1
+        if self.gain is not None:
+            norm *= self.gain
+        if self.exposure_time is not None:
+            norm /= self.exposure_time
+        if self.zero_point is not None:
+            norm /= 10 ** ((self.zero_point - self.normalised_zero_point) / 2.5)
         for ii in range(self.n_exp):
             self[ii] *= norm[ii]
             if self.rms is not None:
                 self.rms[ii] *= norm[ii]
             if self.dc is not None:
                 self.dc[ii] *= norm[ii]
```

### Comparing `lensmc-24.5.1/lensmc/likelihood.py` & `lensmc-24.5.2/lensmc/likelihood.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/measure_shear.py` & `lensmc-24.5.2/lensmc/measure_shear.py`

 * *Files 2% similar despite different names*

```diff
@@ -719,34 +719,43 @@
             else:
                 for ii in range(self._no):
                     self.ra_samples[ii] += ra[ii]
                     self.dec_samples[ii] += dec[ii]
 
     def set_fluxes(self, snr, flux, flux_bulge, flux_disc, image):
 
-        mag = -2.5 * np.log10(flux, where=flux > 0, out=np.full_like(flux, -np.inf)) + \
-              np.full_like(flux, image.normalised_zero_point)
+        mag = -2.5 * np.log10(flux, where=flux > 0, out=np.full_like(flux, -np.inf))
+        if image.normalised_zero_point is not None:
+            mag += np.full_like(flux, image.normalised_zero_point)
         self.snr = np.mean(snr, axis=1)
         self.flux = np.mean(flux, axis=1)
         self.flux_bulge = np.mean(flux_bulge, axis=1)
         self.flux_disc = np.mean(flux_disc, axis=1)
-        self.magnitude = np.mean(mag, axis=1, where=np.isfinite(mag), out=np.full_like(self.flux, np.nan))
+        self.magnitude = np.full_like(self.flux, np.inf)
+        for ii in range(self._no):
+            ix = np.isfinite(mag[ii])
+            if np.any(ix):
+                self.magnitude[ii] = np.mean(mag[ii][ix])
         is_flux_positive = self.flux > 0
         self.bulgefrac = np.divide(self.flux_bulge, self.flux, where=is_flux_positive, out=np.full((self._no,), np.nan))
         if self._has_samples:
             self.snr_err = np.std(snr, axis=1)
             self.bulgefrac_err = np.sqrt(
                 np.divide(np.var(flux_bulge, axis=1), self.flux ** 2, where=is_flux_positive,
                           out=np.full((self._no,), np.nan)) +
                 np.var(flux, axis=1) * np.divide(self.bulgefrac ** 2, self.flux ** 4, where=is_flux_positive,
                                                  out=np.full(self._no, np.nan)))
             self.flux_err = np.std(flux, axis=1)
             self.flux_bulge_err = np.std(flux_bulge, axis=1)
             self.flux_disc_err = np.std(flux_disc, axis=1)
-            self.magnitude = np.std(mag, axis=1, where=np.isfinite(mag), out=np.full_like(self.flux, np.nan))
+            self.magnitude_err = np.full_like(self.magnitude, np.nan)
+            for ii in range(self._no):
+                ix = np.isfinite(mag[ii])
+                if np.any(ix):
+                    self.magnitude_err[ii] = np.std(mag[ii][ix])
             self.snr_samples = snr if self._n > 1 else snr.ravel()
             self.flux_samples = flux if self._n > 1 else flux.ravel()
             self.flux_bulge_samples = flux_bulge if self._n > 1 else flux_bulge.ravel()
             self.flux_disc_samples = flux_disc if self._n > 1 else flux_disc.ravel()
             self.magnitude_samples = mag if self._n > 1 else mag.ravel()
 
         if self._no == 1:
```

### Comparing `lensmc-24.5.1/lensmc/measure_shear_all.py` & `lensmc-24.5.2/lensmc/measure_shear_all.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/models.py` & `lensmc-24.5.2/lensmc/models.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/optimise.py` & `lensmc-24.5.2/lensmc/optimise.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/prior.py` & `lensmc-24.5.2/lensmc/prior.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/psf.py` & `lensmc-24.5.2/lensmc/psf.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/segmentation.py` & `lensmc-24.5.2/lensmc/segmentation.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/shear_bias.py` & `lensmc-24.5.2/lensmc/shear_bias.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/shear_utils.py` & `lensmc-24.5.2/lensmc/shear_utils.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/src/c/fast_fourier_model.cpp` & `lensmc-24.5.2/lensmc/src/c/fast_fourier_model.cpp`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/src/c/fast_fourier_model.hpp` & `lensmc-24.5.2/lensmc/src/c/fast_fourier_model.hpp`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/src/cython/cross_product.c` & `lensmc-24.5.2/lensmc/src/cython/cross_product.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-Ofast",
             "-fpic"
         ],
         "include_dirs": [
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include"
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "lensmc.cross_product",
         "sources": [
             "lensmc/src/cython/cross_product.pyx"
         ]
     },
@@ -1673,177 +1673,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1876,42 +1876,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -17913,261 +17913,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18176,29 +18176,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18209,15 +18209,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18226,29 +18226,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18259,15 +18259,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18276,29 +18276,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18309,15 +18309,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18326,29 +18326,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18359,15 +18359,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18376,29 +18376,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18409,217 +18409,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18635,15 +18635,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18651,68 +18651,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18720,15 +18720,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18743,15 +18743,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18767,15 +18767,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18783,68 +18783,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18852,15 +18852,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18875,15 +18875,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18899,15 +18899,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18915,68 +18915,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18984,15 +18984,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19007,170 +19007,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -21269,26 +21269,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `lensmc-24.5.1/lensmc/src/cython/cross_product.pyx` & `lensmc-24.5.2/lensmc/src/cython/cross_product.pyx`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/src/cython/galaxy_model.cpp` & `lensmc-24.5.2/lensmc/src/cython/galaxy_model.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "lensmc/src/c/fast_fourier_model.hpp"
         ],
         "extra_compile_args": [
             "-Ofast",
             "-fpic"
         ],
         "include_dirs": [
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include",
             "lensmc/src/c"
         ],
         "language": "c++",
         "name": "lensmc.galaxy_model",
         "sources": [
             "lensmc/src/cython/galaxy_model.pyx",
             "lensmc/src/c/fast_fourier_model.cpp"
@@ -1586,177 +1586,177 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1787,42 +1787,42 @@
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6lensmc_12galaxy_model_WorkingArrays;
 struct __pyx_obj_6lensmc_12galaxy_model___pyx_scope_struct__genexpr;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -4593,261 +4593,261 @@
 #define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
 #define __pyx_codeobj__28 __pyx_mstate_global->__pyx_codeobj__28
 #define __pyx_codeobj__30 __pyx_mstate_global->__pyx_codeobj__30
 #define __pyx_codeobj__32 __pyx_mstate_global->__pyx_codeobj__32
 #define __pyx_codeobj__34 __pyx_mstate_global->__pyx_codeobj__34
 /* #### Code section: module_code ### */
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4856,29 +4856,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4889,15 +4889,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4906,29 +4906,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4939,15 +4939,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4956,29 +4956,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4989,15 +4989,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5006,29 +5006,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5039,15 +5039,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5056,29 +5056,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5089,217 +5089,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5315,15 +5315,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5331,68 +5331,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5400,15 +5400,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5423,15 +5423,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5447,15 +5447,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5463,68 +5463,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5532,15 +5532,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5555,15 +5555,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5579,15 +5579,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5595,68 +5595,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5664,15 +5664,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5687,170 +5687,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -14849,26 +14849,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
```

### Comparing `lensmc-24.5.1/lensmc/src/cython/galaxy_model.pxd` & `lensmc-24.5.2/lensmc/src/cython/galaxy_model.pxd`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/src/cython/galaxy_model.pyx` & `lensmc-24.5.2/lensmc/src/cython/galaxy_model.pyx`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/src/cython/linear_fit.c` & `lensmc-24.5.2/lensmc/src/cython/linear_fit.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-Ofast",
             "-fpic"
         ],
         "include_dirs": [
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include"
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "lensmc.linear_fit",
         "sources": [
             "lensmc/src/cython/linear_fit.pyx"
         ]
     },
@@ -1673,177 +1673,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1876,42 +1876,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18001,261 +18001,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18264,29 +18264,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18297,15 +18297,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18314,29 +18314,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18347,15 +18347,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18364,29 +18364,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18397,15 +18397,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18414,29 +18414,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18447,15 +18447,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18464,29 +18464,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18497,217 +18497,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18723,15 +18723,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18739,68 +18739,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18808,15 +18808,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18831,15 +18831,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18855,15 +18855,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18871,68 +18871,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18940,15 +18940,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18963,15 +18963,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18987,15 +18987,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19003,68 +19003,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19072,15 +19072,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19095,170 +19095,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -23157,26 +23157,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `lensmc-24.5.1/lensmc/src/cython/linear_fit.pyx` & `lensmc-24.5.2/lensmc/src/cython/linear_fit.pyx`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/src/cython/star_model.cpp` & `lensmc-24.5.2/lensmc/src/cython/star_model.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "lensmc/src/c/fast_fourier_model.hpp"
         ],
         "extra_compile_args": [
             "-Ofast",
             "-fpic"
         ],
         "include_dirs": [
-            "/tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/core/include",
+            "/tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/core/include",
             "lensmc/src/c"
         ],
         "language": "c++",
         "name": "lensmc.star_model",
         "sources": [
             "lensmc/src/cython/star_model.pyx",
             "lensmc/src/c/fast_fourier_model.cpp"
@@ -1585,177 +1585,177 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1784,42 +1784,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3173,261 +3173,261 @@
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
 #define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
 /* #### Code section: module_code ### */
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3436,29 +3436,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3469,15 +3469,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3486,29 +3486,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3519,15 +3519,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3536,29 +3536,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3569,15 +3569,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3586,29 +3586,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3619,15 +3619,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3636,29 +3636,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3669,217 +3669,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3895,15 +3895,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3911,68 +3911,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -3980,15 +3980,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4003,15 +4003,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4027,15 +4027,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4043,68 +4043,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4112,15 +4112,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4135,15 +4135,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4159,15 +4159,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4175,68 +4175,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4244,15 +4244,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4267,170 +4267,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5406,26 +5406,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../tmp/build-env-8xct1ynd/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../tmp/build-env-q_lp_hu4/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
```

### Comparing `lensmc-24.5.1/lensmc/src/cython/star_model.pyx` & `lensmc-24.5.2/lensmc/src/cython/star_model.pyx`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/stats.py` & `lensmc-24.5.2/lensmc/stats.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/tests/test_background.py` & `lensmc-24.5.2/lensmc/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/tests/test_galaxy_runtime.py` & `lensmc-24.5.2/lensmc/tests/test_galaxy_runtime.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/tests/test_measure_shear.py` & `lensmc-24.5.2/lensmc/tests/test_measure_shear.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/tests/test_measure_shear_all.py` & `lensmc-24.5.2/lensmc/tests/test_measure_shear_all.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc/utils.py` & `lensmc-24.5.2/lensmc/utils.py`

 * *Files identical despite different names*

### Comparing `lensmc-24.5.1/lensmc.egg-info/PKG-INFO` & `lensmc-24.5.2/lensmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lensmc
-Version: 24.5.1
+Version: 24.5.2
 Summary: Python package for weak lensing shear measurements
 Home-page: https://gitlab.com/gcongedo/LensMC
 Author: Giuseppe Congedo
 Author-email: giuseppe.congedo@ed.ac.uk
 License: LGPL - Copyright (C) 2015 Giuseppe Congedo, University of Edinburgh on behalf of the Euclid Science Ground Segment
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lensmc-24.5.1/lensmc.egg-info/SOURCES.txt` & `lensmc-24.5.2/lensmc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 environment.yml
 pyproject.toml
 requirements.txt
 setup.py
 docs/description.md
 lensmc/INFO
 lensmc/__init__.py
-lensmc/catalogue.py
 lensmc/flags.py
 lensmc/image.py
 lensmc/likelihood.py
 lensmc/measure_shear.py
 lensmc/measure_shear_all.py
 lensmc/models.py
 lensmc/optimise.py
```

### Comparing `lensmc-24.5.1/setup.py` & `lensmc-24.5.2/setup.py`

 * *Files identical despite different names*

