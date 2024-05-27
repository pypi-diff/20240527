# Comparing `tmp/jaxns-2.5.0.tar.gz` & `tmp/jaxns-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxns-2.5.0.tar", last modified: Wed May 15 10:21:59 2024, max compression
+gzip compressed data, was "jaxns-2.5.1.tar", last modified: Mon May 27 08:59:29 2024, max compression
```

## Comparing `jaxns-2.5.0.tar` & `jaxns-2.5.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.363427 jaxns-2.5.0/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2518 2024-03-20 16:58:01.000000 jaxns-2.5.0/LICENSE
--rw-r--r--   0 albert    (1000) albert    (1000)    17828 2024-05-15 10:21:59.363427 jaxns-2.5.0/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)    17147 2024-05-15 09:59:15.000000 jaxns-2.5.0/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.351427 jaxns-2.5.0/jaxns/
--rw-rw-r--   0 albert    (1000) albert    (1000)      145 2024-03-12 14:37:32.000000 jaxns-2.5.0/jaxns/__init__.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.355427 jaxns-2.5.0/jaxns/experimental/
--rw-rw-r--   0 albert    (1000) albert    (1000)      147 2024-01-10 09:23:52.000000 jaxns-2.5.0/jaxns/experimental/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    13924 2024-05-08 19:44:48.000000 jaxns-2.5.0/jaxns/experimental/evidence_maximisation.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    21782 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/experimental/global_optimisation.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3280 2024-01-29 16:58:54.000000 jaxns-2.5.0/jaxns/experimental/public.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.355427 jaxns-2.5.0/jaxns/experimental/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2024-01-10 01:28:49.000000 jaxns-2.5.0/jaxns/experimental/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2065 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/experimental/tests/test_evidence_maximisation.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3961 2024-01-29 17:06:40.000000 jaxns-2.5.0/jaxns/experimental/tests/test_global_optimisation.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.355427 jaxns-2.5.0/jaxns/framework/
--rw-rw-r--   0 albert    (1000) albert    (1000)      217 2024-05-15 09:45:25.000000 jaxns-2.5.0/jaxns/framework/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5885 2024-01-31 12:49:58.000000 jaxns-2.5.0/jaxns/framework/abc.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5707 2024-03-14 00:16:44.000000 jaxns-2.5.0/jaxns/framework/bases.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1629 2024-05-15 09:45:25.000000 jaxns-2.5.0/jaxns/framework/jaxify.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6725 2024-03-12 14:42:15.000000 jaxns-2.5.0/jaxns/framework/model.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    11345 2024-03-14 00:16:44.000000 jaxns-2.5.0/jaxns/framework/ops.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6738 2024-03-12 14:33:47.000000 jaxns-2.5.0/jaxns/framework/prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    18691 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/framework/special_priors.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.355427 jaxns-2.5.0/jaxns/framework/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2024-03-11 13:51:33.000000 jaxns-2.5.0/jaxns/framework/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1067 2024-05-15 09:45:25.000000 jaxns-2.5.0/jaxns/framework/tests/test_jaxify.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4432 2024-05-15 09:45:25.000000 jaxns-2.5.0/jaxns/framework/tests/test_model.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15702 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/framework/tests/test_prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3304 2024-03-06 13:22:27.000000 jaxns-2.5.0/jaxns/framework/wrapped_tfp_distribution.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.359428 jaxns-2.5.0/jaxns/internals/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.5.0/jaxns/internals/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4281 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/internals/cumulative_ops.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      853 2023-12-11 11:21:48.000000 jaxns-2.5.0/jaxns/internals/linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12950 2023-12-20 00:59:59.000000 jaxns-2.5.0/jaxns/internals/log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)       92 2024-03-12 14:42:15.000000 jaxns-2.5.0/jaxns/internals/logging.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     8916 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/internals/maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2306 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/internals/namedtuple_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2791 2024-03-20 16:51:32.000000 jaxns-2.5.0/jaxns/internals/random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2023-07-28 03:56:05.000000 jaxns-2.5.0/jaxns/internals/shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6524 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/internals/shrinkage_statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2248 2023-12-10 16:34:32.000000 jaxns-2.5.0/jaxns/internals/stats.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.359428 jaxns-2.5.0/jaxns/internals/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.5.0/jaxns/internals/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4738 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/internals/tests/test_cumulative_ops.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      304 2023-12-11 11:21:48.000000 jaxns-2.5.0/jaxns/internals/tests/test_linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5500 2023-12-10 16:34:33.000000 jaxns-2.5.0/jaxns/internals/tests/test_log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3629 2024-01-31 03:39:54.000000 jaxns-2.5.0/jaxns/internals/tests/test_maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1760 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/internals/tests/test_namedtuple_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1337 2023-12-11 11:21:48.000000 jaxns-2.5.0/jaxns/internals/tests/test_random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2023-07-28 03:56:05.000000 jaxns-2.5.0/jaxns/internals/tests/test_shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)        3 2024-01-09 16:10:02.000000 jaxns-2.5.0/jaxns/internals/tests/test_shrink_statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-07-28 03:56:05.000000 jaxns-2.5.0/jaxns/internals/tests/test_stats.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     7880 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/internals/tests/test_tree_structure.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      792 2024-02-20 02:02:51.000000 jaxns-2.5.0/jaxns/internals/tests/test_types.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15775 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/internals/tree_structure.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     7075 2024-03-11 23:55:22.000000 jaxns-2.5.0/jaxns/internals/types.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.359428 jaxns-2.5.0/jaxns/nested_sampler/
--rw-rw-r--   0 albert    (1000) albert    (1000)       50 2023-12-10 16:33:43.000000 jaxns-2.5.0/jaxns/nested_sampler/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1132 2023-12-10 16:34:32.000000 jaxns-2.5.0/jaxns/nested_sampler/abc.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      303 2023-12-10 16:33:43.000000 jaxns-2.5.0/jaxns/nested_sampler/bases.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    36092 2024-05-08 19:44:48.000000 jaxns-2.5.0/jaxns/nested_sampler/standard_static.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    19018 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/plotting.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     7651 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/public.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.363427 jaxns-2.5.0/jaxns/samplers/
--rw-rw-r--   0 albert    (1000) albert    (1000)      198 2023-12-10 16:33:43.000000 jaxns-2.5.0/jaxns/samplers/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1892 2024-01-08 18:14:31.000000 jaxns-2.5.0/jaxns/samplers/abc.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2695 2024-01-28 16:29:45.000000 jaxns-2.5.0/jaxns/samplers/bases.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.363427 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-12-10 01:41:41.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4677 2024-02-22 03:55:35.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/em_gmm.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    29798 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/multi_ellipsoid_utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.363427 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-12-10 01:41:41.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1309 2024-02-22 03:58:12.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/tests/test_em_gmm.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5345 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4813 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoidal_samplers.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    10290 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/samplers/multi_slice_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15063 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/samplers/uni_slice_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3502 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/samplers/uniform_samplers.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.363427 jaxns-2.5.0/jaxns/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.5.0/jaxns/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    11000 2024-03-05 23:02:32.000000 jaxns-2.5.0/jaxns/tests/conftest.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3245 2024-04-26 13:09:53.000000 jaxns-2.5.0/jaxns/tests/test_nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      816 2023-12-20 00:59:59.000000 jaxns-2.5.0/jaxns/tests/test_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    20138 2024-05-08 19:44:48.000000 jaxns-2.5.0/jaxns/utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      678 2024-03-12 14:33:47.000000 jaxns-2.5.0/jaxns/warnings.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.363427 jaxns-2.5.0/jaxns.egg-info/
--rw-r--r--   0 albert    (1000) albert    (1000)    17828 2024-05-15 10:21:59.000000 jaxns-2.5.0/jaxns.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     2741 2024-05-15 10:21:59.000000 jaxns-2.5.0/jaxns.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2024-05-15 10:21:59.000000 jaxns-2.5.0/jaxns.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       92 2024-05-15 10:21:59.000000 jaxns-2.5.0/jaxns.egg-info/requires.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        6 2024-05-15 10:21:59.000000 jaxns-2.5.0/jaxns.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-28 03:56:05.000000 jaxns-2.5.0/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2024-05-15 10:21:59.363427 jaxns-2.5.0/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     1049 2024-05-15 09:56:23.000000 jaxns-2.5.0/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.838105 jaxns-2.5.1/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2518 2024-03-20 16:58:01.000000 jaxns-2.5.1/LICENSE
+-rw-r--r--   0 albert    (1000) albert    (1000)    17922 2024-05-27 08:59:29.838105 jaxns-2.5.1/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)    17241 2024-05-27 08:43:04.000000 jaxns-2.5.1/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.826105 jaxns-2.5.1/jaxns/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      145 2024-03-12 14:37:32.000000 jaxns-2.5.1/jaxns/__init__.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.826105 jaxns-2.5.1/jaxns/experimental/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      147 2024-01-10 09:23:52.000000 jaxns-2.5.1/jaxns/experimental/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    13924 2024-05-08 19:44:48.000000 jaxns-2.5.1/jaxns/experimental/evidence_maximisation.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    21782 2024-04-26 13:09:03.000000 jaxns-2.5.1/jaxns/experimental/global_optimisation.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3280 2024-01-29 16:58:54.000000 jaxns-2.5.1/jaxns/experimental/public.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.826105 jaxns-2.5.1/jaxns/experimental/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2024-01-10 01:28:49.000000 jaxns-2.5.1/jaxns/experimental/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2065 2024-04-26 13:09:03.000000 jaxns-2.5.1/jaxns/experimental/tests/test_evidence_maximisation.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3961 2024-01-29 17:06:40.000000 jaxns-2.5.1/jaxns/experimental/tests/test_global_optimisation.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.830105 jaxns-2.5.1/jaxns/framework/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      217 2024-05-15 09:45:25.000000 jaxns-2.5.1/jaxns/framework/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5885 2024-01-31 12:49:58.000000 jaxns-2.5.1/jaxns/framework/abc.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5707 2024-03-14 00:16:44.000000 jaxns-2.5.1/jaxns/framework/bases.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1629 2024-05-15 09:45:25.000000 jaxns-2.5.1/jaxns/framework/jaxify.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6725 2024-03-12 14:42:15.000000 jaxns-2.5.1/jaxns/framework/model.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11345 2024-03-14 00:16:44.000000 jaxns-2.5.1/jaxns/framework/ops.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6738 2024-03-12 14:33:47.000000 jaxns-2.5.1/jaxns/framework/prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18691 2024-04-26 13:09:03.000000 jaxns-2.5.1/jaxns/framework/special_priors.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.830105 jaxns-2.5.1/jaxns/framework/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2024-03-11 13:51:33.000000 jaxns-2.5.1/jaxns/framework/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1067 2024-05-15 09:45:25.000000 jaxns-2.5.1/jaxns/framework/tests/test_jaxify.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4432 2024-05-15 09:45:25.000000 jaxns-2.5.1/jaxns/framework/tests/test_model.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15702 2024-04-26 13:09:03.000000 jaxns-2.5.1/jaxns/framework/tests/test_prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3304 2024-03-06 13:22:27.000000 jaxns-2.5.1/jaxns/framework/wrapped_tfp_distribution.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.834105 jaxns-2.5.1/jaxns/internals/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.5.1/jaxns/internals/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4281 2024-05-15 09:16:27.000000 jaxns-2.5.1/jaxns/internals/cumulative_ops.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      853 2023-12-11 11:21:48.000000 jaxns-2.5.1/jaxns/internals/linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12950 2023-12-20 00:59:59.000000 jaxns-2.5.1/jaxns/internals/log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)       92 2024-03-12 14:42:15.000000 jaxns-2.5.1/jaxns/internals/logging.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     8916 2024-04-26 13:09:03.000000 jaxns-2.5.1/jaxns/internals/maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2306 2024-04-26 13:09:03.000000 jaxns-2.5.1/jaxns/internals/namedtuple_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2791 2024-03-20 16:51:32.000000 jaxns-2.5.1/jaxns/internals/random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2023-07-28 03:56:05.000000 jaxns-2.5.1/jaxns/internals/shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6524 2024-05-15 09:16:27.000000 jaxns-2.5.1/jaxns/internals/shrinkage_statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2248 2023-12-10 16:34:32.000000 jaxns-2.5.1/jaxns/internals/stats.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.834105 jaxns-2.5.1/jaxns/internals/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.5.1/jaxns/internals/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4738 2024-05-15 09:16:27.000000 jaxns-2.5.1/jaxns/internals/tests/test_cumulative_ops.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      304 2023-12-11 11:21:48.000000 jaxns-2.5.1/jaxns/internals/tests/test_linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5500 2023-12-10 16:34:33.000000 jaxns-2.5.1/jaxns/internals/tests/test_log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3629 2024-01-31 03:39:54.000000 jaxns-2.5.1/jaxns/internals/tests/test_maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1760 2024-04-26 13:09:03.000000 jaxns-2.5.1/jaxns/internals/tests/test_namedtuple_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1337 2023-12-11 11:21:48.000000 jaxns-2.5.1/jaxns/internals/tests/test_random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2023-07-28 03:56:05.000000 jaxns-2.5.1/jaxns/internals/tests/test_shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)        3 2024-01-09 16:10:02.000000 jaxns-2.5.1/jaxns/internals/tests/test_shrink_statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-07-28 03:56:05.000000 jaxns-2.5.1/jaxns/internals/tests/test_stats.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     7880 2024-05-15 09:16:27.000000 jaxns-2.5.1/jaxns/internals/tests/test_tree_structure.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      792 2024-02-20 02:02:51.000000 jaxns-2.5.1/jaxns/internals/tests/test_types.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15775 2024-05-15 09:16:27.000000 jaxns-2.5.1/jaxns/internals/tree_structure.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     7075 2024-05-26 12:41:46.000000 jaxns-2.5.1/jaxns/internals/types.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.834105 jaxns-2.5.1/jaxns/nested_sampler/
+-rw-rw-r--   0 albert    (1000) albert    (1000)       50 2023-12-10 16:33:43.000000 jaxns-2.5.1/jaxns/nested_sampler/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1132 2023-12-10 16:34:32.000000 jaxns-2.5.1/jaxns/nested_sampler/abc.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      303 2023-12-10 16:33:43.000000 jaxns-2.5.1/jaxns/nested_sampler/bases.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    36040 2024-05-26 12:14:17.000000 jaxns-2.5.1/jaxns/nested_sampler/standard_static.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    19008 2024-05-27 08:53:43.000000 jaxns-2.5.1/jaxns/plotting.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     7666 2024-05-26 16:23:50.000000 jaxns-2.5.1/jaxns/public.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.838105 jaxns-2.5.1/jaxns/samplers/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      198 2023-12-10 16:33:43.000000 jaxns-2.5.1/jaxns/samplers/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1892 2024-01-08 18:14:31.000000 jaxns-2.5.1/jaxns/samplers/abc.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2695 2024-01-28 16:29:45.000000 jaxns-2.5.1/jaxns/samplers/bases.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.838105 jaxns-2.5.1/jaxns/samplers/multi_ellipsoid/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-12-10 01:41:41.000000 jaxns-2.5.1/jaxns/samplers/multi_ellipsoid/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4677 2024-02-22 03:55:35.000000 jaxns-2.5.1/jaxns/samplers/multi_ellipsoid/em_gmm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    29798 2024-04-26 13:09:03.000000 jaxns-2.5.1/jaxns/samplers/multi_ellipsoid/multi_ellipsoid_utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.838105 jaxns-2.5.1/jaxns/samplers/multi_ellipsoid/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-12-10 01:41:41.000000 jaxns-2.5.1/jaxns/samplers/multi_ellipsoid/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1309 2024-02-22 03:58:12.000000 jaxns-2.5.1/jaxns/samplers/multi_ellipsoid/tests/test_em_gmm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5345 2024-04-26 13:09:03.000000 jaxns-2.5.1/jaxns/samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4813 2024-04-26 13:09:03.000000 jaxns-2.5.1/jaxns/samplers/multi_ellipsoidal_samplers.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    10290 2024-05-15 09:16:27.000000 jaxns-2.5.1/jaxns/samplers/multi_slice_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15446 2024-05-26 16:49:25.000000 jaxns-2.5.1/jaxns/samplers/uni_slice_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3502 2024-04-26 13:09:03.000000 jaxns-2.5.1/jaxns/samplers/uniform_samplers.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.838105 jaxns-2.5.1/jaxns/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.5.1/jaxns/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    10976 2024-05-26 16:57:06.000000 jaxns-2.5.1/jaxns/tests/conftest.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3245 2024-04-26 13:09:53.000000 jaxns-2.5.1/jaxns/tests/test_nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      816 2023-12-20 00:59:59.000000 jaxns-2.5.1/jaxns/tests/test_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    20138 2024-05-08 19:44:48.000000 jaxns-2.5.1/jaxns/utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      678 2024-03-12 14:33:47.000000 jaxns-2.5.1/jaxns/warnings.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-27 08:59:29.838105 jaxns-2.5.1/jaxns.egg-info/
+-rw-r--r--   0 albert    (1000) albert    (1000)    17922 2024-05-27 08:59:29.000000 jaxns-2.5.1/jaxns.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2741 2024-05-27 08:59:29.000000 jaxns-2.5.1/jaxns.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2024-05-27 08:59:29.000000 jaxns-2.5.1/jaxns.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       92 2024-05-27 08:59:29.000000 jaxns-2.5.1/jaxns.egg-info/requires.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        6 2024-05-27 08:59:29.000000 jaxns-2.5.1/jaxns.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-28 03:56:05.000000 jaxns-2.5.1/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2024-05-27 08:59:29.838105 jaxns-2.5.1/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     1049 2024-05-27 08:43:04.000000 jaxns-2.5.1/setup.py
```

### Comparing `jaxns-2.5.0/LICENSE` & `jaxns-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/PKG-INFO` & `jaxns-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxns
-Version: 2.5.0
+Version: 2.5.1
 Summary: Nested Sampling in JAX
 Home-page: https://github.com/joshuaalbert/jaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -383,19 +383,21 @@
 The algorithm is fairly memory bound, so running parallelisation over multiple CPUs on the same machine may not yield
 the expected speed up, and depends on how expensive the likelihood evaluations are. Running over separate physical
 devices
 is the best way to achieve speed up.
 
 # Change Log
 
+27 May, 2024 -- JAXS 2.5.1 released. Fixed minor accuracy degradation introduced in 2.4.13.
+
 15 May, 2024 -- JAXNS 2.5.0 released. Added ability to handle non-JAX likelihoods, e.g. if you have a simulation
 framework with python bindings you can now use it for likelihoods in JAXNS. Small performance improvements.
 
 22 Apr, 2024 -- JAXNS 2.4.13 released. Fixes bug where slice sampling not invariant to monotonic transforms of
-likelihod.
+likelihood.
 
 20 Mar, 2024 -- JAXNS 2.4.12 released. Minor bug fixes, and readability improvements. Added Empirical special prior.
 
 5 Mar, 2024 -- JAXNS 2.4.11/b released. Add `random_init` to parametrised variables. Enable special priors to be
 parametrised.
 
 23 Feb, 2024 -- JAXNS 2.4.10 released. Hotfix for import error.
```

### Comparing `jaxns-2.5.0/README.md` & `jaxns-2.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -359,19 +359,21 @@
 The algorithm is fairly memory bound, so running parallelisation over multiple CPUs on the same machine may not yield
 the expected speed up, and depends on how expensive the likelihood evaluations are. Running over separate physical
 devices
 is the best way to achieve speed up.
 
 # Change Log
 
+27 May, 2024 -- JAXS 2.5.1 released. Fixed minor accuracy degradation introduced in 2.4.13.
+
 15 May, 2024 -- JAXNS 2.5.0 released. Added ability to handle non-JAX likelihoods, e.g. if you have a simulation
 framework with python bindings you can now use it for likelihoods in JAXNS. Small performance improvements.
 
 22 Apr, 2024 -- JAXNS 2.4.13 released. Fixes bug where slice sampling not invariant to monotonic transforms of
-likelihod.
+likelihood.
 
 20 Mar, 2024 -- JAXNS 2.4.12 released. Minor bug fixes, and readability improvements. Added Empirical special prior.
 
 5 Mar, 2024 -- JAXNS 2.4.11/b released. Add `random_init` to parametrised variables. Enable special priors to be
 parametrised.
 
 23 Feb, 2024 -- JAXNS 2.4.10 released. Hotfix for import error.
```

### Comparing `jaxns-2.5.0/jaxns/experimental/evidence_maximisation.py` & `jaxns-2.5.1/jaxns/experimental/evidence_maximisation.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/experimental/global_optimisation.py` & `jaxns-2.5.1/jaxns/experimental/global_optimisation.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/experimental/public.py` & `jaxns-2.5.1/jaxns/experimental/public.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/experimental/tests/test_evidence_maximisation.py` & `jaxns-2.5.1/jaxns/experimental/tests/test_evidence_maximisation.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/experimental/tests/test_global_optimisation.py` & `jaxns-2.5.1/jaxns/experimental/tests/test_global_optimisation.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/framework/abc.py` & `jaxns-2.5.1/jaxns/framework/abc.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/framework/bases.py` & `jaxns-2.5.1/jaxns/framework/bases.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/framework/jaxify.py` & `jaxns-2.5.1/jaxns/framework/jaxify.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/framework/model.py` & `jaxns-2.5.1/jaxns/framework/model.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/framework/ops.py` & `jaxns-2.5.1/jaxns/framework/ops.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/framework/prior.py` & `jaxns-2.5.1/jaxns/framework/prior.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/framework/special_priors.py` & `jaxns-2.5.1/jaxns/framework/special_priors.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/framework/tests/test_jaxify.py` & `jaxns-2.5.1/jaxns/framework/tests/test_jaxify.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/framework/tests/test_model.py` & `jaxns-2.5.1/jaxns/framework/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/framework/tests/test_prior.py` & `jaxns-2.5.1/jaxns/framework/tests/test_prior.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/framework/wrapped_tfp_distribution.py` & `jaxns-2.5.1/jaxns/framework/wrapped_tfp_distribution.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/cumulative_ops.py` & `jaxns-2.5.1/jaxns/internals/cumulative_ops.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/linalg.py` & `jaxns-2.5.1/jaxns/internals/linalg.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/log_semiring.py` & `jaxns-2.5.1/jaxns/internals/log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/maps.py` & `jaxns-2.5.1/jaxns/internals/maps.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/namedtuple_utils.py` & `jaxns-2.5.1/jaxns/internals/namedtuple_utils.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/random.py` & `jaxns-2.5.1/jaxns/internals/random.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/shapes.py` & `jaxns-2.5.1/jaxns/internals/shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/shrinkage_statistics.py` & `jaxns-2.5.1/jaxns/internals/shrinkage_statistics.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/stats.py` & `jaxns-2.5.1/jaxns/internals/stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/tests/test_cumulative_ops.py` & `jaxns-2.5.1/jaxns/internals/tests/test_cumulative_ops.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/tests/test_log_semiring.py` & `jaxns-2.5.1/jaxns/internals/tests/test_log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/tests/test_maps.py` & `jaxns-2.5.1/jaxns/internals/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/tests/test_namedtuple_utils.py` & `jaxns-2.5.1/jaxns/internals/tests/test_namedtuple_utils.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/tests/test_random.py` & `jaxns-2.5.1/jaxns/internals/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/tests/test_shapes.py` & `jaxns-2.5.1/jaxns/internals/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/tests/test_stats.py` & `jaxns-2.5.1/jaxns/internals/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/tests/test_tree_structure.py` & `jaxns-2.5.1/jaxns/internals/tests/test_tree_structure.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/tests/test_types.py` & `jaxns-2.5.1/jaxns/internals/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/tree_structure.py` & `jaxns-2.5.1/jaxns/internals/tree_structure.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/internals/types.py` & `jaxns-2.5.1/jaxns/internals/types.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/nested_sampler/abc.py` & `jaxns-2.5.1/jaxns/nested_sampler/abc.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/nested_sampler/standard_static.py` & `jaxns-2.5.1/jaxns/nested_sampler/standard_static.py`

 * *Files 0% similar despite different names*

```diff
@@ -771,17 +771,16 @@
                 sampler=self.sampler,
                 num_samples_per_sync=self.num_live_points,
                 verbose=self.verbose
             )
             if self.num_parallel_workers > 1:
                 # We need to do a final sampling run to make all the chains consistent,
                 #  to a likelihood contour (i.e. standardise on L(X)). Would mean that some workers are idle.
-                target_log_L_contour = jnp.max(
-                    parallel.all_gather(termination_register.log_L_contour, 'i')
-                )
+                target_log_L_contour = parallel.pmax(termination_register.log_L_contour, 'i')
+
                 termination_cond = TerminationCondition(
                     dlogZ=jnp.asarray(0., float_type),
                     log_L_contour=target_log_L_contour,
                     max_samples=jnp.asarray(self.max_samples)
                 )
                 state, termination_register, termination_reason = _single_thread_ns(
                     init_state=state,
```

### Comparing `jaxns-2.5.0/jaxns/plotting.py` & `jaxns-2.5.1/jaxns/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
                 _samples = _samples[is_finite]
                 _log_weights = _log_weights[is_finite]
             _weights = np.exp(_log_weights)
 
             # Plot the 2D histogram, over ranges set by the 1_per and 99_per of each parameter
             ranges = [param_limits[parameters[col]], param_limits[parameters[row]]]
             ax.hist2d(_samples[:, 1], _samples[:, 0], bins=(nbins, nbins), density=True,
-                      cmap=plt.cm.get_cmap('bone_r'),
+                      cmap="bone_r",
                       weights=_weights, range=ranges)
 
             if kde_overlay:  # Put KDE contour on the 2D histograms
 
                 # Calculate the point density
                 x = _samples[:, 1]
                 y = _samples[:, 0]
@@ -428,15 +428,15 @@
         vmin: lower limit of color if norm is None
         vmax: upper limit of color if norm is None
     """
     divider = make_axes_locatable(ax)
     cax = divider.append_axes('right', size='5%', pad=0.05)
     if norm is None:
         norm = plt.Normalize(vmin=vmin, vmax=vmax)
-    sm = plt.cm.ScalarMappable(norm, cmap=plt.cm.get_cmap(cmap))
+    sm = plt.cm.ScalarMappable(norm, cmap=plt.colormaps.get_cmap(cmap))
     if label is None:
         ax.figure.colorbar(sm, cax=cax, orientation='vertical')
     else:
         ax.figure.colorbar(sm, cax=cax, orientation='vertical', label=label)
 
 
 def corner_cornerplot(results: NestedSamplerResults):
```

### Comparing `jaxns-2.5.0/jaxns/public.py` & `jaxns-2.5.1/jaxns/public.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             model=model,
             num_live_points=self._c,
             max_samples=max_samples,
             sampler=UniDimSliceSampler(
                 model=model,
                 num_slices=model.U_ndims * self._s,
                 num_phantom_save=self._k,
-                midpoint_shrink=True,
+                midpoint_shrink=not difficult_model,
                 perfect=True
             ),
             init_efficiency_threshold=init_efficiency_threshold,
             num_parallel_workers=num_parallel_workers,
             verbose=verbose
         )
```

### Comparing `jaxns-2.5.0/jaxns/samplers/abc.py` & `jaxns-2.5.1/jaxns/samplers/abc.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/samplers/bases.py` & `jaxns-2.5.1/jaxns/samplers/bases.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/em_gmm.py` & `jaxns-2.5.1/jaxns/samplers/multi_ellipsoid/em_gmm.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/multi_ellipsoid_utils.py` & `jaxns-2.5.1/jaxns/samplers/multi_ellipsoid/multi_ellipsoid_utils.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/tests/test_em_gmm.py` & `jaxns-2.5.1/jaxns/samplers/multi_ellipsoid/tests/test_em_gmm.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py` & `jaxns-2.5.1/jaxns/samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/samplers/multi_ellipsoidal_samplers.py` & `jaxns-2.5.1/jaxns/samplers/multi_ellipsoidal_samplers.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/samplers/multi_slice_sampler.py` & `jaxns-2.5.1/jaxns/samplers/multi_slice_sampler.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/samplers/uni_slice_sampler.py` & `jaxns-2.5.1/jaxns/samplers/uni_slice_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,43 +71,46 @@
         left: left most point (<= 0).
         right: right most point (>= 0).
 
     Returns:
         point_U: [D]
         t: selection point between [left, right]
     """
-    t = random.uniform(key, minval=left, maxval=right, dtype=float_type)
+    u = random.uniform(key, dtype=float_type)
+    t = left + u * (right - left)
     point_U = point_U0 + t * direction
     # close_to_zero = (left >= -10*jnp.finfo(left.dtype).eps) & (right <= 10*jnp.finfo(right.dtype).eps)
     # point_U = jnp.where(close_to_zero, point_U0, point_U)
     # t = jnp.where(close_to_zero, jnp.zeros_like(t), t)
     return point_U, t
 
 
 def _shrink_interval(key: PRNGKey, t: FloatArray, left: FloatArray, right: FloatArray,
-                     midpoint_shrink: bool) -> Tuple[FloatArray, FloatArray]:
+                     midpoint_shrink: bool, alpha: jax.Array) -> Tuple[FloatArray, FloatArray]:
     """
     Not successful proposal, so shrink, optionally apply exponential shrinkage.
     """
     # witout exponential shrinkage, we shrink to failed proposal point, which is 100% correct.
     left = jnp.where(t < 0., t, left)
     right = jnp.where(t > 0., t, right)
 
     if midpoint_shrink:
         # For this to be correct it must be invariant to monotonic rescaling of the likelihood.
         # Therefore, it must only use the knowledge of ordering of the likelihoods.
         # Basic version: shrink to midpoint of interval, i.e. alpha = 0.5.
         # Extended version: shrink to random point in interval.
-        alpha = random.uniform(key)
+        # do_midpoint_shrink = random.uniform(key) < 0.5
+        # alpha = 1  # 0.8  # random.uniform(key)
         left = jnp.where((t < 0.), alpha * left, left)
         right = jnp.where((t > 0.), alpha * right, right)
     return left, right
 
 
-def _new_proposal(key: PRNGKey, seed_point: SeedPoint, midpoint_shrink: bool, perfect: bool,
+def _new_proposal(key: PRNGKey, seed_point: SeedPoint, midpoint_shrink: bool, alpha: jax.Array,
+                  perfect: bool,
                   gradient_slice: bool,
                   log_L_constraint: FloatArray,
                   model: BaseAbstractModel) -> Tuple[FloatArray, FloatArray, IntArray]:
     """
     Sample from a slice about a seed point.
 
     Args:
@@ -146,15 +149,16 @@
     def body(carry: Carry) -> Carry:
         key, t_key, shrink_key = random.split(carry.key, 3)
         left, right = _shrink_interval(
             key=shrink_key,
             t=carry.t,
             left=carry.left,
             right=carry.right,
-            midpoint_shrink=midpoint_shrink
+            midpoint_shrink=midpoint_shrink,
+            alpha=alpha
         )
         point_U, t = _pick_point_in_interval(
             key=t_key,
             point_U0=seed_point.U0,
             direction=carry.direction,
             left=left,
             right=right
@@ -308,22 +312,27 @@
             U0=sample_collection.U_samples[sample_idx],
             log_L0=sample_collection.log_L[sample_idx]
         )
 
     def get_sample_from_seed(self, key: PRNGKey, seed_point: SeedPoint, log_L_constraint: FloatArray,
                              sampler_state: SamplerState) -> Tuple[Sample, Sample]:
 
-        def propose_op(sample: Sample, key: PRNGKey) -> Sample:
+        class XType(NamedTuple):
+            key: jax.Array
+            alpha: jax.Array
+
+        def propose_op(sample: Sample, x: XType) -> Sample:
             U_sample, log_L, num_likelihood_evaluations = _new_proposal(
-                key=key,
+                key=x.key,
                 seed_point=SeedPoint(
                     U0=sample.U_sample,
                     log_L0=sample.log_L
                 ),
                 midpoint_shrink=self.midpoint_shrink,
+                alpha=x.alpha,
                 perfect=self.perfect,
                 gradient_slice=self.gradient_slice,
                 log_L_constraint=log_L_constraint,
                 model=self.model
             )
             return Sample(
                 U_sample=U_sample,
@@ -334,18 +343,22 @@
 
         init_sample = Sample(
             U_sample=seed_point.U0,
             log_L_constraint=log_L_constraint,
             log_L=seed_point.log_L0,
             num_likelihood_evaluations=jnp.asarray(0, int_type)
         )
+        xs = XType(
+            key=random.split(key, self.num_slices),
+            alpha=jnp.linspace(0.5, 1., self.num_slices)
+        )
         final_sample, cumulative_samples = cumulative_op_static(
             op=propose_op,
             init=init_sample,
-            xs=random.split(key, self.num_slices)
+            xs=xs
         )
 
         # Last sample is the final sample, the rest are potential phantom samples
         # Take only the last num_phantom_save phantom samples
         phantom_samples: Sample = jax.tree.map(lambda x: x[-(self.num_phantom_save + 1):-1], cumulative_samples)
 
         # Due to the cumulative nature of the sampler, the final number of likelihood evaluations should be divided
```

### Comparing `jaxns-2.5.0/jaxns/samplers/uniform_samplers.py` & `jaxns-2.5.1/jaxns/samplers/uniform_samplers.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/tests/conftest.py` & `jaxns-2.5.1/jaxns/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,27 +317,27 @@
     # plot_cornerplot(results)
 
     return log_Z_true, results
 
 
 @pytest.fixture(scope='package')
 def all_run_results(
-        # basic_run_results,
+        basic_run_results,
         basic_with_obj_run_results,
-        # basic2_run_results,
-        # basic3_run_results,
-        # plateau_run_results,
-        # basic_mvn_run_results,
+        basic2_run_results,
+        basic3_run_results,
+        plateau_run_results,
+        basic_mvn_run_results,
         # basic_mvn_run_results_parallel,
-        # multiellipsoidal_mvn_run_results
+        multiellipsoidal_mvn_run_results
 ):
     # Return tuples with names
     return [
-        # ('basic', basic_run_results),
+        ('basic', basic_run_results),
         ('basic_with_obj', basic_with_obj_run_results),
-        # ('basic2', basic2_run_results),
-        # ('basic3', basic3_run_results),
-        # ('plateau', plateau_run_results),
-        # ('basic_mvn', basic_mvn_run_results),
+        ('basic2', basic2_run_results),
+        ('basic3', basic3_run_results),
+        ('plateau', plateau_run_results),
+        ('basic_mvn', basic_mvn_run_results),
         # ('basic_mvn_parallel', basic_mvn_run_results_parallel),
-        # ('multiellipsoidal_mvn', multiellipsoidal_mvn_run_results)
+        ('multiellipsoidal_mvn', multiellipsoidal_mvn_run_results)
     ]
```

### Comparing `jaxns-2.5.0/jaxns/tests/test_nested_sampler.py` & `jaxns-2.5.1/jaxns/tests/test_nested_sampler.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/tests/test_utils.py` & `jaxns-2.5.1/jaxns/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/utils.py` & `jaxns-2.5.1/jaxns/utils.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns/warnings.py` & `jaxns-2.5.1/jaxns/warnings.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/jaxns.egg-info/PKG-INFO` & `jaxns-2.5.1/jaxns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxns
-Version: 2.5.0
+Version: 2.5.1
 Summary: Nested Sampling in JAX
 Home-page: https://github.com/joshuaalbert/jaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -383,19 +383,21 @@
 The algorithm is fairly memory bound, so running parallelisation over multiple CPUs on the same machine may not yield
 the expected speed up, and depends on how expensive the likelihood evaluations are. Running over separate physical
 devices
 is the best way to achieve speed up.
 
 # Change Log
 
+27 May, 2024 -- JAXS 2.5.1 released. Fixed minor accuracy degradation introduced in 2.4.13.
+
 15 May, 2024 -- JAXNS 2.5.0 released. Added ability to handle non-JAX likelihoods, e.g. if you have a simulation
 framework with python bindings you can now use it for likelihoods in JAXNS. Small performance improvements.
 
 22 Apr, 2024 -- JAXNS 2.4.13 released. Fixes bug where slice sampling not invariant to monotonic transforms of
-likelihod.
+likelihood.
 
 20 Mar, 2024 -- JAXNS 2.4.12 released. Minor bug fixes, and readability improvements. Added Empirical special prior.
 
 5 Mar, 2024 -- JAXNS 2.4.11/b released. Add `random_init` to parametrised variables. Enable special priors to be
 parametrised.
 
 23 Feb, 2024 -- JAXNS 2.4.10 released. Hotfix for import error.
```

### Comparing `jaxns-2.5.0/jaxns.egg-info/SOURCES.txt` & `jaxns-2.5.1/jaxns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaxns-2.5.0/setup.py` & `jaxns-2.5.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     'jaxopt'
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='jaxns',
-      version='2.5.0',
+      version='2.5.1',
       description='Nested Sampling in JAX',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/jaxns",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       install_requires=install_requires,
```

