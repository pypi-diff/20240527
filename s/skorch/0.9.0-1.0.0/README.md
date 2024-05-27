# Comparing `tmp/skorch-0.9.0.tar.gz` & `tmp/skorch-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skorch-0.9.0.tar", last modified: Sun Aug 30 10:43:14 2020, max compression
+gzip compressed data, was "skorch-1.0.0.tar", last modified: Mon May 27 15:22:46 2024, max compression
```

## Comparing `skorch-0.9.0.tar` & `skorch-1.0.0.tar`

### file list

```diff
@@ -1,53 +1,67 @@
-drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-08-30 10:43:14.000000 skorch-0.9.0/
--rw-r--r--   0 vinh      (1000) vinh      (1000)     1543 2020-02-08 20:37:16.000000 skorch-0.9.0/LICENSE
--rw-r--r--   0 vinh      (1000) vinh      (1000)       68 2020-02-08 20:37:16.000000 skorch-0.9.0/MANIFEST.in
--rw-r--r--   0 vinh      (1000) vinh      (1000)    10061 2020-08-30 10:43:14.000000 skorch-0.9.0/PKG-INFO
--rw-r--r--   0 vinh      (1000) vinh      (1000)     7664 2020-08-16 10:14:28.000000 skorch-0.9.0/README.rst
--rw-r--r--   0 vinh      (1000) vinh      (1000)        6 2020-08-16 10:15:22.000000 skorch-0.9.0/VERSION
--rw-r--r--   0 vinh      (1000) vinh      (1000)      196 2020-05-12 19:58:32.000000 skorch-0.9.0/requirements-dev.txt
--rw-r--r--   0 vinh      (1000) vinh      (1000)       77 2020-02-08 20:37:16.000000 skorch-0.9.0/requirements.txt
--rw-r--r--   0 vinh      (1000) vinh      (1000)      211 2020-08-30 10:43:14.000000 skorch-0.9.0/setup.cfg
--rw-r--r--   0 vinh      (1000) vinh      (1000)     1027 2020-02-08 20:37:16.000000 skorch-0.9.0/setup.py
-drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch/
--rw-r--r--   0 vinh      (1000) vinh      (1000)     1532 2020-07-30 21:48:45.000000 skorch-0.9.0/skorch/__init__.py
-drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch/callbacks/
--rw-r--r--   0 vinh      (1000) vinh      (1000)      762 2020-05-12 19:58:32.000000 skorch-0.9.0/skorch/callbacks/__init__.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     2167 2020-05-11 20:35:47.000000 skorch-0.9.0/skorch/callbacks/base.py
--rw-rw-r--   0 vinh      (1000) vinh      (1000)    25295 2020-07-05 18:18:28.000000 skorch-0.9.0/skorch/callbacks/logging.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     9173 2020-06-06 18:35:12.000000 skorch-0.9.0/skorch/callbacks/lr_scheduler.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     1499 2020-05-11 20:35:47.000000 skorch-0.9.0/skorch/callbacks/regularization.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    19719 2020-05-12 19:58:32.000000 skorch-0.9.0/skorch/callbacks/scoring.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    26370 2020-07-30 21:50:11.000000 skorch-0.9.0/skorch/callbacks/training.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    11805 2020-07-30 21:50:11.000000 skorch-0.9.0/skorch/classifier.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     9522 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/cli.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    11613 2020-06-06 18:35:12.000000 skorch-0.9.0/skorch/dataset.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)      471 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/exceptions.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    16927 2020-06-06 20:15:12.000000 skorch-0.9.0/skorch/helper.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     7606 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/history.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    72668 2020-08-13 20:17:04.000000 skorch-0.9.0/skorch/net.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     2990 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/regressor.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     3000 2020-07-30 21:50:11.000000 skorch-0.9.0/skorch/scoring.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     2355 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/setter.py
-drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch/tests/
--rw-r--r--   0 vinh      (1000) vinh      (1000)        0 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/tests/__init__.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     3993 2020-06-06 18:35:12.000000 skorch-0.9.0/skorch/tests/conftest.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    11831 2020-08-16 10:14:28.000000 skorch-0.9.0/skorch/tests/test_classifier.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    11084 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/tests/test_cli.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    31725 2020-06-06 18:35:12.000000 skorch-0.9.0/skorch/tests/test_dataset.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    24150 2020-03-11 21:34:25.000000 skorch-0.9.0/skorch/tests/test_helper.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     8506 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/tests/test_history.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)   104875 2020-08-16 10:14:28.000000 skorch-0.9.0/skorch/tests/test_net.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     4027 2020-08-16 10:14:28.000000 skorch-0.9.0/skorch/tests/test_regressor.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     3813 2020-07-30 21:50:11.000000 skorch-0.9.0/skorch/tests/test_scoring.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     2493 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/tests/test_setter.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     3326 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/tests/test_toy.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    29230 2020-07-30 21:50:11.000000 skorch-0.9.0/skorch/tests/test_utils.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     4715 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/toy.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    19241 2020-08-16 10:14:26.000000 skorch-0.9.0/skorch/utils.py
-drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch.egg-info/
--rw-r--r--   0 vinh      (1000) vinh      (1000)    10061 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch.egg-info/PKG-INFO
--rw-r--r--   0 vinh      (1000) vinh      (1000)     1065 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch.egg-info/SOURCES.txt
--rw-r--r--   0 vinh      (1000) vinh      (1000)        1 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch.egg-info/dependency_links.txt
--rw-r--r--   0 vinh      (1000) vinh      (1000)        1 2020-04-12 16:28:14.000000 skorch-0.9.0/skorch.egg-info/not-zip-safe
--rw-r--r--   0 vinh      (1000) vinh      (1000)      147 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch.egg-info/requires.txt
--rw-r--r--   0 vinh      (1000) vinh      (1000)        7 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch.egg-info/top_level.txt
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-05-27 15:22:46.256257 skorch-1.0.0/
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     1543 2019-07-30 20:56:38.000000 skorch-1.0.0/LICENSE
+-rw-r--r--   0 vinh      (1000) vinh      (1000)       68 2019-07-30 20:56:38.000000 skorch-1.0.0/MANIFEST.in
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    11445 2024-05-27 15:22:46.256257 skorch-1.0.0/PKG-INFO
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     9752 2024-05-23 08:09:53.000000 skorch-1.0.0/README.rst
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)        6 2024-05-27 14:02:29.000000 skorch-1.0.0/VERSION
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      289 2023-08-30 13:19:17.000000 skorch-1.0.0/requirements-dev.txt
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)       77 2022-09-06 15:03:10.000000 skorch-1.0.0/requirements.txt
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      159 2024-05-27 15:22:46.256257 skorch-1.0.0/setup.cfg
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     1024 2023-09-04 08:41:24.000000 skorch-1.0.0/setup.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-05-27 15:22:46.248257 skorch-1.0.0/skorch/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     1255 2023-08-23 13:19:06.000000 skorch-1.0.0/skorch/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    35432 2023-06-27 09:22:43.000000 skorch-1.0.0/skorch/_doctor.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    14342 2022-09-06 15:03:10.000000 skorch-1.0.0/skorch/_version.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-05-27 15:22:46.248257 skorch-1.0.0/skorch/callbacks/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      826 2021-12-30 17:20:16.000000 skorch-1.0.0/skorch/callbacks/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2076 2023-05-08 09:03:21.000000 skorch-1.0.0/skorch/callbacks/base.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     9914 2023-08-18 11:44:20.000000 skorch-1.0.0/skorch/callbacks/flycheck_lr_scheduler.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    40915 2023-11-28 15:15:12.000000 skorch-1.0.0/skorch/callbacks/logging.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     9599 2023-08-29 08:58:56.000000 skorch-1.0.0/skorch/callbacks/lr_scheduler.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     1499 2019-10-19 11:47:17.000000 skorch-1.0.0/skorch/callbacks/regularization.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    20337 2024-02-13 13:45:57.000000 skorch-1.0.0/skorch/callbacks/scoring.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    33212 2023-08-02 13:14:17.000000 skorch-1.0.0/skorch/callbacks/training.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    13032 2024-02-13 13:45:57.000000 skorch-1.0.0/skorch/classifier.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     9988 2023-03-17 13:12:32.000000 skorch-1.0.0/skorch/cli.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    11384 2024-04-25 13:01:47.000000 skorch-1.0.0/skorch/dataset.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      860 2023-06-27 09:22:43.000000 skorch-1.0.0/skorch/exceptions.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    11490 2023-06-30 14:24:08.000000 skorch-1.0.0/skorch/flycheck_dataset.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    17482 2023-10-24 10:30:31.000000 skorch-1.0.0/skorch/helper.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    48921 2024-02-07 16:39:39.000000 skorch-1.0.0/skorch/hf.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    18268 2023-04-28 15:44:56.000000 skorch-1.0.0/skorch/history.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-05-27 15:22:46.248257 skorch-1.0.0/skorch/llm/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      283 2023-06-27 09:22:43.000000 skorch-1.0.0/skorch/llm/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    42864 2024-04-25 13:01:47.000000 skorch-1.0.0/skorch/llm/classifier.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      765 2023-06-27 09:22:43.000000 skorch-1.0.0/skorch/llm/prompts.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)   100505 2024-02-13 13:45:35.000000 skorch-1.0.0/skorch/net.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    34045 2022-11-22 10:22:52.000000 skorch-1.0.0/skorch/probabilistic.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2562 2023-06-27 09:22:43.000000 skorch-1.0.0/skorch/regressor.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2991 2021-12-30 17:20:16.000000 skorch-1.0.0/skorch/scoring.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     2355 2019-10-19 11:47:17.000000 skorch-1.0.0/skorch/setter.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-05-27 15:22:46.252257 skorch-1.0.0/skorch/tests/
+-rw-r--r--   0 vinh      (1000) vinh      (1000)        0 2019-07-30 20:56:38.000000 skorch-1.0.0/skorch/tests/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     4248 2023-06-01 09:39:55.000000 skorch-1.0.0/skorch/tests/conftest.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    30626 2023-06-30 14:56:21.000000 skorch-1.0.0/skorch/tests/flycheck_test_utils.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    17030 2024-02-13 13:45:57.000000 skorch-1.0.0/skorch/tests/test_classifier.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    13395 2023-03-17 13:12:31.000000 skorch-1.0.0/skorch/tests/test_cli.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    31560 2023-05-17 09:57:37.000000 skorch-1.0.0/skorch/tests/test_dataset.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    29178 2023-05-08 08:57:25.000000 skorch-1.0.0/skorch/tests/test_doctor.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    26598 2023-03-17 13:12:31.000000 skorch-1.0.0/skorch/tests/test_helper.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    54075 2023-08-30 13:19:17.000000 skorch-1.0.0/skorch/tests/test_hf.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    18572 2024-05-27 14:02:29.000000 skorch-1.0.0/skorch/tests/test_history.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)   161203 2024-05-27 15:00:02.000000 skorch-1.0.0/skorch/tests/test_net.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    24474 2023-06-27 09:22:43.000000 skorch-1.0.0/skorch/tests/test_probabilistic.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     6444 2023-06-27 09:22:43.000000 skorch-1.0.0/skorch/tests/test_regressor.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     3849 2021-12-30 17:20:16.000000 skorch-1.0.0/skorch/tests/test_scoring.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     2493 2019-10-19 11:47:17.000000 skorch-1.0.0/skorch/tests/test_setter.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     3326 2019-10-19 11:47:17.000000 skorch-1.0.0/skorch/tests/test_toy.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    30776 2023-07-06 12:32:05.000000 skorch-1.0.0/skorch/tests/test_utils.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     4715 2019-10-19 11:47:17.000000 skorch-1.0.0/skorch/toy.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    22201 2023-10-24 10:56:26.000000 skorch-1.0.0/skorch/utils.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-05-27 15:22:46.252257 skorch-1.0.0/skorch.egg-info/
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    11445 2024-05-27 15:22:46.000000 skorch-1.0.0/skorch.egg-info/PKG-INFO
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     1401 2024-05-27 15:22:46.000000 skorch-1.0.0/skorch.egg-info/SOURCES.txt
+-rw-r--r--   0 vinh      (1000) vinh      (1000)        1 2024-05-27 15:22:46.000000 skorch-1.0.0/skorch.egg-info/dependency_links.txt
+-rw-r--r--   0 vinh      (1000) vinh      (1000)        1 2019-08-01 20:50:02.000000 skorch-1.0.0/skorch.egg-info/not-zip-safe
+-rw-r--r--   0 vinh      (1000) vinh      (1000)      418 2024-05-27 15:22:46.000000 skorch-1.0.0/skorch.egg-info/requires.txt
+-rw-r--r--   0 vinh      (1000) vinh      (1000)        7 2024-05-27 15:22:46.000000 skorch-1.0.0/skorch.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `skorch-0.9.0/LICENSE` & `skorch-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skorch-0.9.0/README.rst` & `skorch-1.0.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,68 @@
-.. image:: https://github.com/skorch-dev/skorch/blob/master/assets/skorch.svg
+.. image:: https://github.com/skorch-dev/skorch/blob/master/assets/skorch_bordered.svg
    :width: 30%
 
 ------------
 
-|build| |coverage| |docs| |powered|
+|build| |coverage| |docs| |huggingface| |powered|
 
 A scikit-learn compatible neural network library that wraps PyTorch.
 
-.. |build| image:: https://api.travis-ci.org/skorch-dev/skorch.svg?branch=master
-    :alt: Build Status
+.. |build| image:: https://github.com/skorch-dev/skorch/workflows/tests/badge.svg
+    :alt: Test Status
     :scale: 100%
-    :target: https://travis-ci.org/skorch-dev/skorch?branch=master
 
 .. |coverage| image:: https://github.com/skorch-dev/skorch/blob/master/assets/coverage.svg
     :alt: Test Coverage
     :scale: 100%
 
 .. |docs| image:: https://readthedocs.org/projects/skorch/badge/?version=latest
     :alt: Documentation Status
     :scale: 100%
     :target: https://skorch.readthedocs.io/en/latest/?badge=latest
 
+.. |huggingface| image:: https://github.com/skorch-dev/skorch/actions/workflows/test-hf-integration.yml/badge.svg
+    :alt: Hugging Face Integration
+    :scale: 100%
+    :target: https://github.com/skorch-dev/skorch/actions/workflows/test-hf-integration.yml
+
 .. |powered| image:: https://github.com/skorch-dev/skorch/blob/master/assets/powered.svg
     :alt: Powered by
     :scale: 100%
     :target: https://github.com/ottogroup/
 
 =========
 Resources
 =========
 
 - `Documentation <https://skorch.readthedocs.io/en/latest/?badge=latest>`_
 - `Source Code <https://github.com/skorch-dev/skorch/>`_
+- `Installation <https://github.com/skorch-dev/skorch#installation>`_
 
 ========
 Examples
 ========
 
 To see more elaborate examples, look `here
 <https://github.com/skorch-dev/skorch/tree/master/notebooks/README.md>`__.
 
 .. code:: python
 
     import numpy as np
     from sklearn.datasets import make_classification
     from torch import nn
-
     from skorch import NeuralNetClassifier
 
-
     X, y = make_classification(1000, 20, n_informative=10, random_state=0)
     X = X.astype(np.float32)
     y = y.astype(np.int64)
 
     class MyModule(nn.Module):
         def __init__(self, num_units=10, nonlin=nn.ReLU()):
-            super(MyModule, self).__init__()
+            super().__init__()
 
             self.dense0 = nn.Linear(20, num_units)
             self.nonlin = nonlin
             self.dropout = nn.Dropout(0.5)
             self.dense1 = nn.Linear(num_units, num_units)
             self.output = nn.Linear(num_units, 2)
             self.softmax = nn.Softmax(dim=-1)
@@ -67,15 +70,14 @@
         def forward(self, X, **kwargs):
             X = self.nonlin(self.dense0(X))
             X = self.dropout(X)
             X = self.nonlin(self.dense1(X))
             X = self.softmax(self.output(X))
             return X
 
-
     net = NeuralNetClassifier(
         MyModule,
         max_epochs=10,
         lr=0.1,
         # Shuffle training data on each epoch
         iterator_train__shuffle=True,
     )
@@ -86,30 +88,28 @@
 In an `sklearn Pipeline <https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html>`_:
 
 .. code:: python
 
     from sklearn.pipeline import Pipeline
     from sklearn.preprocessing import StandardScaler
 
-
     pipe = Pipeline([
         ('scale', StandardScaler()),
         ('net', net),
     ])
 
     pipe.fit(X, y)
     y_proba = pipe.predict_proba(X)
 
 With `grid search <https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html>`_:
 
 .. code:: python
 
     from sklearn.model_selection import GridSearchCV
 
-
     # deactivate skorch-internal train-valid split and verbose logging
     net.set_params(train_split=False, verbose=0)
     params = {
         'lr': [0.01, 0.02],
         'max_epochs': [10, 20],
         'module__num_units': [10, 20],
     }
@@ -124,20 +124,22 @@
 - `Learning rate schedulers <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.LRScheduler>`_ (Warm restarts, cyclic LR and many more)
 - `Scoring using sklearn (and custom) scoring functions <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.EpochScoring>`_
 - `Early stopping <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.EarlyStopping>`_
 - `Checkpointing <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.Checkpoint>`_
 - `Parameter freezing/unfreezing <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.Freezer>`_
 - `Progress bar <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.ProgressBar>`_ (for CLI as well as jupyter)
 - `Automatic inference of CLI parameters <https://github.com/skorch-dev/skorch/tree/master/examples/cli>`_
+- `Integration with GPyTorch for Gaussian Processes <https://skorch.readthedocs.io/en/latest/user/probabilistic.html>`_
+- `Integration with Hugging Face 🤗 <https://skorch.readthedocs.io/en/stable/user/huggingface.html>`_
 
 ============
 Installation
 ============
 
-skorch requires Python 3.5 or higher.
+skorch requires Python 3.8 or higher.
 
 conda installation
 ==================
 
 You need a working conda installation. Get the correct miniconda for
 your system from `here <https://conda.io/miniconda.html>`__.
 
@@ -156,15 +158,15 @@
 pip installation
 ================
 
 To install with pip, run:
 
 .. code:: bash
 
-    pip install -U skorch
+    python -m pip install -U skorch
 
 Again, we recommend to use a `virtual environment
 <https://docs.python.org/3/tutorial/venv.html>`_ for this.
 
 From source
 ===========
 
@@ -176,91 +178,121 @@
 
 To install skorch from source using conda, proceed as follows:
 
 .. code:: bash
 
     git clone https://github.com/skorch-dev/skorch.git
     cd skorch
-    conda env create
-    source activate skorch
-    pip install .
+    conda create -n skorch-env python=3.10
+    conda activate skorch-env
+    conda install -c pytorch pytorch
+    python -m pip install -r requirements.txt
+    python -m pip install .
 
 If you want to help developing, run:
 
 .. code:: bash
 
     git clone https://github.com/skorch-dev/skorch.git
     cd skorch
-    conda env create
-    source activate skorch
-    pip install -e .
+    conda create -n skorch-env python=3.10
+    conda activate skorch-env
+    conda install -c pytorch pytorch
+    python -m pip install -r requirements.txt
+    python -m pip install -r requirements-dev.txt
+    python -m pip install -e .
 
     py.test  # unit tests
     pylint skorch  # static code checks
 
+You may adjust the Python version to any of the supported Python versions.
+
 Using pip
 ---------
 
 For pip, follow these instructions instead:
 
 .. code:: bash
 
     git clone https://github.com/skorch-dev/skorch.git
     cd skorch
     # create and activate a virtual environment
-    pip install -r requirements.txt
+    python -m pip install -r requirements.txt
     # install pytorch version for your system (see below)
-    pip install .
+    python -m pip install .
 
 If you want to help developing, run:
 
 .. code:: bash
 
     git clone https://github.com/skorch-dev/skorch.git
     cd skorch
     # create and activate a virtual environment
-    pip install -r requirements.txt
+    python -m pip install -r requirements.txt
     # install pytorch version for your system (see below)
-    pip install -r requirements-dev.txt
-    pip install -e .
+    python -m pip install -r requirements-dev.txt
+    python -m pip install -e .
 
     py.test  # unit tests
     pylint skorch  # static code checks
 
 PyTorch
 =======
 
 PyTorch is not covered by the dependencies, since the PyTorch version
 you need is dependent on your OS and device. For installation
 instructions for PyTorch, visit the `PyTorch website
 <http://pytorch.org/>`__. skorch officially supports the last four
 minor PyTorch versions, which currently are:
 
-- 1.3.1
-- 1.4.0
-- 1.5.1
-- 1.6.0
+- 2.0.1
+- 2.1.2
+- 2.2.2
+- 2.3.0
 
 However, that doesn't mean that older versions don't work, just that
 they aren't tested. Since skorch mostly relies on the stable part of
 the PyTorch API, older PyTorch versions should work fine.
 
-In general, running this to install PyTorch should work (assuming CUDA
-10.2):
+In general, running this to install PyTorch should work:
 
 .. code:: bash
 
     # using conda:
-    conda install pytorch cudatoolkit==10.2 -c pytorch
+    conda install pytorch pytorch-cuda -c pytorch
     # using pip
-    pip install torch
+    python -m pip install torch
+
+==================
+External resources
+==================
+
+- @jakubczakon: `blog post
+  <https://neptune.ai/blog/model-training-libraries-pytorch-ecosystem>`_
+  "8 Creators and Core Contributors Talk About Their Model Training
+  Libraries From PyTorch Ecosystem" 2020
+- @BenjaminBossan: `talk 1
+  <https://www.youtube.com/watch?v=Qbu_DCBjVEk>`_ "skorch: A
+  scikit-learn compatible neural network library" at PyCon/PyData 2019
+- @githubnemo: `poster <https://github.com/githubnemo/skorch-poster>`_
+  for the PyTorch developer conference 2019
+- @thomasjpfan: `talk 2 <https://www.youtube.com/watch?v=0J7FaLk0bmQ>`_
+  "Skorch: A Union of Scikit learn and PyTorch" at SciPy 2019
+- @thomasjpfan: `talk 3 <https://www.youtube.com/watch?v=yAXsxf2CQ8M>`_
+  "Skorch - A Union of Scikit-learn and PyTorch" at PyData 2018
+- @BenjaminBossan: `talk 4 <https://youtu.be/y_n7BjDCS-M>`_ "Extend your
+  scikit-learn workflow with Hugging Face and skorch" at PyData Amsterdam 2023
+  (`slides 4 <https://github.com/BenjaminBossan/presentations/blob/main/2023-09-14-pydata/presentation.org>`_)
 
 =============
 Communication
 =============
 
+- `GitHub discussions <https://github.com/skorch-dev/skorch/discussions>`_: 
+  user questions, thoughts, install issues, general discussions.
+
 - `GitHub issues <https://github.com/skorch-dev/skorch/issues>`_: bug
-  reports, feature requests, install issues, RFCs, thoughts, etc.
+  reports, feature requests, RFCs, etc.
 
 - Slack: We run the #skorch channel on the `PyTorch Slack server
   <https://pytorch.slack.com/>`_, for which you can `request access
   here <https://bit.ly/ptslack>`_.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `skorch-0.9.0/setup.py` & `skorch-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,45 +5,43 @@
 
 with open('VERSION', 'r') as f:
     version = f.read().rstrip()
 
 with open('requirements.txt') as f:
     install_requires = [l.strip() for l in f]
 
-tests_require = [
-    'pytest',
-    'pytest-cov',
-]
+with open('requirements-dev.txt') as f:
+    tests_require = [l.strip() for l in f]
+
+
+python_requires = '>=3.8'
 
 docs_require = [
     'Sphinx',
     'sphinx_rtd_theme',
     'numpydoc',
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 try:
     README = open(os.path.join(here, 'README.rst')).read()
 except IOError:
     README = ''
 
-try:
-    CHANGES = open(os.path.join(here, 'CHANGES.txt')).read()
-except IOError:
-    CHANGES = ''
 
 setup(
     name='skorch',
     version=version,
     description='scikit-learn compatible neural network library for pytorch',
     long_description=README,
     license='new BSD 3-Clause',
     packages=find_packages(),
     include_package_data=True,
     url="https://github.com/skorch-dev/skorch",
     zip_safe=False,
+    python_requires=python_requires,
     install_requires=install_requires,
     extras_require={
         'testing': tests_require,
         'docs': docs_require,
     },
 )
```

### Comparing `skorch-0.9.0/skorch/__init__.py` & `skorch-1.0.0/skorch/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,48 @@
 """skorch base imports"""
 
 import sys
 import warnings
 
-import pkg_resources
-from pkg_resources import parse_version
+import importlib.metadata
 
 from .history import History
 from .net import NeuralNet
 from .classifier import NeuralNetClassifier
 from .classifier import NeuralNetBinaryClassifier
 from .regressor import NeuralNetRegressor
 from . import callbacks
+from ._version import Version
 
 
 MIN_TORCH_VERSION = '1.1.0'
 
 
-# TODO: remove in skorch 0.10.0
-if sys.version_info < (3, 6):
-    warnings.warn(
-        "Official support for Python 3.5 will be dropped starting from "
-        "skorch version 0.10.0",
-        FutureWarning,
-    )
-
 try:
     # pylint: disable=wrong-import-position
     import torch
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
         "No module named 'torch', and skorch depends on PyTorch "
         "(aka 'torch'). "
         "Visit https://pytorch.org/ for installation instructions.")
 
-torch_version = pkg_resources.get_distribution('torch').version
-if parse_version(torch_version) < parse_version(MIN_TORCH_VERSION):
+torch_version = torch.__version__
+if Version(torch_version) < Version(MIN_TORCH_VERSION):
     msg = ('skorch depends on a newer version of PyTorch (at least {req}, not '
            '{installed}). Visit https://pytorch.org for installation details')
     raise ImportWarning(msg.format(req=MIN_TORCH_VERSION, installed=torch_version))
 
 
 __all__ = [
     'History',
     'NeuralNet',
     'NeuralNetClassifier',
     'NeuralNetBinaryClassifier',
     'NeuralNetRegressor',
     'callbacks',
 ]
 
-
 try:
-    __version__ = pkg_resources.get_distribution('skorch').version
+    __version__ = importlib.metadata.version("skorch")
 except:  # pylint: disable=bare-except
     __version__ = 'n/a'
```

### Comparing `skorch-0.9.0/skorch/callbacks/__init__.py` & `skorch-1.0.0/skorch/callbacks/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,20 +20,23 @@
     'Checkpoint',
     'EarlyStopping',
     'EpochScoring',
     'EpochTimer',
     'Freezer',
     'GradientNormClipping',
     'Initializer',
+    'InputShapeSetter',
     'LRScheduler',
     'LoadInitState',
+    'MlflowLogger',
     'NeptuneLogger',
     'ParamMapper',
     'PassthroughScoring',
     'PrintLog',
     'ProgressBar',
     'TrainEndCheckpoint',
     'TensorBoard',
+    'SacredLogger',
     'Unfreezer',
     'WandbLogger',
     'WarmRestartLR',
 ]
```

### Comparing `skorch-0.9.0/skorch/callbacks/base.py` & `skorch-1.0.0/skorch/callbacks/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """ Basic callback definition. """
 
+import warnings
+
 from sklearn.base import BaseEstimator
+from skorch.exceptions import SkorchWarning
 
 
 __all__ = ['Callback']
 
 
 class Callback:
     """Base class for callbacks.
@@ -24,45 +27,39 @@
         when the model is re-initialized.
 
         This method should return self.
 
         """
         return self
 
-    def on_train_begin(self, net,
-                       X=None, y=None, **kwargs):
+    def on_train_begin(self, net, X=None, y=None, **kwargs):
         """Called at the beginning of training."""
 
-    def on_train_end(self, net,
-                     X=None, y=None, **kwargs):
+    def on_train_end(self, net, X=None, y=None, **kwargs):
         """Called at the end of training."""
 
-    def on_epoch_begin(self, net,
-                       dataset_train=None, dataset_valid=None, **kwargs):
+    def on_epoch_begin(self, net, dataset_train=None, dataset_valid=None, **kwargs):
         """Called at the beginning of each epoch."""
 
-    def on_epoch_end(self, net,
-                     dataset_train=None, dataset_valid=None, **kwargs):
+    def on_epoch_end(self, net, dataset_train=None, dataset_valid=None, **kwargs):
         """Called at the end of each epoch."""
 
-    def on_batch_begin(self, net,
-                       X=None, y=None, training=None, **kwargs):
+    def on_batch_begin(self, net, batch=None, training=None, **kwargs):
         """Called at the beginning of each batch."""
 
-    def on_batch_end(self, net,
-                     X=None, y=None, training=None, **kwargs):
+    def on_batch_end(self, net, batch=None, training=None, **kwargs):
         """Called at the end of each batch."""
 
-    def on_grad_computed(self, net, named_parameters,
-                         X=None, y=None, training=None, **kwargs):
+    def on_grad_computed(
+            self, net, named_parameters, X=None, y=None, training=None, **kwargs):
         """Called once per batch after gradients have been computed but before
         an update step was performed.
         """
 
     def _get_param_names(self):
-        return (key for key in self.__dict__ if not key.endswith('_'))
+        return [key for key in self.__dict__ if not key.endswith('_')]
 
     def get_params(self, deep=True):
         return BaseEstimator.get_params(self, deep=deep)
 
     def set_params(self, **params):
         BaseEstimator.set_params(self, **params)
```

### Comparing `skorch-0.9.0/skorch/callbacks/logging.py` & `skorch-1.0.0/skorch/callbacks/logging.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """ Callbacks for printing, logging and log information."""
 
 import sys
 import time
+import tempfile
 from contextlib import suppress
 from numbers import Number
 from itertools import cycle
 from pathlib import Path
 
 import numpy as np
 import tqdm
 from tabulate import tabulate
 
 from skorch.utils import Ansi
 from skorch.dataset import get_len
 from skorch.callbacks import Callback
 
 __all__ = ['EpochTimer', 'NeptuneLogger', 'WandbLogger', 'PrintLog', 'ProgressBar',
-           'TensorBoard']
+           'TensorBoard', 'SacredLogger', 'MlflowLogger']
 
 
 def filter_log_keys(keys, keys_ignored=None):
     """Filter out keys that are generally to be ignored.
 
     This is used by several callbacks to filter out keys from history
     that should not be logged.
@@ -60,156 +61,237 @@
         self.epoch_start_time_ = time.time()
 
     def on_epoch_end(self, net, **kwargs):
         net.history.record('dur', time.time() - self.epoch_start_time_)
 
 
 class NeptuneLogger(Callback):
-    """Logs results from history to Neptune
+    """Logs model metadata and training metrics to Neptune.
 
-    Neptune is a lightweight experiment tracking tool.
+    Neptune is a lightweight experiment-tracking tool.
     You can read more about it here: https://neptune.ai
 
     Use this callback to automatically log all interesting values from
     your net's history to Neptune.
 
     The best way to log additional information is to log directly to the
-    experiment object or subclass the ``on_*`` methods.
+    run object.
 
-    To monitor resource consumption install psutil
+    To monitor resource consumption, install psutil:
 
-    >>> pip install psutil
+    $ python -m pip install psutil
 
     You can view example experiment logs here:
-    https://ui.neptune.ai/o/shared/org/skorch-integration/e/SKOR-13/charts
+    https://app.neptune.ai/o/common/org/skorch-integration/e/SKOR-32/all
 
     Examples
     --------
-    >>> # Install neptune
-    >>> pip install neptune-client
-    >>> # Create a neptune experiment object
+    $ # Install Neptune
+    $ python -m pip install neptune
+
+    >>> # Create a Neptune run
     >>> import neptune
-    ...
-    ... # We are using api token for an anonymous user.
-    ... # For your projects use the token associated with your neptune.ai account
-    >>> neptune.init(api_token='ANONYMOUS',
-    ...              project_qualified_name='shared/skorch-integration')
-    ...
-    ... experiment = neptune.create_experiment(
-    ...                        name='skorch-basic-example',
-    ...                        params={'max_epochs': 20,
-    ...                                'lr': 0.01},
-    ...                        upload_source_files=['skorch_example.py'])
+    >>> from neptune.types import File
+    >>> # This example uses the API token for anonymous users.
+    >>> # For your own projects, use the token associated with your neptune.ai account.
+    >>> run = neptune.init_run(
+    ...     api_token=neptune.ANONYMOUS_API_TOKEN,
+    ...     project='shared/skorch-integration',
+    ...     name='skorch-basic-example',
+    ...     source_files=['skorch_example.py'],
+    ... )
 
-    >>> # Create a neptune_logger callback
-    >>> neptune_logger = NeptuneLogger(experiment, close_after_train=False)
+    >>> # Create a NeptuneLogger callback
+    >>> neptune_logger = NeptuneLogger(run, close_after_train=False)
 
-    >>> # Pass a logger to net callbacks argument
+    >>> # Pass the logger to the net callbacks argument
     >>> net = NeuralNetClassifier(
     ...           ClassifierModule,
     ...           max_epochs=20,
     ...           lr=0.01,
-    ...           callbacks=[neptune_logger])
+    ...           callbacks=[neptune_logger, Checkpoint(dirname="./checkpoints")])
+    >>> net.fit(X, y)
+
+    >>> # Save the checkpoints to Neptune
+    >>> neptune_logger.run["checkpoints"].upload_files("./checkpoints")
 
     >>> # Log additional metrics after training has finished
     >>> from sklearn.metrics import roc_auc_score
-    ... y_pred = net.predict_proba(X)
-    ... auc = roc_auc_score(y, y_pred[:, 1])
-    ...
-    ... neptune_logger.experiment.log_metric('roc_auc_score', auc)
-
-    >>> # log charts like ROC curve
-    ... from scikitplot.metrics import plot_roc
-    ... import matplotlib.pyplot as plt
-    ...
-    ... fig, ax = plt.subplots(figsize=(16, 12))
-    ... plot_roc(y, y_pred, ax=ax)
-    ... neptune_logger.experiment.log_image('roc_curve', fig)
-
-    >>> # log net object after training
-    ... net.save_params(f_params='basic_model.pkl')
-    ... neptune_logger.experiment.log_artifact('basic_model.pkl')
+    >>> y_proba = net.predict_proba(X)
+    >>> auc = roc_auc_score(y, y_proba[:, 1])
+    >>> neptune_logger.run["roc_auc_score"].log(auc)
+
+    >>> # Log charts, such as an ROC curve
+    >>> from sklearn.metrics import RocCurveDisplay
+    >>> roc_plot = RocCurveDisplay.from_estimator(net, X, y)
+    >>> neptune_logger.run["roc_curve"].upload(File.as_html(roc_plot.figure_))
+
+    >>> # Log the net object after training
+    >>> net.save_params(f_params='basic_model.pkl')
+    >>> neptune_logger.run["basic_model"].upload(File('basic_model.pkl'))
 
-    >>> # close experiment
-    ... neptune_logger.experiment.stop()
+    >>> # Close the run
+    >>> neptune_logger.run.stop()
 
     Parameters
     ----------
-    experiment : neptune.experiments.Experiment
-      Instantiated ``Experiment`` class.
+    run : neptune.Run or neptune.handler.Handler
+      Instantiated ``Run`` or ``Handler`` class.
 
     log_on_batch_end : bool (default=False)
       Whether to log loss and other metrics on batch level.
 
     close_after_train : bool (default=True)
-      Whether to close the ``Experiment`` object once training
+      Whether to close the ``Run`` object once training
       finishes. Set this parameter to False if you want to continue
-      logging to the same Experiment or if you use it as a context
+      logging to the same run or if you use it as a context
       manager.
 
     keys_ignored : str or list of str (default=None)
-      Key or list of keys that should not be logged to
-      Neptune. Note that in addition to the keys provided by the
-      user, keys such as those starting with 'event_' or ending on
-      '_best' are ignored by default.
+      Key or list of keys that should not be logged to Neptune. Note that in
+      addition to the keys provided by the user, keys such as those starting
+      with ``'event_'`` or ending on ``'_best'`` are ignored by default.
+
+    base_namespace: str
+      Namespace (folder) under which all metadata logged by the ``NeptuneLogger``
+      will be stored. Defaults to "training".
 
     Attributes
     ----------
-    first_batch_ : bool
-        Helper attribute that is set to True at initialization and changes
-        to False on first batch end. Can be used when we want to log things
-        exactly once.
-
     .. _Neptune: https://www.neptune.ai
 
     """
 
     def __init__(
             self,
-            experiment,
+            run,
+            *,
             log_on_batch_end=False,
             close_after_train=True,
             keys_ignored=None,
+            base_namespace='training',
     ):
-        self.experiment = experiment
+        self.run = run
         self.log_on_batch_end = log_on_batch_end
         self.close_after_train = close_after_train
         self.keys_ignored = keys_ignored
+        self.base_namespace = base_namespace
 
-    def initialize(self):
-        self.first_batch_ = True
+    def _log_integration_version(self) -> None:
+        from skorch import __version__
+
+        self.run['source_code/integrations/skorch'] = __version__
 
+    @property
+    def _metric_logger(self):
+        return self.run[self._base_namespace]
+
+    @staticmethod
+    def _get_obj_name(obj):
+        return type(obj).__name__
+
+    def initialize(self):
         keys_ignored = self.keys_ignored
         if isinstance(keys_ignored, str):
             keys_ignored = [keys_ignored]
         self.keys_ignored_ = set(keys_ignored or [])
         self.keys_ignored_.add('batches')
+
+        if self.base_namespace.endswith("/"):
+            self._base_namespace = self.base_namespace[:-1]
+        else:
+            self._base_namespace = self.base_namespace
+
+        self._log_integration_version()
+
         return self
 
+    def on_train_begin(self, net, X, y, **kwargs):
+        # TODO: we might want to improve logging of the multi-module net objects, see:
+        #       https://github.com/skorch-dev/skorch/pull/906#discussion_r993514643
+
+        self._metric_logger['model/model_type'] = self._get_obj_name(net.module_)
+        self._metric_logger['model/summary'] = self._model_summary_file(net.module_)
+
+        self._metric_logger['config/optimizer'] = self._get_obj_name(net.optimizer_)
+        self._metric_logger['config/criterion'] = self._get_obj_name(net.criterion_)
+        self._metric_logger['config/lr'] = net.lr
+        self._metric_logger['config/epochs'] = net.max_epochs
+        self._metric_logger['config/batch_size'] = net.batch_size
+        self._metric_logger['config/device'] = net.device
+
     def on_batch_end(self, net, **kwargs):
         if self.log_on_batch_end:
             batch_logs = net.history[-1]['batches'][-1]
 
             for key in filter_log_keys(batch_logs.keys(), self.keys_ignored_):
-                self.experiment.log_metric(key, batch_logs[key])
-
-        self.first_batch_ = False
+                self._log_metric(key, batch_logs, batch=True)
 
     def on_epoch_end(self, net, **kwargs):
         """Automatically log values from the last history step."""
-        history = net.history
-        epoch_logs = history[-1]
-        epoch = epoch_logs['epoch']
+        epoch_logs = net.history[-1]
 
         for key in filter_log_keys(epoch_logs.keys(), self.keys_ignored_):
-            self.experiment.log_metric(key, x=epoch, y=epoch_logs[key])
+            self._log_metric(key, epoch_logs, batch=False)
 
     def on_train_end(self, net, **kwargs):
+        try:
+            self._metric_logger['train/epoch/event_lr'].append(net.history[:, 'event_lr'])
+        except KeyError:
+            pass
         if self.close_after_train:
-            self.experiment.stop()
+            try:  # >1.0 package structure
+                from neptune.handler import Handler
+            except ImportError:  # <1.0 package structure
+                from neptune.new.handler import Handler
+
+            # Neptune integrations now accept passing Handler object
+            # to an integration.
+            # Ref: https://docs.neptune.ai/api/field_types/#handler
+            # Example of getting an handler from a `Run` object.
+            # handler = run["foo"]
+            # handler['bar'] = 1  # Logs to `foo/bar`
+            # NOTE: Handler provides most of the functionality of `Run`
+            # for logging, however it doesn't implement a few methods like
+            # `stop`, `wait`, etc.
+            root_obj = self.run
+            if isinstance(self.run, Handler):
+                root_obj = self.run.get_root_object()
+
+            root_obj.stop()
+
+    def _log_metric(self, name, logs, batch):
+        kind, _, key = name.partition('_')
+
+        if not key:
+            key = 'epoch_duration' if kind == 'dur' else kind
+            self._metric_logger[key].append(logs[name])
+        else:
+            if kind == 'valid':
+                kind = 'validation'
+
+            if batch:
+                granularity = 'batch'
+            else:
+                granularity = 'epoch'
+
+            # for example:     train /   epoch   / loss
+            self._metric_logger[kind][granularity][key].append(logs[name])
+
+    @staticmethod
+    def _model_summary_file(model):
+        try:
+            # neptune-client>=1.0.0 package structure
+            from neptune.types import File
+        except ImportError:
+            # neptune-client=0.9.0+ package structure
+            from neptune.new.types import File
+
+        return File.from_content(str(model), extension='txt')
+
 
 class WandbLogger(Callback):
     """Logs best model and metrics to `Weights & Biases <https://docs.wandb.com/>`_
 
     Use this callback to automatically log best trained model, all metrics from
     your net's history, model topology and computer resources to Weights & Biases
     after each epoch.
@@ -218,15 +300,15 @@
 
     See `example run
     <https://app.wandb.ai/borisd13/skorch/runs/s20or4ct/overview?workspace=user-borisd13>`_
 
     Examples
     --------
     >>> # Install wandb
-    ... pip install wandb
+    ... python -m pip install wandb
 
     >>> import wandb
     >>> from skorch.callbacks import WandbLogger
 
     >>> # Create a wandb Run
     ... wandb_run = wandb.init()
     >>> # Alternative: Create a wandb Run without having a W&B account
@@ -244,18 +326,18 @@
       wandb Run used to log data.
 
     save_model : bool (default=True)
       Whether to save a checkpoint of the best model and upload it
       to your Run on W&B servers.
 
     keys_ignored : str or list of str (default=None)
-      Key or list of keys that should not be logged to
-      tensorboard. Note that in addition to the keys provided by the
-      user, keys such as those starting with 'event_' or ending on
-      '_best' are ignored by default.
+      Key or list of keys that should not be logged to wandb. Note that in
+      addition to the keys provided by the user, keys such as those starting
+      with ``'event_'`` or ending on ``'_best'`` are ignored by default.
+
     """
 
     def __init__(
             self,
             wandb_run,
             save_model=True,
             keys_ignored=None,
@@ -314,18 +396,18 @@
     *Note*: ``PrintLog`` will not result in good outputs if the number
     of columns varies between epochs, e.g. if the valid loss is only
     present on every other epoch.
 
     Parameters
     ----------
     keys_ignored : str or list of str (default=None)
-      Key or list of keys that should not be part of the printed
-      table. Note that in addition to the keys provided by the user,
-      keys such as those starting with 'event_' or ending on '_best'
-      are ignored by default.
+      Key or list of keys that should not be part of the printed table. Note
+      that in addition to the keys provided by the user, keys such as those
+      starting with ``'event_'`` or ending on ``'_best'`` are ignored by
+      default.
 
     sink : callable (default=print)
       The target that the output string is sent to. By default, the
       output is printed to stdout, but the sink could also be a
       logger, etc.
 
     tablefmt : str (default='simple')
@@ -583,15 +665,15 @@
     def on_epoch_end(self, net, **kwargs):
         self.pbar_.close()
 
     def __getstate__(self):
         # don't save away the temporary pbar_ object which gets created on
         # epoch begin anew anyway. This avoids pickling errors with tqdm.
         state = self.__dict__.copy()
-        del state['pbar_']
+        state.pop('pbar_', None)
         return state
 
 
 def rename_tensorboard_key(key):
     """Rename keys from history to keys in TensorBoard
 
     Specifically, prefixes all names with "Loss/" if they seem to be
@@ -602,63 +684,72 @@
         key = 'Loss/' + key
     return key
 
 
 class TensorBoard(Callback):
     """Logs results from history to TensorBoard
 
-    "TensorBoard provides the visualization and tooling needed for
-    machine learning experimentation" (tensorboard_)
+    "TensorBoard provides the visualization and tooling needed for machine
+    learning experimentation" (`offical docs
+    <https://www.tensorflow.org/tensorboard/>`_).
 
-    Use this callback to automatically log all interesting values from
-    your net's history to tensorboard after each epoch.
+    Use this callback to automatically log all interesting values from your
+    net's history to tensorboard after each epoch.
+
+    Examples
+    --------
+    Here is the standard way of using the callback:
+
+    >>> # Example: normal usage
+    >>> from skorch.callbacks import TensorBoard
+    >>> from torch.utils.tensorboard import SummaryWriter
+    >>> writer = SummaryWriter(...)
+    >>> net = NeuralNet(..., callbacks=[TensorBoard(writer)])
+    >>> net.fit(X, y)
 
     The best way to log additional information is to subclass this
     callback and add your code to one of the ``on_*`` methods.
 
-    Examples
-    --------
-    >>> # Example to log the bias parameter as a histogram
+    >>> # Example: log the bias parameter as a histogram
     >>> def extract_bias(module):
     ...     return module.hidden.bias
-
+    >>> # override on_epoch_end
     >>> class MyTensorBoard(TensorBoard):
     ...     def on_epoch_end(self, net, **kwargs):
     ...         bias = extract_bias(net.module_)
     ...         epoch = net.history[-1, 'epoch']
     ...         self.writer.add_histogram('bias', bias, global_step=epoch)
     ...         super().on_epoch_end(net, **kwargs)  # call super last
+    >>> # other code
+    >>> net = NeuralNet(..., callbacks=[MyTensorBoard(writer)])
 
     Parameters
     ----------
     writer : torch.utils.tensorboard.writer.SummaryWriter
       Instantiated ``SummaryWriter`` class.
 
     close_after_train : bool (default=True)
       Whether to close the ``SummaryWriter`` object once training
       finishes. Set this parameter to False if you want to continue
       logging with the same writer or if you use it as a context
       manager.
 
     keys_ignored : str or list of str (default=None)
-      Key or list of keys that should not be logged to
-      tensorboard. Note that in addition to the keys provided by the
-      user, keys such as those starting with 'event_' or ending on
-      '_best' are ignored by default.
+      Key or list of keys that should not be logged to tensorboard. Note that in
+      addition to the keys provided by the user, keys such as those starting
+      with ``'event_'`` or ending on ``'_best'`` are ignored by default.
 
     key_mapper : callable or function (default=rename_tensorboard_key)
       This function maps a key name from the history to a tag in
       tensorboard. This is useful because tensorboard can
       automatically group similar tags if their names start with the
       same prefix, followed by a forward slash. By default, this
       callback will prefix all keys that start with "train" or "valid"
       with the "Loss/" prefix.
 
-    .. _tensorboard: https://www.tensorflow.org/tensorboard/
-
     """
     def __init__(
             self,
             writer,
             close_after_train=True,
             keys_ignored=None,
             key_mapper=rename_tensorboard_key,
@@ -724,7 +815,335 @@
         for key in filter_log_keys(hist, keys_ignored=self.keys_ignored_):
             tag = self.key_mapper(key)
             self.add_scalar_maybe(history, key=key, tag=tag, global_step=epoch)
 
     def on_train_end(self, net, **kwargs):
         if self.close_after_train:
             self.writer.close()
+
+
+class SacredLogger(Callback):
+    """Logs results from history to Sacred.
+
+    Sacred is a tool to help you configure, organize, log and reproduce
+    experiments. Developed at IDSIA. See https://github.com/IDSIA/sacred.
+
+    Use this callback to automatically log all interesting values from
+    your net's history to Sacred.
+
+    If you want to log additional information, you can simply add it to
+    ``History``. See the documentation on ``Callbacks``, and ``Scoring`` for
+    more information. Alternatively you can subclass this callback and extend
+    the ``on_*`` methods.
+
+    To use this logger, you first have to install Sacred:
+
+    .. code-block:: bash
+
+        python -m pip install sacred
+
+    You might also install pymongo to use a mongodb backend. See the `upstream
+    documentation <https://github.com/IDSIA/sacred#installing>`_ for more
+    details. Once you have installed it, you can set up a simple experiment and
+    pass this Logger as a callback to your skorch estimator:
+
+    Examples
+    --------
+    >>> # contents of sacred-experiment.py
+    >>> import numpy as np
+    >>> from sacred import Experiment
+    >>> from sklearn.datasets import make_classification
+    >>> from skorch.callbacks.logging import SacredLogger
+    >>> from skorch.callbacks.scoring import EpochScoring
+    >>> from skorch import NeuralNetClassifier
+    >>> from skorch.toy import make_classifier
+    >>> ex = Experiment()
+    >>> @ex.config
+    >>> def my_config():
+    ...     max_epochs = 20
+    ...     lr = 0.01
+    >>> X, y = make_classification()
+    >>> X, y = X.astype(np.float32), y.astype(np.int64)
+    >>> @ex.automain
+    >>> def main(_run, max_epochs, lr):
+    ...     # Take care to add additional scoring callbacks *before* the logger.
+    ...     net = NeuralNetClassifier(
+    ...         make_classifier(),
+    ...         max_epochs=max_epochs,
+    ...         lr=0.01,
+    ...         callbacks=[EpochScoring("f1"), SacredLogger(_run)]
+    ...     )
+    ...     # now fit your estimator to your data
+    ...     net.fit(X, y)
+
+    Then call this from the command line, e.g. like this:
+
+    .. code-block:: bash
+
+        python sacred-script.py with max_epochs=15
+
+    You can also change other options on the command line and optionally
+    specify a backend.
+
+    Parameters
+    ----------
+    experiment : sacred.Experiment
+      Instantiated ``Experiment`` class.
+
+    log_on_batch_end : bool (default=False)
+      Whether to log loss and other metrics on batch level.
+
+    log_on_epoch_end : bool (default=True)
+      Whether to log loss and other metrics on epoch level.
+
+    batch_suffix : str (default=None)
+      A string that will be appended to all logged keys. By default (if set to
+      ``None``) "_batch" is used if batch and epoch logging are both enabled
+      and no suffix is used otherwise.
+
+    epoch_suffix : str (default=None)
+      A string that will be appended to all logged keys. By default (if set to
+      ``None``) "_epoch" is used if batch and epoch logging are both enabled
+      and no suffix is used otherwise.
+
+    keys_ignored : str or list of str (default=None)
+      Key or list of keys that should not be logged to Sacred. Note that in
+      addition to the keys provided by the user, keys such as those starting
+      with ``'event_'`` or ending on ``'_best'`` are ignored by default.
+
+    """
+
+    def __init__(
+        self,
+        experiment,
+        log_on_batch_end=False,
+        log_on_epoch_end=True,
+        batch_suffix=None,
+        epoch_suffix=None,
+        keys_ignored=None,
+    ):
+        self.experiment = experiment
+        self.log_on_batch_end = log_on_batch_end
+        self.log_on_epoch_end = log_on_epoch_end
+        self.batch_suffix = batch_suffix
+        self.epoch_suffix = epoch_suffix
+        self.keys_ignored = keys_ignored
+
+    def initialize(self):
+        keys_ignored = self.keys_ignored
+        if isinstance(keys_ignored, str):
+            keys_ignored = [keys_ignored]
+        self.keys_ignored_ = set(keys_ignored or [])
+        self.keys_ignored_.add("batches")
+
+        self.batch_suffix_ = self.batch_suffix
+        self.epoch_suffix_ = self.epoch_suffix
+        if self.batch_suffix_ is None:
+            self.batch_suffix_ = (
+                "_batch" if self.log_on_batch_end and self.log_on_epoch_end else ""
+            )
+        if self.epoch_suffix_ is None:
+            self.epoch_suffix_ = (
+                "_epoch" if self.log_on_batch_end and self.log_on_epoch_end else ""
+            )
+        return self
+
+    def on_batch_end(self, net, **kwargs):
+        if not self.log_on_batch_end:
+            return
+        batch_logs = net.history[-1]["batches"][-1]
+
+        for key in filter_log_keys(batch_logs.keys(), self.keys_ignored_):
+            # skorch does not keep a batch count, but sacred will
+            # automatically associate the results with a counter.
+            self.experiment.log_scalar(key + self.batch_suffix_, batch_logs[key])
+
+    def on_epoch_end(self, net, **kwargs):
+        """Automatically log values from the last history step."""
+        if not self.log_on_epoch_end:
+            return
+        epoch_logs = net.history[-1]
+        epoch = epoch_logs["epoch"]
+
+        for key in filter_log_keys(epoch_logs.keys(), self.keys_ignored_):
+            self.experiment.log_scalar(key + self.epoch_suffix_, epoch_logs[key], epoch)
+
+
+class MlflowLogger(Callback):
+    """Logs results from history and artifact to Mlflow
+
+    "MLflow is an open source platform for managing
+    the end-to-end machine learning lifecycle" (:doc:`mlflow:index`)
+
+    Use this callback to automatically log your metrics
+    and create/log artifacts to mlflow.
+
+    The best way to log additional information is to log directly to the
+    experiment object or subclass the ``on_*`` methods.
+
+    To use this logger, you first have to install Mlflow:
+
+    .. code-block::
+
+      $ python -m pip install mlflow
+
+    Examples
+    --------
+
+    Mlflow :doc:`fluent API <mlflow:python_api/mlflow>`:
+
+    >>> import mlflow
+    >>> net = NeuralNetClassifier(net, callbacks=[MLflowLogger()])
+    >>> with mlflow.start_run():
+    ...     net.fit(X, y)
+
+    Custom :py:class:`run <mlflow.entities.Run>` and
+    :py:class:`client <mlflow.tracking.MlflowClient>`:
+
+    >>> from mlflow.tracking import MlflowClient
+    >>> client = MlflowClient()
+    >>> experiment = client.get_experiment_by_name('Default')
+    >>> run = client.create_run(experiment.experiment_id)
+    >>> net = NeuralNetClassifier(..., callbacks=[MlflowLogger(run, client)])
+    >>> net.fit(X, y)
+
+    Parameters
+    ----------
+
+    run : mlflow.entities.Run (default=None)
+      Instantiated :py:class:`mlflow.entities.Run` class.
+      By default (if set to ``None``),
+      :py:func:`mlflow.active_run` is used to get the current run.
+
+    client : mlflow.tracking.MlflowClient (default=None)
+      Instantiated :py:class:`mlflow.tracking.MlflowClient` class.
+      By default (if set to ``None``),
+      ``MlflowClient()`` is used, which by default has:
+
+      - the tracking URI set by :py:func:`mlflow.set_tracking_uri`
+      - the registry URI set by :py:func:`mlflow.set_registry_uri`
+
+    create_artifact : bool (default=True)
+      Whether to create artifacts for the network's
+      params, optimizer, criterion and history.
+      See :ref:`save_load`
+
+    terminate_after_train : bool (default=True)
+      Whether to terminate the ``Run`` object once training finishes.
+
+    log_on_batch_end : bool (default=False)
+      Whether to log loss and other metrics on batch level.
+
+    log_on_epoch_end : bool (default=True)
+      Whether to log loss and other metrics on epoch level.
+
+    batch_suffix : str (default=None)
+      A string that will be appended to all logged keys. By default (if set to
+      ``None``) ``'_batch'`` is used if batch and epoch logging are both enabled
+      and no suffix is used otherwise.
+
+    epoch_suffix : str (default=None)
+      A string that will be appended to all logged keys. By default (if set to
+      ``None``) ``'_epoch'`` is used if batch and epoch logging are both enabled
+      and no suffix is used otherwise.
+
+    keys_ignored : str or list of str (default=None)
+      Key or list of keys that should not be logged to Mlflow. Note that in
+      addition to the keys provided by the user, keys such as those starting
+      with ``'event_'`` or ending on ``'_best'`` are ignored by default.
+    """
+    def __init__(
+        self,
+        run=None,
+        client=None,
+        create_artifact=True,
+        terminate_after_train=True,
+        log_on_batch_end=False,
+        log_on_epoch_end=True,
+        batch_suffix=None,
+        epoch_suffix=None,
+        keys_ignored=None,
+    ):
+        self.run = run
+        self.client = client
+        self.create_artifact = create_artifact
+        self.terminate_after_train = terminate_after_train
+        self.log_on_batch_end = log_on_batch_end
+        self.log_on_epoch_end = log_on_epoch_end
+        self.batch_suffix = batch_suffix
+        self.epoch_suffix = epoch_suffix
+        self.keys_ignored = keys_ignored
+
+    def initialize(self):
+        self.run_ = self.run
+        if self.run_ is None:
+            import mlflow
+            self.run_ = mlflow.active_run()
+        self.client_ = self.client
+        if self.client_ is None:
+            from mlflow.tracking import MlflowClient
+            self.client_ = MlflowClient()
+        keys_ignored = self.keys_ignored
+        if isinstance(keys_ignored, str):
+            keys_ignored = [keys_ignored]
+        self.keys_ignored_ = set(keys_ignored or [])
+        self.keys_ignored_.add('batches')
+        self.batch_suffix_ = self._init_suffix(self.batch_suffix, '_batch')
+        self.epoch_suffix_ = self._init_suffix(self.epoch_suffix, '_epoch')
+        return self
+
+    def _init_suffix(self, suffix, default):
+        if suffix is not None:
+            return suffix
+        return default if self.log_on_batch_end and self.log_on_epoch_end else ''
+
+    def on_train_begin(self, net, **kwargs):
+        self._batch_count = 0
+
+    def on_batch_end(self, net, training, **kwargs):
+        if not self.log_on_batch_end:
+            return
+        self._batch_count += 1
+        batch_logs = net.history[-1]['batches'][-1]
+        self._iteration_log(batch_logs, self.batch_suffix_, self._batch_count)
+
+    def on_epoch_end(self, net, **kwargs):
+        if not self.log_on_epoch_end:
+            return
+        epoch_logs = net.history[-1]
+        self._iteration_log(epoch_logs, self.epoch_suffix_, len(net.history))
+
+    def _iteration_log(self, logs, suffix, step):
+        for key in filter_log_keys(logs.keys(), self.keys_ignored_):
+            self.client_.log_metric(
+                self.run_.info.run_id,
+                key + suffix,
+                logs[key],
+                step=step,
+            )
+
+    def on_train_end(self, net, **kwargs):
+        try:
+            self._log_artifacts(net)
+        finally:
+            if self.terminate_after_train:
+                self.client_.set_terminated(self.run_.info.run_id)
+
+    def _log_artifacts(self, net):
+        if not self.create_artifact:
+            return
+        with tempfile.TemporaryDirectory(prefix='skorch_mlflow_logger_') as dirpath:
+            dirpath = Path(dirpath)
+            params_filepath = dirpath / 'params.pth'
+            optimizer_filepath = dirpath / 'optimizer.pth'
+            criterion_filepath = dirpath / 'criterion.pth'
+            history_filepath = dirpath / 'history.json'
+            net.save_params(
+                f_params=params_filepath,
+                f_optimizer=optimizer_filepath,
+                f_criterion=criterion_filepath,
+                f_history=history_filepath,
+            )
+            self.client_.log_artifact(self.run_.info.run_id, params_filepath)
+            self.client_.log_artifact(self.run_.info.run_id, optimizer_filepath)
+            self.client_.log_artifact(self.run_.info.run_id, criterion_filepath)
+            self.client_.log_artifact(self.run_.info.run_id, history_filepath)
```

### Comparing `skorch-0.9.0/skorch/callbacks/lr_scheduler.py` & `skorch-1.0.0/skorch/callbacks/lr_scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,20 @@
 # pylint: disable=unused-import
 import warnings
 
 import numpy as np
 import torch
 from torch.optim.lr_scheduler import _LRScheduler
 from torch.optim.lr_scheduler import CosineAnnealingLR
+from torch.optim.lr_scheduler import CyclicLR
 from torch.optim.lr_scheduler import ExponentialLR
 from torch.optim.lr_scheduler import LambdaLR
 from torch.optim.lr_scheduler import MultiStepLR
 from torch.optim.lr_scheduler import ReduceLROnPlateau
 from torch.optim.lr_scheduler import StepLR
-
-try:
-    from torch.optim.lr_scheduler import CyclicLR as TorchCyclicLR
-except ImportError:
-    # Backward compatibility with torch >= 1.0 && < 1.1
-    TorchCyclicLR = None
 from torch.optim.optimizer import Optimizer
 from skorch.callbacks import Callback
 
 __all__ = ['LRScheduler', 'WarmRestartLR']
 
 
 def _check_lr(name, optimizer, lr):
@@ -111,24 +106,14 @@
 
         return np.array(lrs)
 
     def initialize(self):
         self.policy_ = self._get_policy_cls()
         self.lr_scheduler_ = None
         self.batch_idx_ = 0
-        # TODO: Remove this warning on 0.10 release
-        if (self.policy_ == TorchCyclicLR or self.policy_ == "TorchCyclicLR"
-                and self.step_every == 'epoch'):
-            warnings.warn(
-                "The LRScheduler now makes a step every epoch by default. "
-                "To have the cyclic lr scheduler update "
-                "every batch set step_every='batch'",
-                FutureWarning
-            )
-
         return self
 
     def _get_policy_cls(self):
         if isinstance(self.policy, str):
             return getattr(sys.modules[__name__], self.policy)
         return self.policy
 
@@ -148,54 +133,85 @@
                 self.batch_idx_ = sum(net.history[:, 'train_batch_count'])
             except KeyError:
                 self.batch_idx_ = sum(len(b) for b in net.history[:, 'batches'])
         self.lr_scheduler_ = self._get_scheduler(
             net, self.policy_, **self.kwargs
         )
 
+    def _step(self, net, lr_scheduler, score=None):
+        """Helper method to step the lr scheduler.
+
+        This takes care of two things:
+
+        1. If the lr scheduler is ReduceLROnPlateau, we need to pass the score.
+        2. If the net is uses AccelerateMixin, stepping has to be skipped in
+           certain conditions.
+
+        For more info on the latter, see:
+        https://huggingface.co/docs/accelerate/quicktour#mixed-precision-training
+
+        """
+        accelerator_maybe = getattr(net, 'accelerator', None)
+        accelerator_step_skipped = (
+            accelerator_maybe and accelerator_maybe.optimizer_step_was_skipped
+        )
+        if accelerator_step_skipped:
+            return
+
+        if score is None:
+            lr_scheduler.step()
+        else:
+            lr_scheduler.step(score)
+
     def on_epoch_end(self, net, **kwargs):
-        if not self.step_every == 'epoch':
+        if self.step_every != 'epoch':
             return
-        epoch = len(net.history)
         if isinstance(self.lr_scheduler_, ReduceLROnPlateau):
             if callable(self.monitor):
                 score = self.monitor(net)
             else:
-                if self.lr_scheduler_.mode == 'max':
-                    score = -np.inf
-                elif self.lr_scheduler_.mode == 'min':
-                    score = np.inf
-                else:
+                try:
                     score = net.history[-1, self.monitor]
+                except KeyError as e:
+                    raise ValueError(
+                        f"'{self.monitor}' was not found in history. A "
+                        f"Scoring callback with name='{self.monitor}' "
+                        "should be placed before the LRScheduler callback"
+                    ) from e
 
-            self.lr_scheduler_.step(score, epoch)
+            self._step(net, self.lr_scheduler_, score=score)
             # ReduceLROnPlateau does not expose the current lr so it can't be recorded
         else:
-            if self.event_name is not None and hasattr(
-                    self.lr_scheduler_, "get_last_lr"):
-                net.history.record(self.event_name,
-                                   self.lr_scheduler_.get_last_lr()[0])
-            self.lr_scheduler_.step(epoch)
+            if (
+                    (self.event_name is not None)
+                    and hasattr(self.lr_scheduler_, "get_last_lr")
+            ):
+                net.history.record(self.event_name, self.lr_scheduler_.get_last_lr()[0])
+            self._step(net, self.lr_scheduler_)
 
     def on_batch_end(self, net, training, **kwargs):
-        if not training or not self.step_every == 'batch':
+        if not training or self.step_every != 'batch':
             return
-        if self.event_name is not None and hasattr(
-                self.lr_scheduler_, "get_last_lr"):
-            net.history.record_batch(self.event_name,
-                                     self.lr_scheduler_.get_last_lr()[0])
-        self.lr_scheduler_.step()
+        if (
+                (self.event_name is not None)
+                and hasattr(self.lr_scheduler_, "get_last_lr")
+        ):
+            net.history.record_batch(
+                self.event_name, self.lr_scheduler_.get_last_lr()[0])
+        self._step(net, self.lr_scheduler_)
         self.batch_idx_ += 1
 
     def _get_scheduler(self, net, policy, **scheduler_kwargs):
         """Return scheduler, based on indicated policy, with appropriate
         parameters.
         """
-        if policy not in [ReduceLROnPlateau] and \
-                'last_epoch' not in scheduler_kwargs:
+        if (
+                (policy not in [ReduceLROnPlateau])
+                and ('last_epoch' not in scheduler_kwargs)
+        ):
             last_epoch = len(net.history) - 1
             scheduler_kwargs['last_epoch'] = last_epoch
 
         return policy(net.optimizer_, **scheduler_kwargs)
 
 
 class WarmRestartLR(_LRScheduler):
@@ -249,15 +265,15 @@
         self.max_lr = _check_lr('max_lr', optimizer, max_lr)
         self.base_period = base_period
         self.period_mult = period_mult
         super(WarmRestartLR, self).__init__(optimizer, last_epoch)
 
     def _get_current_lr(self, min_lr, max_lr, period, epoch):
         return min_lr + 0.5 * (max_lr - min_lr) * (
-                1 + np.cos(epoch * np.pi / period))
+            1 + np.cos(epoch * np.pi / period))
 
     def get_lr(self):
         epoch_idx = float(self.last_epoch)
         current_period = float(self.base_period)
         while epoch_idx / current_period > 1.0:
             epoch_idx -= current_period + 1
             current_period *= self.period_mult
```

### Comparing `skorch-0.9.0/skorch/callbacks/regularization.py` & `skorch-1.0.0/skorch/callbacks/regularization.py`

 * *Files identical despite different names*

### Comparing `skorch-0.9.0/skorch/callbacks/scoring.py` & `skorch-1.0.0/skorch/callbacks/scoring.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 """ Callbacks for calculating scores."""
 
 from contextlib import contextmanager
 from contextlib import suppress
-from distutils.version import LooseVersion
 from functools import partial
 import warnings
 
 import numpy as np
 import sklearn
 from sklearn.metrics import make_scorer, check_scoring
 
-if LooseVersion(sklearn.__version__) >= '0.22':
-    from sklearn.metrics._scorer import _BaseScorer
-else:
-    from sklearn.metrics.scorer import _BaseScorer
-
+from skorch.callbacks import Callback
+from skorch.dataset import unpack_data
+from sklearn.metrics._scorer import _BaseScorer
 from skorch.utils import data_from_dataset
 from skorch.utils import is_skorch_dataset
 from skorch.utils import to_numpy
-from skorch.callbacks import Callback
 from skorch.utils import check_indexing
 from skorch.utils import to_device
 
 
 __all__ = ['BatchScoring', 'EpochScoring', 'PassthroughScoring']
 
 
@@ -33,14 +29,15 @@
     Returns a modified version of the net whose ``infer`` method will
     subsequently return cached predictions. Leaving the context will
     undo the overwrite of the ``infer`` method.
 
     Deprecated.
 
     """
+    # TODO: remove this function
 
     warnings.warn(
         "cache_net_infer is no longer uesd to provide caching for "
         "the scoring callbacks and will hence be removed in a "
         "future release.",
         DeprecationWarning,
     )
@@ -64,15 +61,20 @@
 def _cache_net_forward_iter(net, use_caching, y_preds):
     """Caching context for ``skorch.NeuralNet`` instance.
 
     Returns a modified version of the net whose ``forward_iter``
     method will subsequently return cached predictions. Leaving the
     context will undo the overwrite of the ``forward_iter`` method.
 
+    Note that the net may override the use of caching.
+
     """
+    if net.use_caching != 'auto':
+        use_caching = net.use_caching
+
     if not use_caching:
         yield net
         return
     y_preds = iter(y_preds)
 
     # pylint: disable=unused-argument
     def cached_forward_iter(*args, device=net.device, **kwargs):
@@ -94,15 +96,15 @@
     """If ``scoring`` is a sklearn metric function, convert it to a
     sklearn scorer and return it. Otherwise, return ``scoring`` unchanged."""
     if callable(scoring):
         module = getattr(scoring, '__module__', None)
 
         # those are scoring objects returned by make_scorer starting
         # from sklearn 0.22
-        scorer_names = ('_PredictScorer', '_ProbaScorer', '_ThresholdScorer')
+        scorer_names = ('_PredictScorer', '_ProbaScorer', '_ThresholdScorer', '_Scorer')
         if (
                 hasattr(module, 'startswith') and
                 module.startswith('sklearn.metrics.') and
                 not module.startswith('sklearn.metrics.scorer') and
                 not module.startswith('sklearn.metrics.tests.') and
                 not scoring.__class__.__name__ in scorer_names
         ):
@@ -142,17 +144,16 @@
             return self.scoring_
         if isinstance(self.scoring_, partial):
             return self.scoring_.func.__name__
         if isinstance(self.scoring_, _BaseScorer):
             if hasattr(self.scoring_._score_func, '__name__'):
                 # sklearn < 0.22
                 return self.scoring_._score_func.__name__
-            else:
-                # sklearn >= 0.22
-                return self.scoring_._score_func._score_func.__name__
+            # sklearn >= 0.22
+            return self.scoring_._score_func._score_func.__name__
         if isinstance(self.scoring_, dict):
             raise ValueError("Dict not supported as scorer for multi-metric scoring."
                              " Register multiple scoring callbacks instead.")
         return self.scoring_.__name__
 
     def initialize(self):
         self.best_score_ = np.inf if self.lower_is_better else -np.inf
@@ -230,23 +231,25 @@
 
     target_extractor : callable (default=to_numpy)
       This is called on y before it is passed to scoring.
 
     use_caching : bool (default=True)
       Re-use the model's prediction for computing the loss to calculate
       the score. Turning this off will result in an additional inference
-      step for each batch.
+      step for each batch. Note that the net may override the use of
+      caching.
 
     """
     # pylint: disable=unused-argument,arguments-differ
 
-    def on_batch_end(self, net, X, y, training, **kwargs):
+    def on_batch_end(self, net, batch, training, **kwargs):
         if training != self.on_train:
             return
 
+        X, y = unpack_data(batch)
         y_preds = [kwargs['y_pred']]
         with _cache_net_forward_iter(net, self.use_caching, y_preds) as cached_net:
             # In case of y=None we will not have gathered any samples.
             # We expect the scoring function to deal with y=None.
             y = None if y is None else self.target_extractor(y)
             try:
                 score = self._scoring(cached_net, X, y)
@@ -345,15 +348,15 @@
       Collect labels and predictions (``y_true`` and ``y_pred``)
       over the course of one epoch and use the cached values for
       computing the score. The cached values are shared between
       all ``EpochScoring`` instances. Disabling this will result
       in an additional inference step for each epoch and an
       inability to use arbitrary datasets as input (since we
       don't know how to extract ``y_true`` from an arbitrary
-      dataset).
+      dataset). Note that the net may override the use of caching.
 
     """
     def _initialize_cache(self):
         self.y_trues_ = []
         self.y_preds_ = []
 
     def initialize(self):
@@ -363,44 +366,52 @@
 
     # pylint: disable=arguments-differ,unused-argument
     def on_epoch_begin(self, net, dataset_train, dataset_valid, **kwargs):
         self._initialize_cache()
 
     # pylint: disable=arguments-differ
     def on_batch_end(
-            self, net, y, y_pred, training, **kwargs):
-        if not self.use_caching or training != self.on_train:
+            self, net, batch, y_pred, training, **kwargs):
+        use_caching = self.use_caching
+        if net.use_caching !=  'auto':
+            use_caching = net.use_caching
+
+        if (not use_caching) or (training != self.on_train):
             return
 
         # We collect references to the prediction and target data
         # emitted by the training process. Since we don't copy the
         # data, all *Scoring callback instances use the same
         # underlying data. This is also the reason why we don't run
         # self.target_extractor(y) here but on epoch end, so that
         # there are no copies of parts of y hanging around during
         # training.
+        _X, y = unpack_data(batch)
         if y is not None:
             self.y_trues_.append(y)
         self.y_preds_.append(y_pred)
 
-    def get_test_data(self, dataset_train, dataset_valid):
+    def get_test_data(self, dataset_train, dataset_valid, use_caching):
         """Return data needed to perform scoring.
 
         This is a convenience method that handles picking of
         train/valid, different types of input data, use of cache,
         etc. for you.
 
         Parameters
         ----------
         dataset_train
           Incoming training data or dataset.
 
         dataset_valid
           Incoming validation data or dataset.
 
+        use_caching : bool
+          Whether caching of inference is being used.
+
         Returns
         -------
         X_test
           Input data used for making the prediction.
 
         y_test
           Target ground truth. If caching was enabled, return cached
@@ -412,15 +423,15 @@
           of the predictions. It may thus be necessary to concatenate
           the output before working with it:
           ``y_pred = np.concatenate(y_pred)``
 
         """
         dataset = dataset_train if self.on_train else dataset_valid
 
-        if self.use_caching:
+        if use_caching:
             X_test = dataset
             y_pred = self.y_preds_
             y_test = [self.target_extractor(y) for y in self.y_trues_]
             # In case of y=None we will not have gathered any samples.
             # We expect the scoring function to deal with y_test=None.
             y_test = np.concatenate(y_test) if y_test else None
             return X_test, y_test, y_pred
@@ -458,15 +469,23 @@
     # pylint: disable=unused-argument,arguments-differ
     def on_epoch_end(
             self,
             net,
             dataset_train,
             dataset_valid,
             **kwargs):
-        X_test, y_test, y_pred = self.get_test_data(dataset_train, dataset_valid)
+        use_caching = self.use_caching
+        if net.use_caching !=  'auto':
+            use_caching = net.use_caching
+
+        X_test, y_test, y_pred = self.get_test_data(
+            dataset_train,
+            dataset_valid,
+            use_caching=use_caching,
+        )
         if X_test is None:
             return
 
         with _cache_net_forward_iter(net, self.use_caching, y_pred) as cached_net:
             current_score = self._scoring(cached_net, X_test, y_test)
 
         self._record_score(net.history, current_score)
```

### Comparing `skorch-0.9.0/skorch/callbacks/training.py` & `skorch-1.0.0/skorch/callbacks/training.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,41 +3,48 @@
 import os
 import pickle
 import warnings
 from contextlib import suppress
 from fnmatch import fnmatch
 from functools import partial
 from itertools import product
+from copy import deepcopy
 
 import numpy as np
 from skorch.callbacks import Callback
 from skorch.exceptions import SkorchException
 from skorch.utils import _check_f_arguments
 from skorch.utils import noop
 from skorch.utils import open_file_like
 from skorch.utils import freeze_parameter
 from skorch.utils import unfreeze_parameter
 
 
 __all__ = ['Checkpoint', 'EarlyStopping', 'ParamMapper', 'Freezer',
-           'Unfreezer', 'Initializer', 'LoadInitState', 'TrainEndCheckpoint']
+           'Unfreezer', 'Initializer', 'InputShapeSetter', 'LoadInitState',
+           'TrainEndCheckpoint']
 
 
 class Checkpoint(Callback):
     """Save the model during training if the given metric improved.
 
     This callback works by default in conjunction with the validation
     scoring callback since it creates a ``valid_loss_best`` value
     in the history which the callback uses to determine if this
     epoch is save-worthy.
 
     You can also specify your own metric to monitor or supply a
     callback that dynamically evaluates whether the model should
     be saved in this epoch.
 
+    As checkpointing is often used in conjunction with early stopping
+    there is a need to restore the state of the model to the best
+    checkpoint after training is done. The checkpoint callback will
+    do this for you if you wish.
+
     Some or all of the following can be saved:
 
       - model parameters (see ``f_params`` parameter);
       - optimizer state (see ``f_optimizer`` parameter);
       - criterion state (see ``f_criterion`` parameter);
       - training history (see ``f_history`` parameter);
       - entire model object (see ``f_pickle`` parameter).
@@ -128,56 +135,84 @@
       Pass ``None`` to disable placing events in history.
 
     sink : callable (default=noop)
       The target that the information about created checkpoints is
       sent to. This can be a logger or ``print`` function (to send to
       stdout). By default the output is discarded.
 
+    load_best: bool (default=False)
+      Load the best checkpoint automatically once training ended.
+      This can be particularly helpful in combination with early stopping
+      as it allows for scoring with the best model, even when early stopping
+      ended training a number of epochs later. Note that this will only
+      work when ``monitor != None``.
+
+    use_safetensors : bool (default=False)
+      Whether to use the ``safetensors`` library to persist the state. By
+      default, PyTorch is used, which in turn uses :mod:`pickle` under the
+      hood. When enabling ``safetensors``, be aware that only PyTorch
+      tensors can be stored. Therefore, certain attributes like the
+      optimizer cannot be saved.
+
     """
     def __init__(
             self,
             monitor='valid_loss_best',
             f_params='params.pt',
             f_optimizer='optimizer.pt',
             f_criterion='criterion.pt',
             f_history='history.json',
             f_pickle=None,
             fn_prefix='',
             dirname='',
             event_name='event_cp',
             sink=noop,
+            load_best=False,
+            use_safetensors=False,
             **kwargs
     ):
         self.monitor = monitor
         self.f_params = f_params
         self.f_optimizer = f_optimizer
         self.f_criterion = f_criterion
         self.f_history = f_history
         self.f_pickle = f_pickle
         self.fn_prefix = fn_prefix
         self.dirname = dirname
         self.event_name = event_name
         self.sink = sink
+        self.load_best = load_best
+        self.use_safetensors = use_safetensors
         self._check_kwargs(kwargs)
         vars(self).update(**kwargs)
         self._validate_filenames()
 
     def _check_kwargs(self, kwargs):
         for key in kwargs:
             if not key.startswith('f_'):
                 raise TypeError(
                     "{cls_name} got an unexpected argument '{key}', did you mean "
                     "'f_{key}'?".format(cls_name=self.__class__.__name__, key=key))
+        if self.use_safetensors and self.f_optimizer is not None:
+            raise ValueError(
+                "Cannot save optimizer state when using safetensors, "
+                "please set f_optimizer=None or don't use safetensors.")
 
     def initialize(self):
         self._validate_filenames()
         if self.dirname and not os.path.exists(self.dirname):
             os.makedirs(self.dirname, exist_ok=True)
         return self
 
+    def on_train_end(self, net, **kwargs):
+        if not self.load_best or self.monitor is None:
+            return
+        self._sink("Loading best checkpoint after training.", net.verbose)
+        net.load_params(checkpoint=self, use_safetensors=self.use_safetensors)
+
     def on_epoch_end(self, net, **kwargs):
         if "{}_best".format(self.monitor) in net.history[-1]:
             warnings.warn(
                 "Checkpoint monitor parameter is set to '{0}' and the history "
                 "contains '{0}_best'. Perhaps you meant to set the parameter "
                 "to '{0}_best'".format(self.monitor), UserWarning)
 
@@ -185,18 +220,18 @@
             do_checkpoint = True
         elif callable(self.monitor):
             do_checkpoint = self.monitor(net)
         else:
             try:
                 do_checkpoint = net.history[-1, self.monitor]
             except KeyError as e:
-                raise SkorchException(
-                    "Monitor value '{}' cannot be found in history. "
-                    "Make sure you have validation data if you use "
-                    "validation scores for checkpointing.".format(e.args[0]))
+                msg = (
+                    f"{e.args[0]} Make sure you have validation data if you use "
+                    "validation scores for checkpointing.")
+                raise SkorchException(msg)
 
         if self.event_name is not None:
             net.history.record(self.event_name, bool(do_checkpoint))
 
         if do_checkpoint:
             self.save_model(net)
             self._sink("A checkpoint was triggered in epoch {}.".format(
@@ -264,15 +299,15 @@
                     idx = i
 
         return {key: self._format_target(net, val, idx) for key, val
                 in self._f_kwargs().items()}
 
     def _save_params(self, f, net, f_name, log_name):
         try:
-            net.save_params(**{f_name: f})
+            net.save_params(**{f_name: f, 'use_safetensors': self.use_safetensors})
         except Exception as e:  # pylint: disable=broad-except
             self._sink(
                 "Unable to save {} to {}, {}: {}".format(
                     log_name, f, type(e).__name__, e), net.verbose)
 
     def _format_target(self, net, f, idx):
         """Apply formatting to the target filename template."""
@@ -342,55 +377,85 @@
         score so far (relative)
 
     sink : callable (default=print)
       The target that the information about early stopping is
       sent to. By default, the output is printed to stdout, but the
       sink could also be a logger or :func:`~skorch.utils.noop`.
 
+    load_best: bool (default=False)
+      Whether to restore module weights from the epoch with the best value of
+      the monitored quantity. If False, the module weights obtained at the
+      last step of training are used. Note that only the module is restored.
+      Use the ``Checkpoint`` callback with the :attr:`~Checkpoint.load_best`
+      argument set to ``True`` if you need to restore the whole object.
+
     """
     def __init__(
             self,
             monitor='valid_loss',
             patience=5,
             threshold=1e-4,
             threshold_mode='rel',
             lower_is_better=True,
             sink=print,
+            load_best=False,
     ):
         self.monitor = monitor
         self.lower_is_better = lower_is_better
         self.patience = patience
         self.threshold = threshold
         self.threshold_mode = threshold_mode
         self.misses_ = 0
         self.dynamic_threshold_ = None
         self.sink = sink
+        self.load_best = load_best
+
+    def __getstate__(self):
+        # Avoids to save the module_ weights twice when pickling
+        state = self.__dict__.copy()
+        state['best_model_weights_'] = None
+        return state
 
     # pylint: disable=arguments-differ
     def on_train_begin(self, net, **kwargs):
         if self.threshold_mode not in ['rel', 'abs']:
             raise ValueError("Invalid threshold mode: '{}'"
                              .format(self.threshold_mode))
         self.misses_ = 0
         self.dynamic_threshold_ = np.inf if self.lower_is_better else -np.inf
+        self.best_model_weights_ = None
+        self.best_epoch_ = 0
 
     def on_epoch_end(self, net, **kwargs):
         current_score = net.history[-1, self.monitor]
         if not self._is_score_improved(current_score):
             self.misses_ += 1
         else:
             self.misses_ = 0
             self.dynamic_threshold_ = self._calc_new_threshold(current_score)
+            self.best_epoch_ = net.history[-1, "epoch"]
+            if self.load_best:
+                self.best_model_weights_ = deepcopy(net.module_.state_dict())
         if self.misses_ == self.patience:
             if net.verbose:
                 self._sink("Stopping since {} has not improved in the last "
                            "{} epochs.".format(self.monitor, self.patience),
                            verbose=net.verbose)
             raise KeyboardInterrupt
 
+    def on_train_end(self, net, **kwargs):
+        if (
+            self.load_best and (self.best_epoch_ != net.history[-1, "epoch"])
+            and (self.best_model_weights_ is not None)
+        ):
+            net.module_.load_state_dict(self.best_model_weights_)
+            self._sink("Restoring best model from epoch {}.".format(
+                self.best_epoch_
+            ), verbose=net.verbose)
+
     def _is_score_improved(self, score):
         if self.lower_is_better:
             return score < self.dynamic_threshold_
         return score > self.dynamic_threshold_
 
     def _calc_new_threshold(self, score):
         """Determine threshold based on score."""
@@ -508,15 +573,15 @@
                     'Invalid value for `at` (at={}). The first possible '
                     'epoch number is 1.'.format(self.at))
             self.at = partial(self._epoch_at, epoch=self.at)
 
         return self
 
     def named_parameters(self, net):
-        return net.module_.named_parameters()
+        return net.get_all_learnable_params()
 
     def filter_parameters(self, patterns, params):
         pattern_fns = (
             pattern if callable(pattern) else partial(fnmatch, pat=pattern)
             for pattern in patterns
         )
         for pattern_fn, (name, param) in product(pattern_fns, params):
@@ -603,33 +668,49 @@
     continue training from there.
 
     Parameters
     ----------
     checkpoint: :class:`.Checkpoint`
       Checkpoint to get filenames from.
 
+    use_safetensors : bool (default=False)
+      Whether to use the ``safetensors`` library to load the state. By default,
+      PyTorch is used, which in turn uses :mod:`pickle` under the hood. When the
+      state was saved using ``safetensors``, (e.g. by enabling it with the
+      :class:`.Checkpoint`), you should set this to ``True``.
+
     """
-    def __init__(self, checkpoint):
+    def __init__(self, checkpoint, use_safetensors=False):
         self.checkpoint = checkpoint
+        self.use_safetensors = use_safetensors
 
     def initialize(self):
         self.did_load_ = False
         return self
 
     def on_train_begin(self, net,
                        X=None, y=None, **kwargs):
         if not self.did_load_:
             self.did_load_ = True
-            with suppress(Exception):
-                net.load_params(checkpoint=self.checkpoint)
+            with suppress(FileNotFoundError):
+                if isinstance(self.checkpoint, TrainEndCheckpoint):
+                    net.load_params(
+                        checkpoint=self.checkpoint.checkpoint_,
+                        use_safetensors=self.use_safetensors
+                    )
+                else:
+                    net.load_params(
+                        checkpoint=self.checkpoint,
+                        use_safetensors=self.use_safetensors
+                    )
 
 
 class TrainEndCheckpoint(Callback):
     """Saves the model parameters, optimizer state, and history at the end of
-    training. The default ``fn_prefix`` is 'train_end_'.
+    training. The default ``fn_prefix`` is ``'train_end_'``.
 
     Examples
     --------
 
     Consider running the following example multiple times:
 
     >>> train_end_cp = TrainEndCheckpoint(dirname='exp1')
@@ -639,15 +720,14 @@
 
     After the first run, model parameters, optimizer state, and history are
     saved into a directory named `exp1`. On the next run, `LoadInitState` will
     load the state from the first run and continue training.
 
     Parameters
     ----------
-
     f_params : file-like object, str, None (default='params.pt')
       File path to the file or file-like object where the model
       parameters should be saved. Pass ``None`` to disable saving
       model parameters.
 
       If the value is a string you can also use format specifiers
       to, for example, indicate the current epoch. Accessible format
@@ -685,14 +765,21 @@
     fn_prefix: str (default='train_end_')
       Prefix for filenames. If ``f_params``, ``f_optimizer``, ``f_history``,
       or ``f_pickle`` are strings, they will be prefixed by ``fn_prefix``.
 
     dirname: str (default='')
       Directory where files are stored.
 
+    use_safetensors : bool (default=False)
+      Whether to use the ``safetensors`` library to persist the state. By
+      default, PyTorch is used, which in turn uses :mod:`pickle` under the
+      hood. When enabling ``safetensors``, be aware that only PyTorch
+      tensors can be stored. Therefore, certain attributes like the
+      optimizer cannot be saved.
+
     sink : callable (default=noop)
       The target that the information about created checkpoints is
       sent to. This can be a logger or ``print`` function (to send to
       stdout). By default the output is discarded.
 
     """
     def __init__(
@@ -700,24 +787,26 @@
             f_params='params.pt',
             f_optimizer='optimizer.pt',
             f_criterion='criterion.pt',
             f_history='history.json',
             f_pickle=None,
             fn_prefix='train_end_',
             dirname='',
+            use_safetensors=False,
             sink=noop,
             **kwargs
     ):
         self.f_params = f_params
         self.f_optimizer = f_optimizer
         self.f_criterion = f_criterion
         self.f_history = f_history
         self.f_pickle = f_pickle
         self.fn_prefix = fn_prefix
         self.dirname = dirname
+        self.use_safetensors = use_safetensors
         self.sink = sink
         Checkpoint._check_kwargs(self, kwargs)
         vars(self).update(**kwargs)
 
     def _f_kwargs(self):
         return {name: getattr(self, name) for name in dir(self)
                 if name.startswith('f_')}
@@ -725,17 +814,90 @@
     def initialize(self):
         self.checkpoint_ = Checkpoint(
             monitor=None,
             fn_prefix=self.fn_prefix,
             dirname=self.dirname,
             event_name=None,
             sink=self.sink,
+            use_safetensors=self.use_safetensors,
             **self._f_kwargs()
         )
         self.checkpoint_.initialize()
+        return self
 
     def on_train_end(self, net, **kwargs):
         self.checkpoint_.save_model(net)
         self.checkpoint_._sink("Final checkpoint triggered", net.verbose)
+        return self
+
+
+class InputShapeSetter(Callback):
+    """Sets the input dimension of the PyTorch module to the input dimension
+    of the training data. By default the last dimension of X (``X.shape[-1]``)
+    will be used.
+
+    This can be of use when the shape of X is not known beforehand,
+    e.g. when using a skorch model within an sklearn pipeline and
+    grid-searching feature transformers, or using feature selection
+    methods.
+
+    Basic usage:
+
+    >>> class MyModule(torch.nn.Module):
+    ...     def __init__(self, input_dim=1):
+    ...         super().__init__()
+    ...         self.layer = torch.nn.Linear(input_dim, 3)
+    ... # ...
+    >>> X1 = np.zeros(100, 5)
+    >>> X2 = np.zeros(100, 3)
+    >>> y = np.zeros(100)
+    >>> net = NeuralNetClassifier(MyModule, callbacks=[InputShapeSetter()])
+    >>> net.fit(X1, y)  # self.module_.layer.in_features == 5
+    >>> net.fit(X2, y)  # self.module_.layer.in_features == 3
+
+    Parameters
+    ----------
+    param_name : str (default='input_dim')
+      The parameter name is the parameter your model uses to define the
+      input dimension in its ``__init__`` method.
+
+    input_dim_fn : callable, None (default=None)
+      In case your ``X`` value is more complex and deriving the input
+      dimension is not as easy as ``X.shape[-1]`` you can pass a callable
+      to this parameter which takes ``X`` and returns the input dimension.
+
+    module_name : str (default='module')
+      Only needs change when you are using more than one module in your
+      skorch model (e.g., in case of GANs).
+    """
+    def __init__(
+        self,
+        param_name='input_dim',
+        input_dim_fn=None,
+        module_name='module',
+    ):
+        self.module_name = module_name
+        self.param_name = param_name
+        self.input_dim_fn = input_dim_fn
+
+    def get_input_dim(self, X):
+        if self.input_dim_fn is not None:
+            return self.input_dim_fn(X)
+        if len(X.shape) < 2:
+            raise ValueError(
+                "Expected at least two-dimensional input data for X. "
+                "If your data is one-dimensional, please use the "
+                "`input_dim_fn` parameter to infer the correct "
+                "input shape."
+            )
+        return X.shape[-1]
+
+    def on_train_begin(self, net, X, y, **kwargs):
+        params = net.get_params()
+        input_dim = self.get_input_dim(X)
+        param_name = f'{self.module_name}__{self.param_name}'
+
+        if params.get(param_name, None) == input_dim:
+            return
 
-    def __getattr__(self, attr):
-        return getattr(self.checkpoint_, attr)
+        kwargs = {param_name: input_dim}
+        net.set_params(**kwargs)
```

### Comparing `skorch-0.9.0/skorch/classifier.py` & `skorch-1.0.0/skorch/classifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 from torch.utils.data import DataLoader
 
 from skorch import NeuralNet
 from skorch.callbacks import EpochTimer
 from skorch.callbacks import PrintLog
 from skorch.callbacks import EpochScoring
 from skorch.callbacks import PassthroughScoring
-from skorch.dataset import CVSplit
-from skorch.utils import get_dim
-from skorch.utils import is_dataset
-from skorch.utils import to_numpy
-
+from skorch.dataset import ValidSplit
+from skorch.utils import data_from_dataset, is_dataset, get_dim, to_numpy
 
 neural_net_clf_doc_start = """NeuralNet for classification tasks
 
     Use this specifically if you have a standard classification task,
     with input data X and target y.
 
 """
@@ -58,15 +55,15 @@
     __doc__ = get_neural_net_clf_doc(NeuralNet.__doc__)
 
     def __init__(
             self,
             module,
             *args,
             criterion=torch.nn.NLLLoss,
-            train_split=CVSplit(5, stratified=True),
+            train_split=ValidSplit(5, stratified=True),
             classes=None,
             **kwargs
     ):
         super(NeuralNetClassifier, self).__init__(
             module,
             *args,
             criterion=criterion,
@@ -96,35 +93,61 @@
 
     @property
     def classes_(self):
         if self.classes is not None:
             if not len(self.classes):
                 raise AttributeError("{} has no attribute 'classes_'".format(
                     self.__class__.__name__))
-            return self.classes
-        return self.classes_inferred_
+            return np.asarray(self.classes)
+
+        try:
+            return self.classes_inferred_
+        except AttributeError as exc:
+            # It's not easily possible to track exactly what circumstances led
+            # to this, so try to make an educated guess and provide a possible
+            # solution.
+            msg = (
+                f"{self.__class__.__name__} could not infer the classes from y; "
+                "this error probably occurred because the net was trained without y "
+                "and some function tried to access the '.classes_' attribute; "
+                "a possible solution is to provide the 'classes' argument when "
+                f"initializing {self.__class__.__name__}"
+            )
+            raise AttributeError(msg) from exc
 
     # pylint: disable=signature-differs
     def check_data(self, X, y):
         if (
                 (y is None) and
                 (not is_dataset(X)) and
                 (self.iterator_train is DataLoader)
         ):
             msg = ("No y-values are given (y=None). You must either supply a "
                    "Dataset as X or implement your own DataLoader for "
                    "training (and your validation) and supply it using the "
                    "``iterator_train`` and ``iterator_valid`` parameters "
                    "respectively.")
             raise ValueError(msg)
+
+        if (y is None) and is_dataset(X):
+            try:
+                _, y_ds = data_from_dataset(X)
+                self.classes_inferred_ = np.unique(to_numpy(y_ds))
+            except AttributeError:
+                # If this fails, we might still be good to go, so don't raise
+                pass
+
         if y is not None:
-            self.classes_inferred_ = np.unique(y)
+            # pylint: disable=attribute-defined-outside-init
+            self.classes_inferred_ = np.unique(to_numpy(y))
 
     # pylint: disable=arguments-differ
     def get_loss(self, y_pred, y_true, *args, **kwargs):
+        # we can assume that the attribute criterion_ exists; if users define
+        # custom criteria, they have to override get_loss anyway
         if isinstance(self.criterion_, torch.nn.NLLLoss):
             eps = torch.finfo(y_pred.dtype).eps
             y_pred = torch.log(y_pred + eps)
         return super().get_loss(y_pred, y_true, *args, **kwargs)
 
     # pylint: disable=signature-differs
     def fit(self, X, y, **fit_params):
@@ -202,15 +225,15 @@
           ``Dataset`` that can deal with the data.
 
         Returns
         -------
         y_pred : numpy ndarray
 
         """
-        return super().predict_proba(X).argmax(axis=1)
+        return self.predict_proba(X).argmax(axis=1)
 
 
 neural_net_binary_clf_doc_start = """NeuralNet for binary classification tasks
 
     Use this specifically if you have a binary classification task,
     with input data X and target y. y must be 1d.
 
@@ -240,15 +263,15 @@
     __doc__ = get_neural_net_binary_clf_doc(NeuralNet.__doc__)
 
     def __init__(
             self,
             module,
             *args,
             criterion=torch.nn.BCEWithLogitsLoss,
-            train_split=CVSplit(5, stratified=True),
+            train_split=ValidSplit(5, stratified=True),
             threshold=0.5,
             **kwargs
     ):
         super().__init__(
             module,
             criterion=criterion,
             train_split=train_split,
@@ -274,15 +297,15 @@
                 lower_is_better=False,
             )),
             ('print_log', PrintLog()),
         ]
 
     @property
     def classes_(self):
-        return [0, 1]
+        return np.array([0, 1])
 
     # pylint: disable=signature-differs
     def check_data(self, X, y):
         super().check_data(X, y)
         if (not is_dataset(X)) and (get_dim(y) != 1):
             raise ValueError("The target data should be 1-dimensional.")
```

### Comparing `skorch-0.9.0/skorch/cli.py` & `skorch-1.0.0/skorch/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,15 +157,16 @@
     return resolved
 
 
 def _yield_preproc_steps(model):
     if not isinstance(model, Pipeline):
         return
 
-    for key, val in model.get_params().items():
+    preproc_pipe = Pipeline(model.steps[:-1])
+    for key, val in preproc_pipe.get_params().items():
         if isinstance(val, BaseEstimator):
             if not isinstance(val, (Pipeline, FeatureUnion)):
                 yield key, val
 
 
 def _yield_estimators(model):
     """Yield estimator and its prefix from the model.
@@ -186,15 +187,20 @@
         module_prefixes.append(name)
         net = model.steps[-1][1]
     else:
         net = model
 
     yield '__'.join(net_prefixes), net
 
-    module = net.module
+    module = getattr(net, 'module', None)
+    if not module:
+        # There is no module attribute, we're dealing with a normal
+        # scikit-learn estimator, so no need to show further help.
+        return
+
     module_prefixes.append('module')
     yield '__'.join(module_prefixes), module
 
 
 def _extract_estimator_cls(estimator):
     if isinstance(estimator, partial):
         # is partialled
@@ -290,20 +296,27 @@
     >>>     parsed = parse_args(kwargs)
     >>>     my_model = parsed(my_model)
     >>>     my_model.fit(X, y)
     >>>
     >>> if __name__ == '__main__':
     >>>     fire.Fire(main)
 
+
+    Note
+    ----
+    The function you pass to `fire.Fire` shouldn't have any positional
+    arguments, otherwise the displayed help will not correctly work;
+    this is a quirk of fire.
+
     Parameters
     ----------
     kwargs : dict
       The arguments as parsed by fire.
 
-    defautls : dict or None (default=None)
+    defaults : dict or None (default=None)
       Optionally, change the default values to use custom
       defaults. Commandline arguments have precedence over defaults.
 
     Returns
     -------
     print_help_and_exit : callable
       If --help is in the arguments, print help and exit.
@@ -312,21 +325,25 @@
       If --help is not in the options, apply command line arguments to
       the estimator and return it.
 
     """
     try:
         import fire  # pylint: disable=unused-import
     except ImportError:
-        raise ImportError("Using skorch cli helpers requires the fire library,"
-                          " you can install it with pip: pip install fire.")
+        raise ImportError(
+            "Using skorch cli helpers requires the fire library,"
+            " you can install it with pip: python -m pip install fire."
+        )
     try:
         import numpydoc.docscrape  # pylint: disable=unused-import
     except ImportError:
-        raise ImportError("Using skorch cli helpers requires the numpydoc library,"
-                          " you can install it with pip: pip install numpydoc.")
+        raise ImportError(
+            "Using skorch cli helpers requires the numpydoc library,"
+            " you can install it with pip: python -m pip install numpydoc."
+        )
 
     defaults = defaults or {}
 
     def print_help_and_exit(estimator):
         print_help(estimator, defaults=defaults)
         sys.exit()
```

### Comparing `skorch-0.9.0/skorch/dataset.py` & `skorch-1.0.0/skorch/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-"""Contains custom skorch Dataset and CVSplit."""
+"""Contains custom skorch Dataset and ValidSplit."""
 import warnings
+from collections.abc import Mapping
 from functools import partial
 from numbers import Number
 
 import numpy as np
 from scipy import sparse
 from sklearn.model_selection import ShuffleSplit
 from sklearn.model_selection import StratifiedKFold
@@ -36,15 +37,15 @@
 def _apply_to_data(data, func, unpack_dict=False):
     """Apply a function to data, trying to unpack different data
     types.
 
     """
     apply_ = partial(_apply_to_data, func=func, unpack_dict=unpack_dict)
 
-    if isinstance(data, dict):
+    if isinstance(data, Mapping):
         if unpack_dict:
             return [apply_(v) for v in data.values()]
         return {k: apply_(v) for k, v in data.items()}
 
     if isinstance(data, (list, tuple)):
         try:
             # e.g.list/tuple of arrays
@@ -65,33 +66,27 @@
 def _len(x):
     if _is_sparse(x):
         return x.shape[0]
     return len(x)
 
 
 def get_len(data):
+    if isinstance(data, Mapping) and (data.get('input_ids') is not None):
+        # Special casing Huggingface BatchEncodings because they are lists of
+        # lists and thus their length would be determined incorrectly, returning
+        # the sequence length instead of the number of samples.
+        return len(data['input_ids'])
     lens = [_apply_to_data(data, _len, unpack_dict=True)]
     lens = list(flatten(lens))
     len_set = set(lens)
     if len(len_set) != 1:
         raise ValueError("Dataset does not have consistent lengths.")
     return list(len_set)[0]
 
 
-def uses_placeholder_y(ds):
-    """If ``ds`` is a ``skorch.dataset.Dataset`` or a
-    ``skorch.dataset.Dataset`` nested inside a
-    ``torch.utils.data.Subset`` and uses
-    y as a placeholder, return ``True``."""
-
-    if isinstance(ds, torch.utils.data.Subset):
-        return uses_placeholder_y(ds.dataset)
-    return isinstance(ds, Dataset) and hasattr(ds, "y") and ds.y is None
-
-
 def unpack_data(data):
     """Unpack data returned by the net's iterator into a 2-tuple.
 
     If the wrong number of items is returned, raise a helpful error
     message.
 
     """
@@ -106,16 +101,15 @@
         # if a 1-tuple/list or something else like a torch tensor
         if not isinstance(data, (tuple, list)) or len(data) < 2:
             raise ValueError(ERROR_MSG_1_ITEM)
         raise ValueError(ERROR_MSG_MORE_THAN_2_ITEMS.format(len(data)))
 
 
 class Dataset(torch.utils.data.Dataset):
-    # pylint: disable=anomalous-backslash-in-string
-    """General dataset wrapper that can be used in conjunction with
+    r"""General dataset wrapper that can be used in conjunction with
     PyTorch :class:`~torch.utils.data.DataLoader`.
 
     The dataset will always yield a tuple of two values, the first
     from the data (``X``) and the second from the target (``y``).
     However, the target is allowed to be ``None``. In that case,
     :class:`.Dataset` will currently return a dummy tensor, since
     :class:`~torch.utils.data.DataLoader` does not work with
@@ -169,16 +163,15 @@
                 raise ValueError("X and y have inconsistent lengths.")
         self._len = len_X
 
     def __len__(self):
         return self._len
 
     def transform(self, X, y):
-        # pylint: disable=anomalous-backslash-in-string
-        """Additional transformations on ``X`` and ``y``.
+        r"""Additional transformations on ``X`` and ``y``.
 
         By default, they are cast to PyTorch :class:`~torch.Tensor`\s.
         Override this if you want a different behavior.
 
         Note: If you use this in conjuction with PyTorch
         :class:`~torch.utils.data.DataLoader`, the latter will call
         the dataset for each row separately, which means that the
@@ -205,15 +198,15 @@
             X = {k: X[k].values.reshape(-1, 1) for k in X}
 
         Xi = multi_indexing(X, i, self.X_indexing)
         yi = multi_indexing(y, i, self.y_indexing)
         return self.transform(Xi, yi)
 
 
-class CVSplit:
+class ValidSplit:
     """Class that performs the internal train/valid split on a dataset.
 
     The ``cv`` argument here works similarly to the regular sklearn ``cv``
     parameter in, e.g., ``GridSearchCV``. However, instead of cycling
     through all splits, only one fixed split (the first one) is
     used. To get a full cycle through the splits, don't use
     ``NeuralNet``'s internal validation but instead the corresponding
@@ -256,23 +249,21 @@
             random_state=None,
     ):
         self.stratified = stratified
         self.random_state = random_state
 
         if isinstance(cv, Number) and (cv <= 0):
             raise ValueError("Numbers less than 0 are not allowed for cv "
-                             "but CVSplit got {}".format(cv))
+                             "but ValidSplit got {}".format(cv))
 
         if not self._is_float(cv) and random_state is not None:
-            # TODO: raise a ValueError instead of a warning
-            warnings.warn(
+            raise ValueError(
                 "Setting a random_state has no effect since cv is not a float. "
-                "This will raise an error in a future. You should leave "
-                "random_state to its default (None), or set cv to a float value.",
-                FutureWarning
+                "You should leave random_state to its default (None), or set cv "
+                "to a float value.",
             )
 
         self.cv = cv
 
     def _is_stratified(self, cv):
         return isinstance(cv, (StratifiedKFold, StratifiedShuffleSplit))
 
@@ -335,8 +326,8 @@
         idx_train, idx_valid = next(iter(cv.split(*args, groups=groups)))
         dataset_train = torch.utils.data.Subset(dataset, idx_train)
         dataset_valid = torch.utils.data.Subset(dataset, idx_valid)
         return dataset_train, dataset_valid
 
     def __repr__(self):
         # pylint: disable=useless-super-delegation
-        return super(CVSplit, self).__repr__()
+        return super(ValidSplit, self).__repr__()
```

### Comparing `skorch-0.9.0/skorch/helper.py` & `skorch-1.0.0/skorch/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 """Helper functions and classes for users.
 
-They should not be used in skorch directly.
+They are intended to be used by end users but should not be depended upon for
+skorch-internal usage.
 
 """
-from collections import Sequence
-from collections import namedtuple
+from collections.abc import Sequence
 from functools import partial
 
 import numpy as np
 from sklearn.base import BaseEstimator
 from sklearn.base import TransformerMixin
 import torch
 
+from skorch._doctor import SkorchDoctor
 from skorch.cli import parse_args
 from skorch.utils import _make_split
+from skorch.utils import to_numpy
 from skorch.utils import is_torch_data_type
 from skorch.utils import to_tensor
 
 
+__all__ = [
+    "DataFrameTransformer",
+    "SliceDataset",
+    "SkorchDoctor",
+    "SliceDict",
+    "predefined_split",
+    "parse_args",
+]
+
+
 class SliceDict(dict):
     """Wrapper for Python dict that makes it sliceable across values.
 
     Use this if your input data is a dictionary and you have problems
     with sklearn not being able to slice it. Wrap your dict with
     SliceDict and it should usually work.
 
@@ -49,50 +61,50 @@
                 "".format(', '.join(map(str, sorted(lengths_set)))))
 
         if not lengths:
             self._len = 0
         else:
             self._len = lengths[0]
 
-        super(SliceDict, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __len__(self):
         return self._len
 
     def __getitem__(self, sl):
         if isinstance(sl, int):
             # Indexing with integers is not well-defined because that
             # recudes the dimension of arrays by one, messing up
             # lengths and shapes.
             raise ValueError("SliceDict cannot be indexed by integers.")
         if isinstance(sl, str):
-            return super(SliceDict, self).__getitem__(sl)
-        return SliceDict(**{k: v[sl] for k, v in self.items()})
+            return super().__getitem__(sl)
+        return type(self)(**{k: v[sl] for k, v in self.items()})
 
     def __setitem__(self, key, value):
         if not isinstance(key, str):
             raise TypeError("Key must be str, not {}.".format(type(key)))
 
         length = value.shape[0]
         if not self.keys():
             self._len = length
 
         if self._len != length:
             raise ValueError(
                 "Cannot set array with shape[0] != {}"
                 "".format(self._len))
 
-        super(SliceDict, self).__setitem__(key, value)
+        super().__setitem__(key, value)
 
     def update(self, kwargs):
         for key, value in kwargs.items():
             self.__setitem__(key, value)
 
     def __repr__(self):
-        out = super(SliceDict, self).__repr__()
+        out = super().__repr__()
         return "SliceDict(**{})".format(out)
 
     @property
     def shape(self):
         return (self._len,)
 
     def copy(self):
@@ -229,34 +241,43 @@
 
     def __getitem__(self, i):
         if isinstance(i, (int, np.integer)):
             Xn = self.dataset[self.indices_[i]]
             Xi = self._select_item(Xn)
             return self.transform(Xi)
 
+        cls = type(self)
         if isinstance(i, slice):
-            return SliceDataset(self.dataset, idx=self.idx, indices=self.indices_[i])
+            return cls(self.dataset, idx=self.idx, indices=self.indices_[i])
 
         if isinstance(i, np.ndarray):
             if i.ndim != 1:
                 raise IndexError("SliceDataset only supports slicing with 1 "
                                  "dimensional arrays, got {} dimensions instead."
                                  "".format(i.ndim))
-            if i.dtype == np.bool:
+            if i.dtype == bool:
                 i = np.flatnonzero(i)
 
-        return SliceDataset(self.dataset, idx=self.idx, indices=self.indices_[i])
+        return cls(self.dataset, idx=self.idx, indices=self.indices_[i])
+
+    def __array__(self, dtype=None):
+        # This method is invoked when calling np.asarray(X)
+        # https://numpy.org/devdocs/user/basics.dispatch.html
+        X = [self[i] for i in range(len(self))]
+        if np.isscalar(X[0]):
+            return np.asarray(X)
+        return np.asarray([to_numpy(x) for x in X], dtype=dtype)
 
 
 def predefined_split(dataset):
     """Uses ``dataset`` for validiation in :class:`.NeuralNet`.
 
     Examples
     --------
-    >>> valid_ds = skorch.Dataset(X, y)
+    >>> valid_ds = skorch.dataset.Dataset(X, y)
     >>> net = NeuralNet(..., train_split=predefined_split(valid_ds))
 
     Parameters
     ----------
     dataset: torch Dataset
        Validiation dataset
 
@@ -345,16 +366,14 @@
 
     Notes
     -----
     The value of X will always be 2-dimensional, even if it only
     contains 1 column.
 
     """
-    import pandas as pd
-
     def __init__(
             self,
             treat_int_as_categorical=False,
             float_dtype=np.float32,
             int_dtype=np.int64,
     ):
         self.treat_int_as_categorical = treat_int_as_categorical
@@ -374,24 +393,26 @@
         ValueError
           If there already is a column named 'X'.
 
         TypeError
           If a wrong dtype is found.
 
         """
+        import pandas as pd
+
         if 'X' in df:
             raise ValueError(
                 "DataFrame contains a column named 'X', which clashes "
                 "with the name chosen for cardinal features; consider "
                 "renaming that column.")
 
         wrong_dtypes = []
 
         for col, dtype in zip(df, df.dtypes):
-            if isinstance(dtype, self.pd.api.types.CategoricalDtype):
+            if isinstance(dtype, pd.api.types.CategoricalDtype):
                 continue
             if np.issubdtype(dtype, np.integer):
                 continue
             if np.issubdtype(dtype, np.floating):
                 continue
             wrong_dtypes.append((col, dtype))
 
@@ -422,23 +443,25 @@
         -------
         X_dict: dict
           Dictionary with all floats concatenated using the key "X"
           and all categorical values encoded as integers, using their
           respective column names as keys.
 
         """
+        import pandas as pd
+
         self._check_dtypes(df)
 
         X_dict = {}
         Xf = []  # floats
 
         for col, dtype in zip(df, df.dtypes):
             X_col = df[col]
 
-            if isinstance(dtype, self.pd.api.types.CategoricalDtype):
+            if isinstance(dtype, pd.api.types.CategoricalDtype):
                 x = X_col.cat.codes.values
                 if self.int_dtype is not None:
                     x = x.astype(self.int_dtype)
                 X_dict[col] = x
                 continue
 
             if (
```

### Comparing `skorch-0.9.0/skorch/net.py` & `skorch-1.0.0/skorch/net.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,57 @@
-"""Neural net classes."""
+"""Neural net base class
+
+This is the most flexible class, not making assumptions on the kind of
+task being peformed. Subclass this to create more specialized and
+sklearn-conforming classes like NeuralNetClassifier.
+
+"""
 
 import fnmatch
+from collections.abc import Mapping
+from functools import partial
 from itertools import chain
 from collections import OrderedDict
+from contextlib import contextmanager
+import os
 import tempfile
 import warnings
 
 import numpy as np
 from sklearn.base import BaseEstimator
 import torch
 from torch.utils.data import DataLoader
 
 from skorch.callbacks import EpochTimer
 from skorch.callbacks import PrintLog
 from skorch.callbacks import PassthroughScoring
 from skorch.dataset import Dataset
-from skorch.dataset import CVSplit
+from skorch.dataset import ValidSplit
 from skorch.dataset import get_len
 from skorch.dataset import unpack_data
-from skorch.dataset import uses_placeholder_y
 from skorch.exceptions import DeviceWarning
+from skorch.exceptions import SkorchAttributeError
+from skorch.exceptions import SkorchTrainingImpossibleError
 from skorch.history import History
 from skorch.setter import optimizer_setter
 from skorch.utils import _identity
-from skorch.utils import _infer_predict_nonlinearty
+from skorch.utils import _infer_predict_nonlinearity
 from skorch.utils import FirstStepAccumulator
 from skorch.utils import TeeGenerator
 from skorch.utils import _check_f_arguments
 from skorch.utils import check_is_fitted
 from skorch.utils import duplicate_items
 from skorch.utils import get_map_location
 from skorch.utils import is_dataset
 from skorch.utils import params_for
 from skorch.utils import to_device
 from skorch.utils import to_numpy
 from skorch.utils import to_tensor
 
 
-_PYTORCH_COMPONENTS = {'criterion', 'module', 'optimizer'}
-"""Special names that mark pytorch components.
-
-These special names are used to recognize whether an attribute that is
-being set in the net should be added to prefixes_ and
-cuda_dependent_attributes_
-
-"""
-
-
 # pylint: disable=too-many-instance-attributes
 class NeuralNet:
     # pylint: disable=anomalous-backslash-in-string
     """NeuralNet base class.
 
     The base class covers more generic cases. Depending on your use
     case, you might want to use :class:`.NeuralNetClassifier` or
@@ -80,15 +81,15 @@
 
     This can be useful when you want to change certain parameters
     using a callback, when using the net in an sklearn grid search,
     etc.
 
     By default an :class:`.EpochTimer`, :class:`.BatchScoring` (for
     both training and validation datasets), and :class:`.PrintLog`
-    callbacks are installed for the user's convenience.
+    callbacks are added for convenience.
 
     Parameters
     ----------
     module : torch module (class or instance)
       A PyTorch :class:`~torch.nn.Module`. In general, the
       uninstantiated class should be passed, although instantiated
       modules will also work.
@@ -131,25 +132,34 @@
       dealing with a lot of data types out of the box, so only change
       this if your data is not supported. You should generally pass the
       uninitialized ``Dataset`` class and define additional arguments to
       X and y by prefixing them with ``dataset__``. It is also possible
       to pass an initialzed ``Dataset``, in which case no additional
       arguments may be passed.
 
-    train_split : None or callable (default=skorch.dataset.CVSplit(5))
-      If None, there is no train/validation split. Else, train_split
+    train_split : None or callable (default=skorch.dataset.ValidSplit(5))
+      If ``None``, there is no train/validation split. Else, ``train_split``
       should be a function or callable that is called with X and y
       data and should return the tuple ``dataset_train, dataset_valid``.
-      The validation data may be None.
+      The validation data may be ``None``.
 
-    callbacks : None or list of Callback instances (default=None)
-      More callbacks, in addition to those returned by
-      ``get_default_callbacks``. Each callback should inherit from
-      :class:`.Callback`. If not ``None``, a list of callbacks is
-      expected where the callback names are inferred from the class
+    callbacks : None, "disable", or list of Callback instances (default=None)
+      Which callbacks to enable. There are three possible values:
+
+      If ``callbacks=None``, only use default callbacks,
+      those returned by ``get_default_callbacks``.
+
+      If ``callbacks="disable"``, disable all callbacks, i.e. do not run
+      any of the callbacks, not even the default callbacks.
+
+      If ``callbacks`` is a list of callbacks, use those callbacks in
+      addition to the default callbacks. Each callback should be an
+      instance of :class:`.Callback`.
+
+      Callback names are inferred from the class
       name. Name conflicts are resolved by appending a count suffix
       starting with 1, e.g. ``EpochScoring_1``. Alternatively,
       a tuple ``(name, callback)`` can be passed, where ``name``
       should be unique. Callbacks may or may not be instantiated.
       The callback name can be used to set parameters on specific
       callbacks (e.g., for the callback with name ``'print_log'``, use
       ``net.set_params(callbacks__print_log__keys_ignored=['epoch',
@@ -191,26 +201,51 @@
       This parameter controls how much print output is generated by
       the net and its callbacks. By setting this value to 0, e.g. the
       summary scores at the end of each epoch are no longer printed.
       This can be useful when running a hyperparameter search. The
       summary scores are always logged in the history attribute,
       regardless of the verbose setting.
 
-    device : str, torch.device (default='cpu')
-      The compute device to be used. If set to 'cuda', data in torch
-      tensors will be pushed to cuda tensors before being sent to the
-      module. If set to None, then all compute devices will be left
-      unmodified.
+    device : str, torch.device, or None (default='cpu')
+      The compute device to be used. If set to 'cuda' in order to use
+      GPU acceleration, data in torch tensors will be pushed to cuda
+      tensors before being sent to the module. If set to None, then
+      all compute devices will be left unmodified.
+
+    compile : bool (default=False)
+      If set to ``True``, compile all modules using ``torch.compile``. For this
+      to work, the installed torch version has to support ``torch.compile``.
+      Compiled modules should work identically to non-compiled modules but
+      should run faster on new GPU architectures (Volta and Ampere for
+      instance).
+      Additional arguments for ``torch.compile`` can be passed using the dunder
+      notation, e.g. when initializing the net with ``compile__dynamic=True``,
+      ``torch.compile`` will be called with ``dynamic=True``.
+
+    use_caching : bool or 'auto' (default='auto')
+      Optionally override the caching behavior of scoring callbacks. Callbacks
+      such as :class:`.EpochScoring` and :class:`.BatchScoring` allow to cache
+      the inference call to save time when calculating scores during training at
+      the expense of memory. In certain situations, e.g. when memory is tight,
+      you may want to disable caching. As it is cumbersome to change the setting
+      on each callback individually, this parameter allows to override their
+      behavior globally.
+      By default (``'auto'``), the callbacks will determine if caching is used
+      or not. If this argument is set to ``False``, caching will be disabled on
+      all callbacks. If set to ``True``, caching will be enabled on all
+      callbacks.
+      Implementation note: It is the job of the callbacks to honor this setting.
 
     Attributes
     ----------
     prefixes_ : list of str
       Contains the prefixes to special parameters. E.g., since there
-      is the ``'module'`` prefix, it is possible to set parameters like
-      so: ``NeuralNet(..., optimizer__momentum=0.95)``.
+      is the ``'optimizer'`` prefix, it is possible to set parameters like
+      so: ``NeuralNet(..., optimizer__momentum=0.95)``. Some prefixes are
+      populated dynamically, based on what modules and criteria are defined.
 
     cuda_dependent_attributes_ : list of str
       Contains a list of all attribute prefixes whose values depend on a
       CUDA device. If a ``NeuralNet`` trained with a CUDA-enabled device
       is unpickled on a machine without CUDA or with CUDA disabled, the
       listed attributes are mapped to CPU.  Expand this list if you
       want to add other cuda-dependent attributes.
@@ -224,38 +259,62 @@
     criterion_ : torch criterion (instance)
       The instantiated criterion.
 
     callbacks_ : list of tuples
       The complete (i.e. default and other), initialized callbacks, in
       a tuple with unique names.
 
+    _modules : list of str
+      List of names of all modules that are torch modules. This list is
+      collected dynamically when the net is initialized. Typically, there is no
+      reason for a user to modify this list.
+
+    _criteria : list of str
+      List of names of all criteria that are torch modules. This list is
+      collected dynamically when the net is initialized. Typically, there is no
+      reason for a user to modify this list.
+
+    _optimizers : list of str
+      List of names of all optimizers. This list is collected dynamically when
+      the net is initialized. Typically, there is no reason for a user to modify
+      this list.
+
     """
-    prefixes_ = ['module', 'iterator_train', 'iterator_valid', 'optimizer',
-                 'criterion', 'callbacks', 'dataset']
+    prefixes_ = ['iterator_train', 'iterator_valid', 'callbacks', 'dataset', 'compile']
+
+    cuda_dependent_attributes_ = []
+
+    # This attribute keeps track of which initialization method is being used.
+    # It should not be changed manually.
+    init_context_ = None
 
-    cuda_dependent_attributes_ = ['module_', 'optimizer_', 'criterion_']
+    _modules = []
+    _criteria = []
+    _optimizers = []
 
     # pylint: disable=too-many-arguments
     def __init__(
             self,
             module,
             criterion,
             optimizer=torch.optim.SGD,
             lr=0.01,
             max_epochs=10,
             batch_size=128,
             iterator_train=DataLoader,
             iterator_valid=DataLoader,
             dataset=Dataset,
-            train_split=CVSplit(5),
+            train_split=ValidSplit(5),
             callbacks=None,
             predict_nonlinearity='auto',
             warm_start=False,
             verbose=1,
             device='cpu',
+            compile=False,
+            use_caching='auto',
             **kwargs
     ):
         self.module = module
         self.criterion = criterion
         self.optimizer = optimizer
         self.lr = lr
         self.max_epochs = max_epochs
@@ -265,21 +324,23 @@
         self.dataset = dataset
         self.train_split = train_split
         self.callbacks = callbacks
         self.predict_nonlinearity = predict_nonlinearity
         self.warm_start = warm_start
         self.verbose = verbose
         self.device = device
+        self.compile = compile
+        self.use_caching = use_caching
 
         self._check_deprecated_params(**kwargs)
         history = kwargs.pop('history', None)
         initialized = kwargs.pop('initialized_', False)
         virtual_params = kwargs.pop('virtual_params_', dict())
 
-        kwargs = self._check_kwargs(kwargs)
+        self._params_to_validate = set(kwargs.keys())
         vars(self).update(kwargs)
 
         self.history_ = history
         self.initialized_ = initialized
         self.virtual_params_ = virtual_params
 
     @property
@@ -321,58 +382,63 @@
 
         """
         getattr(self, method_name)(self, **cb_kwargs)
         for _, cb in self.callbacks_:
             getattr(cb, method_name)(self, **cb_kwargs)
 
     # pylint: disable=unused-argument
-    def on_train_begin(self, net,
-                       X=None, y=None, **kwargs):
+    def on_train_begin(self, net, X=None, y=None, **kwargs):
         pass
 
     # pylint: disable=unused-argument
-    def on_train_end(self, net,
-                     X=None, y=None, **kwargs):
+    def on_train_end(self, net, X=None, y=None, **kwargs):
         pass
 
     # pylint: disable=unused-argument
-    def on_epoch_begin(self, net,
-                       dataset_train=None, dataset_valid=None, **kwargs):
+    def on_epoch_begin(self, net, dataset_train=None, dataset_valid=None, **kwargs):
         self.history.new_epoch()
         self.history.record('epoch', len(self.history))
 
     # pylint: disable=unused-argument
-    def on_epoch_end(self, net,
-                     dataset_train=None, dataset_valid=None, **kwargs):
+    def on_epoch_end(self, net, dataset_train=None, dataset_valid=None, **kwargs):
         pass
 
     # pylint: disable=unused-argument
-    def on_batch_begin(self, net,
-                       Xi=None, yi=None, training=False, **kwargs):
+    def on_batch_begin(self, net, batch=None, training=False, **kwargs):
         self.history.new_batch()
 
-    def on_batch_end(self, net,
-                     Xi=None, yi=None, training=False, **kwargs):
+    def on_batch_end(self, net, batch=None, training=False, **kwargs):
         pass
 
-    def on_grad_computed(self, net, named_parameters,
-                         Xi=None, yi=None,
-                         training=False, **kwargs):
+    def on_grad_computed(
+            self, net, named_parameters, batch=None, training=False, **kwargs):
         pass
 
     def _yield_callbacks(self):
         """Yield all callbacks set on this instance including
         a set whether its name was set by the user.
 
         Handles these cases:
           * default and user callbacks
           * callbacks with and without name
           * initialized and uninitialized callbacks
           * puts PrintLog(s) last
 
+        Yields
+        ------
+        name : str
+          Name of the callback.
+
+        cb : Callback or Callback instance
+          The callback itself
+
+        named_by_user : bool
+          Whether the name was given by the user or determined
+          automatically.
+
         """
         print_logs = []
         for item in self.get_default_callbacks() + (self.callbacks or []):
             if isinstance(item, (tuple, list)):
                 named_by_user = True
                 name, cb = item
             else:
@@ -460,64 +526,78 @@
             if isinstance(cb, type):  # uninitialized:
                 cb = cb(**params)
             else:
                 cb.set_params(**params)
             cb.initialize()
             callbacks_.append((name, cb))
 
+        # pylint: disable=attribute-defined-outside-init
         self.callbacks_ = callbacks_
         return self
 
-    def initialize_criterion(self):
-        """Initializes the criterion."""
-        criterion_params = self.get_params_for('criterion')
-        self.criterion_ = self.criterion(**criterion_params)
-        if isinstance(self.criterion_, torch.nn.Module):
-            self.criterion_ = to_device(self.criterion_, self.device)
-        return self
+    def initialized_instance(self, instance_or_cls, kwargs):
+        """Return an instance initialized with the given parameters
 
-    def _format_reinit_msg(self, name, kwargs=None, triggered_directly=True):
-        """Returns a message that informs about re-initializing a compoment.
+        This is a helper method that deals with several possibilities for a
+        component that might need to be initialized:
 
-        Sometimes, the module or optimizer need to be
-        re-initialized. Not only should the user receive a message
-        about this but also should they be informed about what
-        parameters, if any, caused it.
+        * It is already an instance that's good to go
+        * It is an instance but it needs to be re-initialized
+        * It's not an instance and needs to be initialized
 
-        """
-        msg = "Re-initializing {}".format(name)
-        if triggered_directly and kwargs:
-            msg += (" because the following parameters were re-set: {}."
-                    .format(', '.join(sorted(kwargs))))
-        else:
-            msg += "."
-        return msg
+        For the majority of use cases, this comes down to just comes down to
+        just initializing the class with its arguments.
 
-    def initialize_module(self):
-        """Initializes the module.
+        Parameters
+        ----------
+        instance_or_cls
+          The instance or class or callable to be initialized, e.g.
+          ``self.module``.
 
-        Note that if the module has learned parameters, those will be
-        reset.
+        kwargs : dict
+          The keyword arguments to initialize the instance or class. Can be an
+          empty dict.
+
+        Returns
+        -------
+        instance
+          The initialized component.
 
         """
-        kwargs = self.get_params_for('module')
-        module = self.module
-        is_initialized = isinstance(module, torch.nn.Module)
+        is_init = isinstance(instance_or_cls, torch.nn.Module)
+        if is_init and not kwargs:
+            return instance_or_cls
+        if is_init:
+            return type(instance_or_cls)(**kwargs)
+        return instance_or_cls(**kwargs)
 
-        if kwargs or not is_initialized:
-            if is_initialized:
-                module = type(module)
+    def initialize_criterion(self):
+        """Initializes the criterion.
 
-            if (is_initialized or self.initialized_) and self.verbose:
-                msg = self._format_reinit_msg("module", kwargs)
-                print(msg)
+        If the criterion is already initialized and no parameter was changed, it
+        will be left as is.
+
+        """
+        kwargs = self.get_params_for('criterion')
+        criterion = self.initialized_instance(self.criterion, kwargs)
+        # pylint: disable=attribute-defined-outside-init
+        self.criterion_ = criterion
+        return self
+
+    def initialize_module(self):
+        """Initializes the module.
 
-            module = module(**kwargs)
+        If the module is already initialized and no parameter was changed, it
+        will be left as is.
 
-        self.module_ = to_device(module, self.device)
+        """
+        kwargs = self.get_params_for('module')
+        module = self.initialized_instance(self.module, kwargs)
+        # pylint: disable=attribute-defined-outside-init
+        self.module_ = module
         return self
 
     def _is_virtual_param(self, key):
         return any(fnmatch.fnmatch(key, pat) for pat in self.virtual_params_)
 
     def _virtual_setattr(self, param, val):
         setattr(self, param, val)
@@ -534,133 +614,393 @@
                 if not fnmatch.fnmatch(key, pattern):
                     continue
                 fn(self, key, val)
 
     def initialize_virtual_params(self):
         self.virtual_params_ = {}
 
-    def initialize_optimizer(self, triggered_directly=True):
+    def initialize_optimizer(self, triggered_directly=None):
         """Initialize the model optimizer. If ``self.optimizer__lr``
         is not set, use ``self.lr`` instead.
 
         Parameters
         ----------
-        triggered_directly : bool (default=True)
-          Only relevant when optimizer is re-initialized.
-          Initialization of the optimizer can be triggered directly
-          (e.g. when lr was changed) or indirectly (e.g. when the
-          module was re-initialized). If and only if the former
-          happens, the user should receive a message informing them
-          about the parameters that caused the re-initialization.
+        triggered_directly
+          Deprecated, don't use it anymore.
 
         """
-        args, kwargs = self.get_params_for_optimizer(
-            'optimizer', self.module_.named_parameters())
-
-        if self.initialized_ and self.verbose:
-            msg = self._format_reinit_msg(
-                "optimizer", kwargs, triggered_directly=triggered_directly)
-            print(msg)
+        # handle deprecated paramter
+        if triggered_directly is not None:
+            warnings.warn(
+                "The 'triggered_directly' argument to 'initialize_optimizer' is "
+                "deprecated, please don't use it anymore.", DeprecationWarning)
 
-        if 'lr' not in kwargs:
-            kwargs['lr'] = self.lr
+        named_parameters = self.get_all_learnable_params()
+        args, kwargs = self.get_params_for_optimizer(
+            'optimizer', named_parameters)
 
+        # pylint: disable=attribute-defined-outside-init
         self.optimizer_ = self.optimizer(*args, **kwargs)
-
-        self._register_virtual_param(
-            ['optimizer__param_groups__*__*', 'optimizer__*', 'lr'],
-            optimizer_setter,
-        )
+        return self
 
     def initialize_history(self):
         """Initializes the history."""
-        self.history_ = History()
+        if self.history_ is None:
+            self.history_ = History()
+        else:
+            self.history_.clear()
+        return self
 
-    def initialize(self):
-        """Initializes all components of the :class:`.NeuralNet` and
-        returns self.
+    def _format_reinit_msg(self, name, kwargs=None, triggered_directly=True):
+        """Returns a message that informs about re-initializing a compoment.
+
+        Sometimes, the module or optimizer need to be
+        re-initialized. Not only should the user receive a message
+        about this but also should they be informed about what
+        parameters, if any, caused it.
+
+        """
+        msg = "Re-initializing {}".format(name)
+        if triggered_directly and kwargs:
+            msg += (" because the following parameters were re-set: {}"
+                    .format(', '.join(sorted(kwargs))))
+        msg += "."
+        return msg
+
+    @contextmanager
+    def _current_init_context(self, name):
+        try:
+            self.init_context_ = name
+            yield
+        finally:
+            self.init_context_ = None
+
+    def _initialize_virtual_params(self):
+        # this init context is for consistency and not being used at the moment
+        with self._current_init_context('virtual_params'):
+            self.initialize_virtual_params()
+            return self
+
+    def _initialize_callbacks(self):
+        # this init context is for consistency and not being used at the moment
+        with self._current_init_context('callbacks'):
+            if self.callbacks == "disable":
+                self.callbacks_ = []
+                return self
+            self.initialize_callbacks()
+            return self
+
+    def _initialize_criterion(self, reason=None):
+        # _initialize_criterion and _initialize_module share the same logic
+        with self._current_init_context('criterion'):
+            kwargs = {}
+            for criterion_name in self._criteria:
+                kwargs.update(self.get_params_for(criterion_name))
+
+            has_init_criterion = any(
+                isinstance(getattr(self, criterion_name + '_', None), torch.nn.Module)
+                for criterion_name in self._criteria)
+
+            # check if a re-init message is required
+            if kwargs or reason or has_init_criterion:
+                if self.initialized_ and self.verbose:
+                    if reason:
+                        # re-initialization was triggered indirectly
+                        msg = reason
+                    else:
+                        # re-initialization was triggered directly
+                        msg = self._format_reinit_msg("criterion", kwargs)
+                    print(msg)
+
+            self.initialize_criterion()
+
+            # deal with device
+            for name in self._criteria:
+                criterion = getattr(self, name + '_')
+                if isinstance(criterion, torch.nn.Module):
+                    criterion = to_device(criterion, self.device)
+                    criterion = self.torch_compile(criterion, name=name)
+                    setattr(self, name + '_', criterion)
+
+            return self
+
+    def _initialize_module(self, reason=None):
+        # _initialize_criterion and _initialize_module share the same logic
+        with self._current_init_context('module'):
+            kwargs = {}
+            for module_name in self._modules:
+                kwargs.update(self.get_params_for(module_name))
+
+            has_init_module = any(
+                isinstance(getattr(self, module_name + '_', None), torch.nn.Module)
+                for module_name in self._modules)
+
+            if kwargs or reason or has_init_module:
+                if self.initialized_ and self.verbose:
+                    if reason:
+                        # re-initialization was triggered indirectly
+                        msg = reason
+                    else:
+                        # re-initialization was triggered directly
+                        msg = self._format_reinit_msg("module", kwargs)
+                    print(msg)
+
+            self.initialize_module()
+
+            # deal with device
+            for name in self._modules:
+                module = getattr(self, name + '_')
+                if isinstance(module, torch.nn.Module):
+                    module = to_device(module, self.device)
+                    module = self.torch_compile(module, name=name)
+                    setattr(self, name + '_', module)
+
+            return self
+
+    # pylint: disable=unused-argument
+    def torch_compile(self, module, name):
+        """Compile torch modules
+
+        If ``compile=True`` was set, compile all torch modules of the net. Those
+        typically are ``module_`` and ``criterion_``, but custom modules are
+        also included if defined.
+
+        Notes
+        -----
+        Make sure that the installed PyTorch version supports compiling (v1.14,
+        v2.0 and higher).
+
+        Parameters
+        ----------
+        module : torch.nn.Module
+          The torch module to be compiled.
+
+        name : str
+          The name of the module. This argument is not used but provided for
+          convenience. You could use it, e.g., to skip compilation for specific
+          modules.
+
+        Returns
+        -------
+        module : torch.nn.Module or torch._dynamo.OptimizedModule
+          The compiled module if ``compile=True``, otherwise the uncompiled module.
+
+        Raises
+        ------
+        ValueError
+          If ``compile=True`` but ``torch.compile`` is not available, raise an
+          error.
 
         """
-        self.initialize_virtual_params()
-        self.initialize_callbacks()
-        self.initialize_criterion()
-        self.initialize_module()
-        self.initialize_optimizer()
-        self.initialize_history()
+        # TODO: adjust docstring once we no longer support PyTorch versions without compile
+        if not self.compile:
+            return module
+
+        # Whether torch.compile is available (PyTorch 2.0 and up)
+        torch_compile_available = hasattr(torch, 'compile')
+        if not torch_compile_available:
+            raise ValueError(
+                "Setting compile=True but torch.compile is not available. Please "
+                f"check that your installed PyTorch version ({torch.__version__}) "
+                "supports torch.compile (requires v1.14, v2.0 or higher)")
+
+        params = self.get_params_for('compile')
+        module_compiled = torch.compile(module, **params)
+        return module_compiled
+
+    def get_all_learnable_params(self):
+        """Yield the learnable parameters of all modules
+
+        Typically, this will yield the ``named_parameters`` of the standard
+        module of the net. However, if you add custom modules or if your
+        criterion has learnable parameters, these are returned as well.
+
+        If you want your optimizer to only update the parameters of some but not
+        all modules, you should override :meth:`.initialize_module` and match
+        the corresponding modules and optimizers there:
+
+        .. code:: python
+
+            class MyNet(NeuralNet):
+
+                def initialize_optimizer(self, *args, **kwargs):
+                    # first initialize the normal optimizer
+                    named_params = self.module_.named_parameters()
+                    args, kwargs = self.get_params_for_optimizer('optimizer', named_params)
+                    self.optimizer_ = self.optimizer(*args, **kwargs)
+
+                    # next add an another optimizer called 'optimizer2_' that is
+                    # only responsible for training 'module2_'
+                    named_params = self.module2_.named_parameters()
+                    args, kwargs = self.get_params_for_optimizer('optimizer2', named_params)
+                    self.optimizer2_ = torch.optim.SGD(*args, **kwargs)
+                    return self
+
+        Yields
+        ------
+        named_parameters : generator of parameter name and parameter
+          A generator over all module parameters, yielding both the name of the
+          parameter as well as the parameter itself. Use this, for instance, to
+          pass the named parameters to :meth:`.get_params_for_optimizer`.
+
+        """
+        # Note: we have to filter out potential duplicate parameters. This can
+        # happen when a module references another module (e.g. the criterion
+        # references the module), thus yielding that module's parameters again.
+        # The parameter name can be difference, therefore we check only the
+        # identity of the parameter itself.
+        seen = set()
+        for name in self._modules + self._criteria:
+            module = getattr(self, name + '_')
+            named_parameters = getattr(module, 'named_parameters', None)
+            if not named_parameters:
+                continue
+
+            for param_name, param in named_parameters():
+                if param in seen:
+                    continue
+
+                seen.add(param)
+                yield param_name, param
+
+    def _initialize_optimizer(self, reason=None):
+        with self._current_init_context('optimizer'):
+            if self.initialized_ and self.verbose:
+                if reason:
+                    # re-initialization was triggered indirectly
+                    msg = reason
+                else:
+                    # re-initialization was triggered directly
+                    msg = self._format_reinit_msg("optimizer", triggered_directly=False)
+                print(msg)
+
+            self.initialize_optimizer()
+
+            # register the virtual params for all optimizers
+            for name in self._optimizers:
+                param_pattern = [name + '__param_groups__*__*', name + '__*']
+                if name == 'optimizer':  # 'lr' is short for optimizer__lr
+                    param_pattern.append('lr')
+                setter = partial(
+                    optimizer_setter,
+                    optimizer_attr=name + '_',
+                    optimizer_name=name,
+                )
+                self._register_virtual_param(param_pattern, setter)
+            return self
+
+    def _initialize_history(self):
+        # this init context is for consistency and not being used at the moment
+        with self._current_init_context('history'):
+            self.initialize_history()
+            return self
+
+    def initialize(self):
+        """Initializes all of its components and returns self."""
+        self.check_training_readiness()
+
+        self._initialize_virtual_params()
+        self._initialize_callbacks()
+        self._initialize_module()
+        self._initialize_criterion()
+        self._initialize_optimizer()
+        self._initialize_history()
+
+        self._validate_params()
 
         self.initialized_ = True
         return self
 
+    def check_training_readiness(self):
+        """Check that the net is ready to train"""
+        is_trimmed_for_prediction = getattr(self, '_trimmed_for_prediction', False)
+        if is_trimmed_for_prediction:
+            msg = (
+                "The net's attributes were trimmed for prediction, thus it cannot "
+                "be used for training anymore"
+            )
+            raise SkorchTrainingImpossibleError(msg)
+
     def check_data(self, X, y=None):
         pass
 
-    def validation_step(self, Xi, yi, **fit_params):
+    def _set_training(self, training=True):
+        """Set training/evaluation mode on all modules and criteria that are torch
+        Modules.
+
+        Parameters
+        ----------
+        training : bool (default=True)
+          Whether to set to training mode (True) or evaluation mode (False).
+
+        """
+        for module_name in self._modules + self._criteria:
+            module = getattr(self, module_name + '_')
+            if isinstance(module, torch.nn.Module):
+                module.train(training)
+
+    def validation_step(self, batch, **fit_params):
         """Perform a forward step using batched data and return the
         resulting loss.
 
         The module is set to be in evaluation mode (e.g. dropout is
         not applied).
 
         Parameters
         ----------
-        Xi : input data
-          A batch of the input data.
-
-        yi : target data
-          A batch of the target data.
+        batch
+          A single batch returned by the data loader.
 
         **fit_params : dict
           Additional parameters passed to the ``forward`` method of
           the module and to the ``self.train_split`` call.
 
         """
-        self.module_.eval()
+        self._set_training(False)
+        Xi, yi = unpack_data(batch)
         with torch.no_grad():
             y_pred = self.infer(Xi, **fit_params)
             loss = self.get_loss(y_pred, yi, X=Xi, training=False)
         return {
             'loss': loss,
             'y_pred': y_pred,
-            }
+        }
 
-    def train_step_single(self, Xi, yi, **fit_params):
+    def train_step_single(self, batch, **fit_params):
         """Compute y_pred, loss value, and update net's gradients.
 
         The module is set to be in train mode (e.g. dropout is
         applied).
 
         Parameters
         ----------
-        Xi : input data
-          A batch of the input data.
-
-        yi : target data
-          A batch of the target data.
+        batch
+          A single batch returned by the data loader.
 
         **fit_params : dict
           Additional parameters passed to the ``forward`` method of
           the module and to the ``self.train_split`` call.
 
+        Returns
+        -------
+        step : dict
+          A dictionary ``{'loss': loss, 'y_pred': y_pred}``, where the
+          float ``loss`` is the result of the loss function and
+          ``y_pred`` the prediction generated by the PyTorch module.
+
         """
-        self.module_.train()
+        self._set_training(True)
+        Xi, yi = unpack_data(batch)
         y_pred = self.infer(Xi, **fit_params)
         loss = self.get_loss(y_pred, yi, X=Xi, training=True)
         loss.backward()
-
-        self.notify(
-            'on_grad_computed',
-            named_parameters=TeeGenerator(self.module_.named_parameters()),
-            X=Xi,
-            y=yi
-        )
-
         return {
             'loss': loss,
             'y_pred': y_pred,
-            }
+        }
 
     def get_train_step_accumulator(self):
         """Return the train step accumulator.
 
         By default, the accumulator stores and retrieves the first
         value from the optimizer call. Most optimizers make only one
         call, so first value is at the same time the only value.
@@ -670,61 +1010,131 @@
         loss function is evaluated multiple times per optimizer
         call. If you don't want to return the first value in that
         case, override this method to return your custom accumulator.
 
         """
         return FirstStepAccumulator()
 
-    def train_step(self, Xi, yi, **fit_params):
+    def _zero_grad_optimizer(self, set_to_none=None):
+        """Zero out the gradient of all optimizers.
+
+        Parameters
+        ----------
+        set_to_none : bool or None (default=None)
+          Whether to zero out gradients (default) or to set them to None by
+          passing True. Note that since this option is only available starting
+          from PyTorch 1.7, it is ignored by default (i.e. when its value is
+          None). For skorch to pass this value to the ``zero_grad`` call,
+          override this method and set the value to True or False.
+
+          The advantages and disadvantages of setting this value to True are
+          discussed here:
+
+          https://pytorch.org/docs/stable/optim.html#torch.optim.Optimizer.zero_grad
+
+        """
+        for name in self._optimizers:
+            optimizer = getattr(self, name + '_')
+            if set_to_none is None:
+                optimizer.zero_grad()
+            else:
+                optimizer.zero_grad(set_to_none=set_to_none)
+
+    def _step_optimizer(self, step_fn):
+        """Perform a ``step`` call on all optimizers.
+
+        Parameters
+        ----------
+        step_fn : callable or None
+          If None, just call ``optimizer.step()`` without arguments. Else, this
+          will be passed as the training step closure to the optimizer(s). Note
+          that this could lead to the function being called multiple times. If
+          more fine-grained control is desired instead, please override the
+          :meth:`.train_step` method.
+
+        """
+        for name in self._optimizers:
+            optimizer = getattr(self, name + '_')
+            if step_fn is None:
+                optimizer.step()
+            else:
+                optimizer.step(step_fn)
+
+    def train_step(self, batch, **fit_params):
         """Prepares a loss function callable and pass it to the optimizer,
         hence performing one optimization step.
 
         Loss function callable as required by some optimizers (and accepted by
         all of them):
         https://pytorch.org/docs/master/optim.html#optimizer-step-closure
 
         The module is set to be in train mode (e.g. dropout is
         applied).
 
         Parameters
         ----------
-        Xi : input data
-          A batch of the input data.
-
-        yi : target data
-          A batch of the target data.
+        batch
+          A single batch returned by the data loader.
 
         **fit_params : dict
           Additional parameters passed to the ``forward`` method of
           the module and to the train_split call.
 
+        Returns
+        -------
+        step : dict
+          A dictionary ``{'loss': loss, 'y_pred': y_pred}``, where the
+          float ``loss`` is the result of the loss function and
+          ``y_pred`` the prediction generated by the PyTorch module.
+
         """
         step_accumulator = self.get_train_step_accumulator()
 
         def step_fn():
-            self.optimizer_.zero_grad()
-            step = self.train_step_single(Xi, yi, **fit_params)
+            self._zero_grad_optimizer()
+            step = self.train_step_single(batch, **fit_params)
             step_accumulator.store_step(step)
+
+            self.notify(
+                'on_grad_computed',
+                named_parameters=TeeGenerator(self.get_all_learnable_params()),
+                batch=batch,
+                training=True,
+            )
             return step['loss']
 
-        self.optimizer_.step(step_fn)
+        self._step_optimizer(step_fn)
         return step_accumulator.get_step()
 
-    def evaluation_step(self, Xi, training=False):
+    def evaluation_step(self, batch, training=False):
         """Perform a forward step to produce the output used for
         prediction and scoring.
 
-        Therefore the module is set to evaluation mode by default
+        Therefore, the module is set to evaluation mode by default
         beforehand which can be overridden to re-enable features
         like dropout by setting ``training=True``.
 
+        Parameters
+        ----------
+        batch
+          A single batch returned by the data loader.
+
+        training : bool (default=False)
+          Whether to set the module to train mode or not.
+
+        Returns
+        -------
+        y_infer
+          The prediction generated by the module.
+
         """
         self.check_is_fitted()
+        Xi, _ = unpack_data(batch)
         with torch.set_grad_enabled(training):
-            self.module_.train(training)
+            self._set_training(training)
             return self.infer(Xi)
 
     def fit_loop(self, X, y=None, epochs=None, **fit_params):
         """The proper fit loop.
 
         Contains the logic of what actually happens during the fit
         loop.
@@ -756,67 +1166,73 @@
 
         **fit_params : dict
           Additional parameters passed to the ``forward`` method of
           the module and to the ``self.train_split`` call.
 
         """
         self.check_data(X, y)
+        self.check_training_readiness()
         epochs = epochs if epochs is not None else self.max_epochs
 
         dataset_train, dataset_valid = self.get_split_datasets(
             X, y, **fit_params)
         on_epoch_kwargs = {
             'dataset_train': dataset_train,
             'dataset_valid': dataset_valid,
         }
+        iterator_train = self.get_iterator(dataset_train, training=True)
+        iterator_valid = None
+        if dataset_valid is not None:
+            iterator_valid = self.get_iterator(dataset_valid, training=False)
 
         for _ in range(epochs):
             self.notify('on_epoch_begin', **on_epoch_kwargs)
 
-            self.run_single_epoch(dataset_train, training=True, prefix="train",
+            self.run_single_epoch(iterator_train, training=True, prefix="train",
                                   step_fn=self.train_step, **fit_params)
 
-            if dataset_valid is not None:
-                self.run_single_epoch(dataset_valid, training=False, prefix="valid",
-                                      step_fn=self.validation_step, **fit_params)
+            self.run_single_epoch(iterator_valid, training=False, prefix="valid",
+                                  step_fn=self.validation_step, **fit_params)
 
             self.notify("on_epoch_end", **on_epoch_kwargs)
         return self
 
-    def run_single_epoch(self, dataset, training, prefix, step_fn, **fit_params):
+    def run_single_epoch(self, iterator, training, prefix, step_fn, **fit_params):
         """Compute a single epoch of train or validation.
 
         Parameters
         ----------
-        dataset : torch Dataset
-            The initialized dataset to loop over.
+        iterator : torch DataLoader or None
+          The initialized ``DataLoader`` to loop over. If None, skip this step.
 
         training : bool
-            Whether to set the module to train mode or not.
+          Whether to set the module to train mode or not.
 
         prefix : str
-            Prefix to use when saving to the history.
+          Prefix to use when saving to the history.
 
         step_fn : callable
-            Function to call for each batch.
+          Function to call for each batch.
 
         **fit_params : dict
-            Additional parameters passed to the ``step_fn``.
+          Additional parameters passed to the ``step_fn``.
+
         """
-        is_placeholder_y = uses_placeholder_y(dataset)
+        if iterator is None:
+            return
 
         batch_count = 0
-        for data in self.get_iterator(dataset, training=training):
-            Xi, yi = unpack_data(data)
-            yi_res = yi if not is_placeholder_y else None
-            self.notify("on_batch_begin", X=Xi, y=yi_res, training=training)
-            step = step_fn(Xi, yi, **fit_params)
+        for batch in iterator:
+            self.notify("on_batch_begin", batch=batch, training=training)
+            step = step_fn(batch, **fit_params)
             self.history.record_batch(prefix + "_loss", step["loss"].item())
-            self.history.record_batch(prefix + "_batch_size", get_len(Xi))
-            self.notify("on_batch_end", X=Xi, y=yi_res, training=training, **step)
+            batch_size = (get_len(batch[0]) if isinstance(batch, (tuple, list))
+                          else get_len(batch))
+            self.history.record_batch(prefix + "_batch_size", batch_size)
+            self.notify("on_batch_end", batch=batch, training=training, **step)
             batch_count += 1
 
         self.history.record(prefix + "_batch_count", batch_count)
 
     # pylint: disable=unused-argument
     def partial_fit(self, X, y=None, classes=None, **fit_params):
         """Fit the module.
@@ -917,17 +1333,75 @@
 
         Raises
         ------
         skorch.exceptions.NotInitializedError
           When the given attributes are not present.
 
         """
-        attributes = attributes or ['module_']
+        # first check attributes argument, but if it's empty, check that the
+        # indicated _modules exist, and if those are not defined, assume that
+        # the standard 'module_' attribute should exist
+        attributes = (
+            attributes or [module + '_' for module in self._modules] or ['module_']
+        )
         check_is_fitted(self, attributes, *args, **kwargs)
 
+    def trim_for_prediction(self):
+        """Remove all attributes not required for prediction.
+
+        Use this method after you finished training your net, with the goal of
+        reducing its size. All attributes only required during training (e.g.
+        the optimizer) are set to None. This can lead to a considerable decrease
+        in memory footprint. It also makes it more likely that the net can be
+        loaded with different library versions.
+
+        After calling this function, the net can only be used for prediction
+        (e.g. ``net.predict`` or ``net.predict_proba``) but no longer for
+        training (e.g. ``net.fit(X, y)`` will raise an exception).
+
+        This operation is irreversible. Once the net has been trimmed for
+        prediction, it is no longer possible to restore the original state.
+        Morevoer, this operation mutates the net. If you need the unmodified
+        net, create a deepcopy before trimming:
+
+        .. code:: python
+
+            from copy import deepcopy
+            net = NeuralNet(...)
+            net.fit(X, y)
+            # training finished
+            net_original = deepcopy(net)
+            net.trim_for_prediction()
+            net.predict(X)
+
+        """
+        # pylint: disable=protected-access
+        if getattr(self, '_trimmed_for_prediction', False):
+            return
+
+        self.check_is_fitted()
+        # pylint: disable=attribute-defined-outside-init
+        self._trimmed_for_prediction = True
+        self._set_training(False)
+
+        if isinstance(self.callbacks, list):
+            self.callbacks.clear()
+        self.callbacks_.clear()
+
+        self.train_split = None
+        self.iterator_train = None
+        self.history.clear()
+
+        attrs_to_trim = self._optimizers[:] + self._criteria[:]
+
+        for name in attrs_to_trim:
+            setattr(self, name + '_', None)
+            if hasattr(self, name):
+                setattr(self, name, None)
+
     def forward_iter(self, X, training=False, device='cpu'):
         """Yield outputs of module forward calls on each batch of data.
         The storage device of the yielded tensors is determined
         by the ``device`` parameter.
 
         Parameters
         ----------
@@ -959,17 +1433,16 @@
         ------
         yp : torch tensor
           Result from a forward call on an individual batch.
 
         """
         dataset = self.get_dataset(X)
         iterator = self.get_iterator(dataset, training=training)
-        for data in iterator:
-            Xi = unpack_data(data)[0]
-            yp = self.evaluation_step(Xi, training=training)
+        for batch in iterator:
+            yp = self.evaluation_step(batch, training=training)
             yield to_device(yp, device=device)
 
     def forward(self, X, training=False, device='cpu'):
         """Gather and concatenate the output from forward call with
         input data.
 
         The outputs from ``self.module_.forward`` are gathered on the
@@ -1038,15 +1511,15 @@
 
         **fit_params : dict
           Additional parameters passed to the ``forward`` method of
           the module and to the ``self.train_split`` call.
 
         """
         x = to_tensor(x, device=self.device)
-        if isinstance(x, dict):
+        if isinstance(x, Mapping):
             x_dict = self._merge_x_and_fit_params(x, fit_params)
             return self.module_(**x_dict)
         return self.module_(x, **fit_params)
 
     def _get_predict_nonlinearity(self):
         """Return the nonlinearity to be applied to the prediction
 
@@ -1077,15 +1550,15 @@
 
         """
         self.check_is_fitted()
         nonlin = self.predict_nonlinearity
         if nonlin is None:
             nonlin = _identity
         elif nonlin == 'auto':
-            nonlin = _infer_predict_nonlinearty(self)
+            nonlin = _infer_predict_nonlinearity(self)
         if not callable(nonlin):
             raise TypeError("predict_nonlinearity has to be a callable, 'auto' or None")
         return nonlin
 
     def predict_proba(self, X):
         """Return the output of the module's forward method as a numpy
         array.
@@ -1185,18 +1658,14 @@
           ``Dataset`` that can deal with the data.
 
         training : bool (default=False)
           Whether train mode should be used or not.
 
         """
         y_true = to_tensor(y_true, device=self.device)
-
-        if isinstance(self.criterion_, torch.nn.Module):
-            self.criterion_.train(training)
-
         return self.criterion_(y_pred, y_true)
 
     def get_dataset(self, X, y=None):
         """Get a dataset that contains the input data and is passed to
         the iterator.
 
         Override this if you want to initialize your dataset
@@ -1395,14 +1864,19 @@
                 p = [params.pop(i)[1] for i in reversed(matches)]
                 pgroups.append({'params': p, **group})
 
         if params:
             pgroups.append({'params': [p for _, p in params]})
 
         args = (pgroups,)
+
+        # 'lr' is an optimizer param that can be set without the 'optimizer__'
+        # prefix because it's so common
+        if 'lr' not in kwargs:
+            kwargs['lr'] = self.lr
         return args, kwargs
 
     def get_params_for_optimizer(self, prefix, named_parameters):
         """Collect and return init parameters for an optimizer.
 
         Parse kwargs configuration for the optimizer identified by
         the given prefix. Supports param group assignment using wildcards:
@@ -1460,15 +1934,15 @@
           rate.
 
         """
         args, kwargs = self._get_params_for_optimizer(prefix, named_parameters)
         return args, kwargs
 
     def _get_param_names(self):
-        return (k for k in self.__dict__ if not k.endswith('_'))
+        return [k for k in self.__dict__ if not k.endswith('_')]
 
     def _get_params_callbacks(self, deep=True):
         """sklearn's .get_params checks for `hasattr(value,
         'get_params')`. This returns False for a list. But our
         callbacks reside within a list. Hence their parameters have to
         be retrieved separately.
         """
@@ -1489,46 +1963,62 @@
 
     def get_params(self, deep=True, **kwargs):
         params = BaseEstimator.get_params(self, deep=deep, **kwargs)
         # Callback parameters are not returned by .get_params, needs
         # special treatment.
         params_cb = self._get_params_callbacks(deep=deep)
         params.update(params_cb)
-        return params
 
-    def _check_kwargs(self, kwargs):
+        # don't include the following attributes
+        to_exclude = {'_modules', '_criteria', '_optimizers'}
+        return {key: val for key, val in params.items() if key not in to_exclude}
+
+    def _validate_params(self):
         """Check argument names passed at initialization.
 
+        Note: This method is similar to
+        :meth:`sklearn.base.BaseEstimator._validate_params` but doesn't use its
+        machinery.
+
         Raises
         ------
-        TypeError
-          Raises a TypeError if one or more arguments don't seem to
+        ValueError
+          Raises a ValueError if one or more arguments don't seem to
           match or are malformed.
 
-        Returns
-        -------
-        kwargs: dict
-          Return the passed keyword arguments.
-
         Example
         -------
         >>> net = NeuralNetClassifier(MyModule, iterator_train_shuffle=True)
-        TypeError: Got an unexpected argument iterator_train_shuffle,
+        ValueError: Got an unexpected argument iterator_train_shuffle,
         did you mean iterator_train__shuffle?
 
         """
+        # warn about usage of iterator_valid__shuffle=True, since this
+        # is almost certainly not what the user wants
+        if 'iterator_valid__shuffle' in self._params_to_validate:
+            if self.iterator_valid__shuffle:
+                warnings.warn(
+                    "You set iterator_valid__shuffle=True; this is most likely not "
+                    "what you want because the values returned by predict and "
+                    "predict_proba will be shuffled.",
+                    UserWarning)
+
+        # check for wrong arguments
         unexpected_kwargs = []
         missing_dunder_kwargs = []
-        for key in kwargs:
+        for key in sorted(self._params_to_validate):
             if key.endswith('_'):
                 continue
 
             # see https://github.com/skorch-dev/skorch/pull/590 for
             # why this must be sorted
             for prefix in sorted(self.prefixes_, key=lambda s: (-len(s), s)):
+                if key == prefix:
+                    # e.g. someone did net.set_params(callbacks=[])
+                    break
                 if key.startswith(prefix):
                     if not key.startswith(prefix + '__'):
                         missing_dunder_kwargs.append((prefix, key))
                     break
             else:  # no break means key didn't match a prefix
                 unexpected_kwargs.append(key)
 
@@ -1543,19 +2033,24 @@
 
         for prefix, key in sorted(missing_dunder_kwargs, key=lambda tup: tup[1]):
             tmpl = "Got an unexpected argument {}, did you mean {}?"
             suffix = key[len(prefix):].lstrip('_')
             suggestion = prefix + '__' + suffix
             msgs.append(tmpl.format(key, suggestion))
 
+        valid_vals_use_caching = ('auto', False, True)
+        if self.use_caching not in valid_vals_use_caching:
+            msgs.append(
+                f"Incorrect value for use_caching used ('{self.use_caching}'), "
+                f"use one of: {', '.join(map(str, valid_vals_use_caching))}"
+            )
+
         if msgs:
             full_msg = '\n'.join(msgs)
-            raise TypeError(full_msg)
-
-        return kwargs
+            raise ValueError(full_msg)
 
     def _check_deprecated_params(self, **kwargs):
         pass
 
     def set_params(self, **kwargs):
         """Set the parameters of this class.
 
@@ -1571,63 +2066,103 @@
         virtual_params = {}
 
         for key, val in kwargs.items():
             if self._is_virtual_param(key):
                 virtual_params[key] = val
             elif key.startswith('callbacks'):
                 cb_params[key] = val
+                self._params_to_validate.add(key)
             elif any(key.startswith(prefix) for prefix in self.prefixes_):
                 special_params[key] = val
+                self._params_to_validate.add(key)
+            elif '__' in key:
+                special_params[key] = val
+                self._params_to_validate.add(key)
             else:
                 normal_params[key] = val
 
         self._apply_virtual_params(virtual_params)
         BaseEstimator.set_params(self, **normal_params)
 
         for key, val in special_params.items():
             if key.endswith('_'):
                 raise ValueError(
                     "Something went wrong here. Please open an issue on "
                     "https://github.com/skorch-dev/skorch/issues detailing what "
                     "caused this error.")
             setattr(self, key, val)
 
-        # Below: Re-initialize parts of the net if necessary.
-
         if cb_params:
             # callbacks need special treatmeant since they are list of tuples
-            self.initialize_callbacks()
+            self._initialize_callbacks()
             self._set_params_callback(**cb_params)
+            vars(self).update(cb_params)
 
-        if any('criterion' in key.split('__', 1)[0] for key in special_params):
-            self.initialize_criterion()
-
-        module_triggers_optimizer_reinit = False
-        if any('module' in key.split('__', 1)[0] for key in special_params):
-            self.initialize_module()
-            module_triggers_optimizer_reinit = True
+        # If the net is not initialized or there are no special params, we can
+        # exit as this point, because the special_params have been set as
+        # attributes and will be applied by initialize() at a later point in
+        # time.
+        if not self.initialized_ or not special_params:
+            return self
+
+        # if net is initialized, checking kwargs is possible
+        self._validate_params()
+
+        ######################################################
+        # Below: Re-initialize parts of the net if necessary #
+        ######################################################
+
+        # if there are module params, reinit module, criterion, optimizer
+        # if there are criterion params, reinit criterion, optimizer
+        # optimizer params don't need to be checked, as they are virtual
+        reinit_module = False
+        reinit_criterion = False
+        reinit_optimizer = False
+
+        component_names = {key.split('__', 1)[0] for key in special_params}
+        for prefix in component_names:
+            if (prefix in self._modules) or (prefix == 'compile'):
+                reinit_module = True
+                reinit_criterion = True
+                reinit_optimizer = True
+
+                module_params = {k: v for k, v in special_params.items()
+                                 if k.startswith(prefix)}
+                msg_module = self._format_reinit_msg(
+                    "module", module_params, triggered_directly=True)
+                msg_criterion = self._format_reinit_msg(
+                    "criterion", triggered_directly=False)
+                msg_optimizer = self._format_reinit_msg(
+                    "optimizer", triggered_directly=False)
 
-        optimizer_changed = (
-            any('optimizer' in key.split('__', 1)[0] for key in special_params)
-            or 'lr' in normal_params
-        )
-        if module_triggers_optimizer_reinit or optimizer_changed:
-            # Model selectors such as GridSearchCV will set the
-            # parameters before .initialize() is called, therefore we
-            # need to make sure that we have an initialized model here
-            # as the optimizer depends on it.
-            if not hasattr(self, 'module_'):
-                self.initialize_module()
-
-            # If we reached this point but the optimizer was not
-            # changed, it means that optimizer initialization was
-            # triggered indirectly.
-            self.initialize_optimizer(triggered_directly=optimizer_changed)
+                # if any module is modified, everything needs to be
+                # re-initialized, no need to check any further
+                break
 
-        vars(self).update(kwargs)
+            if prefix in self._criteria:
+                reinit_criterion = True
+                reinit_optimizer = True
+
+                criterion_params = {k: v for k, v in special_params.items()
+                                    if k.startswith(prefix)}
+                msg_criterion = self._format_reinit_msg(
+                    "criterion", criterion_params, triggered_directly=True)
+                msg_optimizer = self._format_reinit_msg(
+                    "optimizer", triggered_directly=False)
+
+        if not (reinit_module or reinit_criterion or reinit_optimizer):
+            raise ValueError("Something went wrong, please open an issue on "
+                             "https://github.com/skorch-dev/skorch/issues")
+
+        if reinit_module:
+            self._initialize_module(reason=msg_module)
+        if reinit_criterion:
+            self._initialize_criterion(reason=msg_criterion)
+        if reinit_optimizer:
+            self._initialize_optimizer(reason=msg_optimizer)
 
         return self
 
     def _set_params_callback(self, **params):
         """Special handling for setting params on callbacks."""
         # model after sklearn.utils._BaseCompostion._set_params
         # 1. All steps
@@ -1699,98 +2234,154 @@
         state.pop('__cuda_dependent_attributes__')
 
         self.__dict__.update(state)
 
     def _register_attribute(
             self,
             name,
+            attr,
             prefixes=True,
             cuda_dependent_attributes=True,
     ):
-        """Add attribute name to prefixes_ and
-        cuda_dependent_attributes_.
+        """Add attribute name to prefixes_ and cuda_dependent_attributes_,
+        keep track of modules, criteria, and optimizers.
 
-        The first is to take care that the attribute works correctly
-        with set_params, e.g. when it comes to re-initialization.
+        Keeping track of prefxies is to take care that the attribute works
+        correctly with set_params, e.g. when it comes to re-initialization.
 
-        The second is to make sure that nets trained with CUDA can be
-        loaded without CUDA.
+        Keeping track of cuda dependent attributes is to make sure that nets
+        trained with CUDA can be loaded without CUDA.
 
         This method takes care of not mutating the lists.
 
         Parameters
         ----------
+        name : str
+          Name of the attribute.
+
+        attr : torch.nn.Module or torch.optim.Optimizer
+          The attribute itself.
+
         prefixes : bool (default=True)
           Whether to add to prefixes_.
 
         cuda_dependent_attributes : bool (default=True)
           Whether to add to cuda_dependent_attributes_.
 
         """
-        # copy the lists to avoid mutation
+        name = name.rstrip('_')  # module_ -> module
+
+        # Always copy the collections to avoid mutation
         if prefixes:
             self.prefixes_ = self.prefixes_[:] + [name]
 
         if cuda_dependent_attributes:
             self.cuda_dependent_attributes_ = (
                 self.cuda_dependent_attributes_[:] + [name + '_'])
 
+        # make sure to not double register -- this should never happen, but
+        # still better to check
+        if (self.init_context_ == 'module') and (name not in self._modules):
+            self._modules = self._modules[:] + [name]
+        elif (self.init_context_ == 'criterion') and (name not in self._criteria):
+            self._criteria = self._criteria[:] + [name]
+        elif (self.init_context_ == 'optimizer') and (name not in self._optimizers):
+            self._optimizers = self._optimizers[:] + [name]
+
     def _unregister_attribute(
             self,
             name,
             prefixes=True,
             cuda_dependent_attributes=True,
     ):
-        """Remove attribute name from prefixes_ and
-        cuda_dependent_attributes_.
+        """Remove attribute name from prefixes_, cuda_dependent_attributes_ and the
+        _modules/_criteria/_optimizers list if applicable.
 
         Use this to remove PyTorch components that are not needed
         anymore. This is mostly a clean up job, so as to not leave
         unnecessary prefixes or cuda-dependent attributes.
 
         This method takes care of not mutating the lists.
 
         Parameters
         ----------
+        name : str
+          Name of the attribute.
+
         prefixes : bool (default=True)
           Whether to remove from prefixes_.
 
         cuda_dependent_attributes : bool (default=True)
           Whether to remove from cuda_dependent_attributes_.
 
         """
+        name = name.rstrip('_')  # module_ -> module
+
         # copy the lists to avoid mutation
         if prefixes:
             self.prefixes_ = [p for p in self.prefixes_ if p != name]
 
         if cuda_dependent_attributes:
             self.cuda_dependent_attributes_ = [
                 a for a in self.cuda_dependent_attributes_ if a != name + '_']
 
+        if name in self._modules:
+            self._modules = [p for p in self._modules if p != name]
+        if name in self._criteria:
+            self._criteria = [p for p in self._criteria if p != name]
+        if name in self._optimizers:
+            self._optimizers = [p for p in self._optimizers if p != name]
+
+    def _check_settable_attr(self, name, attr):
+        """Check whether this attribute is valid for it to be settable.
+
+        E.g. for it to work with set_params.
+
+        """
+        if (self.init_context_ is None) and isinstance(attr, torch.nn.Module):
+            msg = ("Trying to set torch compoment '{}' outside of an initialize method."
+                   " Consider defining it inside 'initialize_module'".format(name))
+            raise SkorchAttributeError(msg)
+
+        if (self.init_context_ is None) and isinstance(attr, torch.optim.Optimizer):
+            msg = ("Trying to set torch compoment '{}' outside of an initialize method."
+                   " Consider defining it inside 'initialize_optimizer'".format(name))
+            raise SkorchAttributeError(msg)
+
+        if not name.endswith('_'):
+            msg = ("Names of initialized modules or optimizers should end "
+                   "with an underscore (e.g. '{}_')".format(name))
+            raise SkorchAttributeError(msg)
+
     def __setattr__(self, name, attr):
         """Set an attribute on the net
 
         When a custom net with additional torch modules or optimizers
         is created, those attributes are added to ``prefixes_`` and
         ``cuda_dependent_attributes_`` automatically.
 
+        These components are also tracked to correctly set the device.
+
         """
         # If it's a
         # 1. known attribute or
         # 2. special param like module__num_units or
-        # 3. not a torch module/optimizer instance or class
+        # 3. the net is being __init__-ialized
+        # 4. not a torch module/optimizer instance or class
         # just setattr as usual.
         # For a discussion why we chose this implementation, see here:
         # https://github.com/skorch-dev/skorch/pull/597
-        is_known = name.endswith('_') or (name in self.prefixes_)
+        is_known = name in self.prefixes_ or name.rstrip('_') in self.prefixes_
         is_special_param = '__' in name
-        is_torch_component = any(c in name for c in _PYTORCH_COMPONENTS)
+        first_init = not hasattr(self, 'initialized_')
+        is_torch_component = isinstance(attr, (torch.nn.Module, torch.optim.Optimizer))
 
-        if not (is_known or is_special_param) and is_torch_component:
-            self._register_attribute(name)
+        if not (is_known or is_special_param or first_init) and is_torch_component:
+            self._check_settable_attr(name, attr)
+            self._register_attribute(name, attr)
         super().__setattr__(name, attr)
 
     def __delattr__(self, name):
         # take extra precautions to undo the changes made in __setattr__
         self._unregister_attribute(name)
         super().__delattr__(name)
 
@@ -1819,14 +2410,15 @@
 
     def save_params(
             self,
             f_params=None,
             f_optimizer=None,
             f_criterion=None,
             f_history=None,
+            use_safetensors=False,
             **kwargs):
         """Saves the module's parameters, history, and optimizer,
         not the whole object.
 
         To save the whole object, use pickle. This is necessary when
         you need additional learned attributes on the net, e.g. the
         ``classes_`` attribute on
@@ -1848,64 +2440,103 @@
 
         f_criterion : file-like object, str, None (default=None)
           Path of criterion. Pass ``None`` to not save
 
         f_history : file-like object, str, None (default=None)
           Path to history. Pass ``None`` to not save
 
+        use_safetensors : bool (default=False)
+          Whether to use the ``safetensors`` library to persist the state. By
+          default, PyTorch is used, which in turn uses :mod:`pickle` under the
+          hood. When enabling ``safetensors``, be aware that only PyTorch
+          tensors can be stored. Therefore, certain attributes like the
+          optimizer cannot be saved.
+
         Examples
         --------
         >>> before = NeuralNetClassifier(mymodule)
         >>> before.save_params(f_params='model.pkl',
         ...                    f_optimizer='optimizer.pkl',
         ...                    f_history='history.json')
         >>> after = NeuralNetClassifier(mymodule).initialize()
         >>> after.load_params(f_params='model.pkl',
         ...                   f_optimizer='optimizer.pkl',
         ...                   f_history='history.json')
 
         """
+        if use_safetensors:
+            def _save_state_dict(state_dict, f_name):
+                from safetensors.torch import save_file, save
+                try:
+                    if isinstance(f_name, (str, os.PathLike)):
+                        save_file(state_dict, f_name)
+                    else:  # file
+                        as_bytes = save(state_dict)
+                        f_name.write(as_bytes)
+                except ValueError as exc:
+                    msg = (
+                        f"You are trying to store {f_name} using safetensors "
+                        "but there was an error. Safetensors can only store "
+                        "tensors, not generic Python objects (as e.g. optimizer "
+                        "states). If you want to store generic Python objects, "
+                        "don't use safetensors."
+                    )
+                    raise ValueError(msg) from exc
+        else:
+            def _save_state_dict(state_dict, f_name):
+                torch.save(module.state_dict(), f_name)
+
         kwargs_module, kwargs_other = _check_f_arguments(
             'save_params',
             f_params=f_params,
             f_optimizer=f_optimizer,
             f_criterion=f_criterion,
             f_history=f_history,
             **kwargs)
 
         if not kwargs_module and not kwargs_other:
-            print("Nothing to save")
+            if self.verbose:
+                print("Nothing to save")
             return
 
         msg_init = (
             "Cannot save state of an un-initialized model. "
             "Please initialize first by calling .initialize() "
             "or by fitting the model with .fit(...).")
         msg_module = (
             "You are trying to save 'f_{name}' but for that to work, the net "
             "needs to have an attribute called 'net.{name}_' that is a PyTorch "
-            "Module; make sure that it exists and check for typos.")
+            "Module or Optimizer; make sure that it exists and check for typos.")
 
         for attr, f_name in kwargs_module.items():
             # valid attrs can be 'module_', 'optimizer_', etc.
-            if attr[:-1] in self.prefixes_:
+            if attr.endswith('_') and not self.initialized_:
                 self.check_is_fitted([attr], msg=msg_init)
             module = self._get_module(attr, msg=msg_module)
-            torch.save(module.state_dict(), f_name)
+            _save_state_dict(module.state_dict(), f_name)
 
         # only valid key in kwargs_other is f_history
         f_history = kwargs_other.get('f_history')
         if f_history is not None:
             self.history.to_file(f_history)
 
     def _check_device(self, requested_device, map_device):
         """Compare the requested device with the map device and
         return the map device if it differs from the requested device
         along with a warning.
         """
+        if requested_device is None:
+            # user has set net.device=None, we don't know the type, use fallback
+            msg = (
+                f"Setting self.device = {map_device} since the requested device "
+                f"was not specified"
+            )
+            warnings.warn(msg, DeviceWarning)
+            return map_device
+
         type_1 = torch.device(requested_device)
         type_2 = torch.device(map_device)
         if type_1 != type_2:
             warnings.warn(
                 'Setting self.device = {} since the requested device ({}) '
                 'is not available.'.format(map_device, requested_device),
                 DeviceWarning)
@@ -1917,14 +2548,15 @@
     def load_params(
             self,
             f_params=None,
             f_optimizer=None,
             f_criterion=None,
             f_history=None,
             checkpoint=None,
+            use_safetensors=False,
             **kwargs):
         """Loads the the module's parameters, history, and optimizer,
         not the whole object.
 
         To save and load the whole object, use pickle.
 
         ``f_params``, ``f_optimizer``, etc. uses PyTorch's
@@ -1948,30 +2580,54 @@
           Path to history. Pass ``None`` to not load.
 
         checkpoint : :class:`.Checkpoint`, None (default=None)
           Checkpoint to load params from. If a checkpoint and a ``f_*``
           path is passed in, the ``f_*`` will be loaded. Pass
           ``None`` to not load.
 
+        use_safetensors : bool (default=False)
+          Whether to use the ``safetensors`` library to load the state. By
+          default, PyTorch is used, which in turn uses :mod:`pickle` under the
+          hood. When the state was saved with ``safetensors=True`` when
+          :meth:`skorch.net.NeuralNet.save_params` was called, it should be set
+          to ``True`` here as well.
+
         Examples
         --------
         >>> before = NeuralNetClassifier(mymodule)
         >>> before.save_params(f_params='model.pkl',
         >>>                    f_optimizer='optimizer.pkl',
         >>>                    f_history='history.json')
         >>> after = NeuralNetClassifier(mymodule).initialize()
         >>> after.load_params(f_params='model.pkl',
         >>>                   f_optimizer='optimizer.pkl',
         >>>                   f_history='history.json')
 
         """
-        def _get_state_dict(f):
-            map_location = get_map_location(self.device)
-            self.device = self._check_device(self.device, map_location)
-            return torch.load(f, map_location=map_location)
+        if use_safetensors:
+            def _get_state_dict(f_name):
+                from safetensors import safe_open
+                from safetensors.torch import load
+
+                if isinstance(f_name, (str, os.PathLike)):
+                    state_dict = {}
+                    with safe_open(f_name, framework='pt', device=self.device) as f:
+                        for key in f.keys():
+                            state_dict[key] = f.get_tensor(key)
+                else:
+                    # file
+                    as_bytes = f_name.read()
+                    state_dict = load(as_bytes)
+
+                return state_dict
+        else:
+            def _get_state_dict(f_name):
+                map_location = get_map_location(self.device)
+                self.device = self._check_device(self.device, map_location)
+                return torch.load(f_name, map_location=map_location)
 
         kwargs_full = {}
         if checkpoint is not None:
             if not self.initialized_:
                 self.initialize()
             if f_history is None and checkpoint.f_history is not None:
                 self.history = History.from_file(checkpoint.f_history_)
@@ -1983,34 +2639,35 @@
                          ('f_criterion', f_criterion), ('f_history', f_history)]:
             if val:
                 kwargs_full[key] = val
 
         kwargs_module, kwargs_other = _check_f_arguments('load_params', **kwargs_full)
 
         if not kwargs_module and not kwargs_other:
-            print("Nothing to load")
+            if self.verbose:
+                print("Nothing to load")
             return
 
         # only valid key in kwargs_other is f_history
         f_history = kwargs_other.get('f_history')
         if f_history is not None:
             self.history = History.from_file(f_history)
 
         msg_init = (
             "Cannot load state of an un-initialized model. "
             "Please initialize first by calling .initialize() "
             "or by fitting the model with .fit(...).")
         msg_module = (
             "You are trying to load 'f_{name}' but for that to work, the net "
             "needs to have an attribute called 'net.{name}_' that is a PyTorch "
-            "Module; make sure that it exists and check for typos.")
+            "Module or Optimizer; make sure that it exists and check for typos.")
 
         for attr, f_name in kwargs_module.items():
             # valid attrs can be 'module_', 'optimizer_', etc.
-            if attr[:-1] in self.prefixes_:
+            if attr.endswith('_') and not self.initialized_:
                 self.check_is_fitted([attr], msg=msg_init)
             module = self._get_module(attr, msg=msg_module)
             state_dict = _get_state_dict(f_name)
             module.load_state_dict(state_dict)
 
     def __repr__(self):
         to_include = ['module']
```

### Comparing `skorch-0.9.0/skorch/regressor.py` & `skorch-1.0.0/skorch/regressor.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,23 +62,14 @@
                              "(and your validation) and supply it using the "
                              "``iterator_train`` and ``iterator_valid`` "
                              "parameters respectively.")
         if y is None:
             # The user implements its own mechanism for generating y.
             return
 
-        if get_dim(y) == 1:
-            msg = (
-                "The target data shouldn't be 1-dimensional but instead have "
-                "2 dimensions, with the second dimension having the same size "
-                "as the number of regression targets (usually 1). Please "
-                "reshape your target data to be 2-dimensional "
-                "(e.g. y = y.reshape(-1, 1).")
-            raise ValueError(msg)
-
     # pylint: disable=signature-differs
     def fit(self, X, y, **fit_params):
         """See ``NeuralNet.fit``.
 
         In contrast to ``NeuralNet.fit``, ``y`` is non-optional to
         avoid mistakenly forgetting about ``y``. However, ``y`` can be
         set to ``None`` in case it is derived dynamically from
```

### Comparing `skorch-0.9.0/skorch/scoring.py` & `skorch-1.0.0/skorch/scoring.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+"""Custom scoring functions"""
+
 import numpy as np
-from skorch.net import NeuralNet
+
 from skorch.dataset import unpack_data
 
 
-def loss_scoring(net: NeuralNet, X, y=None, sample_weight=None):
+def loss_scoring(net, X, y=None, sample_weight=None):
     """Calculate score using the criterion of the net
-    
+
     Use the exact same logic as during model training to calculate the score.
 
     This function can be used to implement the ``score`` method for a
     :class:`.NeuralNet` through sub-classing. This is useful, for example, when
     combining skorch models with sklearn objects that rely on the model's
     ``score`` method. For example:
 
@@ -28,14 +30,15 @@
           * numpy arrays
           * torch tensors
           * pandas DataFrame or Series
           * scipy sparse CSR matrices
           * a dictionary of the former three
           * a list/tuple of the former three
           * a Dataset
+
         If this doesn't work with your data, you have to pass a
         ``Dataset`` that can deal with the data.
 
     y : target data, compatible with skorch.dataset.Dataset
         The same data types as for ``X`` are supported. If your X is a Dataset
         that contains the target, ``y`` may be set to None.
 
@@ -62,17 +65,18 @@
     history = {"loss": [], "batch_size": []}
     reduction = net.criterion_.reduction
     if reduction not in ["mean", "sum", "none"]:
         raise ValueError(
             "Expected one of 'mean', 'sum' or 'none' "
             "for reduction but got {reduction}.".format(reduction=reduction)
         )
-    for data in iterator:
-        Xi, yi = unpack_data(data)
-        yp = net.evaluation_step(Xi, training=False)
+
+    for batch in iterator:
+        yp = net.evaluation_step(batch, training=False)
+        yi = unpack_data(batch)[1]
         loss = net.get_loss(yp, yi)
         if reduction == "none":
             loss_value = loss.detach().cpu().numpy()
         else:
             loss_value = loss.item()
         history["loss"].append(loss_value)
         history["batch_size"].append(yi.size(0))
```

### Comparing `skorch-0.9.0/skorch/setter.py` & `skorch-1.0.0/skorch/setter.py`

 * *Files identical despite different names*

### Comparing `skorch-0.9.0/skorch/tests/conftest.py` & `skorch-1.0.0/skorch/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Contains shared fixtures, hooks, etc."""
 
-from unittest.mock import Mock
-
 import numpy as np
 import pytest
 from sklearn.datasets import make_classification
 from sklearn.datasets import make_regression
 from sklearn.preprocessing import StandardScaler
 import torch
 from torch import nn
@@ -146,14 +144,23 @@
     # pylint: disable=unused-import
     import neptune
 
     neptune_installed = True
 except ImportError:
     pass
 
+sacred_installed = False
+try:
+    # pylint: disable=unused-import
+    import sacred
+
+    sacred_installed = True
+except ImportError:
+    pass
+
 wandb_installed = False
 try:
     # pylint: disable=unused-import
     import wandb
 
     wandb_installed = True
 except ImportError:
@@ -172,7 +179,17 @@
 try:
     # pylint: disable=unused-import
     import tensorboard
 
     tensorboard_installed = True
 except ImportError:
     pass
+
+mlflow_installed = False
+try:
+    # pylint: disable=unused-import
+    import mlflow
+
+    mlflow_installed = True
+except ImportError:
+    pass
+
```

### Comparing `skorch-0.9.0/skorch/tests/test_cli.py` & `skorch-1.0.0/skorch/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -249,14 +249,63 @@
             '<MLPModule> options',
             '--net__module__hidden_units : int (default=55)'
         ]
         for snippet in expected_snippets:
             assert snippet in out
 
     @pytest.fixture
+    def clf_sklearn(self):
+        from sklearn.linear_model import LinearRegression
+        return LinearRegression()
+
+    @pytest.fixture
+    def pipe_sklearn(self, clf_sklearn):
+        return Pipeline([
+            ('features', FeatureUnion([
+                ('scale', MinMaxScaler()),
+            ])),
+            ('clf', clf_sklearn),
+        ])
+
+    def test_print_help_sklearn_estimator(self, print_help, clf_sklearn, capsys):
+        # Should also work with non-skorch sklearn estimator;
+        # need to assert that count==1 since there was a bug in my
+        # first implementation that resulted in the help for the final
+        # estimator appearing twice.
+        print_help(clf_sklearn)
+        out = capsys.readouterr()[0]
+
+        expected_snippets = [
+            '-- --help',
+            '--fit_intercept',
+            '--copy_X',
+        ]
+        for snippet in expected_snippets:
+            assert snippet in out
+            assert out.count(snippet) == 1
+
+    def test_print_help_sklearn_pipeline(self, print_help, pipe_sklearn, capsys):
+        # Should also work with non-skorch sklearn pipelines;
+        # need to assert that count==1 since there was a bug in my
+        # first implementation that resulted in the help for the final
+        # estimator appearing twice.
+        print_help(pipe_sklearn)
+        out = capsys.readouterr()[0]
+
+        expected_snippets = [
+            '-- --help',
+            '<MinMaxScaler> options',
+            '--features__scale__feature_range',
+            '--clf__fit_intercept',
+        ]
+        for snippet in expected_snippets:
+            assert snippet in out
+            assert out.count(snippet) == 1
+
+    @pytest.fixture
     def parse_args(self):
         from skorch.cli import parse_args
         return parse_args
 
     @pytest.fixture
     def estimator(self, net_cls):
         mock = Mock(net_cls)
@@ -282,38 +331,52 @@
         assert estimator.set_params.call_count == 2  # defaults and kwargs
 
         defaults_set_params = estimator.set_params.call_args_list[0][1]
         assert not defaults_set_params  # no defaults specified
 
         kwargs_set_params = estimator.set_params.call_args_list[1][1]
         assert kwargs_set_params['foo'] == 'bar'
+        # pylint: disable=comparison-with-callable
         assert kwargs_set_params['baz'] == cos
 
         assert help_.call_count == 0
         assert exit_.call_count == 0
 
     def test_parse_args_net_custom_defaults(self, parse_args, net):
         defaults = {'batch_size': 256, 'module__hidden_units': 55}
         kwargs = {'batch_size': 123, 'module__nonlin': nn.Hardtanh(1, 2)}
         parsed = parse_args(kwargs, defaults)
         net = parsed(net)
 
         # cmd line args have precedence over defaults
         assert net.batch_size == 123
-        assert net.module_.hidden_units == 55
-        assert isinstance(net.module_.nonlin, nn.Hardtanh)
-        assert net.module_.nonlin.min_val == 1
-        assert net.module_.nonlin.max_val == 2
+        assert net.module__hidden_units == 55
+        assert isinstance(net.module__nonlin, nn.Hardtanh)
+        assert net.module__nonlin.min_val == 1
+        assert net.module__nonlin.max_val == 2
 
     def test_parse_args_pipe_custom_defaults(self, parse_args, pipe):
         defaults = {'net__batch_size': 256, 'net__module__hidden_units': 55}
         kwargs = {'net__batch_size': 123, 'net__module__nonlin': nn.Hardtanh(1, 2)}
         parsed = parse_args(kwargs, defaults)
         pipe = parsed(pipe)
         net = pipe.steps[-1][1]
 
         # cmd line args have precedence over defaults
         assert net.batch_size == 123
-        assert net.module_.hidden_units == 55
-        assert isinstance(net.module_.nonlin, nn.Hardtanh)
-        assert net.module_.nonlin.min_val == 1
-        assert net.module_.nonlin.max_val == 2
+        assert net.module__hidden_units == 55
+        assert isinstance(net.module__nonlin, nn.Hardtanh)
+        assert net.module__nonlin.min_val == 1
+        assert net.module__nonlin.max_val == 2
+
+    def test_parse_args_sklearn_pipe_custom_defaults(self, parse_args, pipe_sklearn):
+        defaults = {'features__scale__copy': 123, 'clf__fit_intercept': 456}
+        kwargs = {'features__scale__copy': 555, 'clf__n_jobs': 5}
+        parsed = parse_args(kwargs, defaults)
+        pipe = parsed(pipe_sklearn)
+        scaler = pipe.steps[0][1].transformer_list[0][1]
+        clf = pipe.steps[-1][1]
+
+        # cmd line args have precedence over defaults
+        assert scaler.copy == 555
+        assert clf.fit_intercept == 456
+        assert clf.n_jobs == 5
```

### Comparing `skorch-0.9.0/skorch/tests/test_dataset.py` & `skorch-1.0.0/skorch/tests/test_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Tests for dataset.py."""
 
+import unittest
 from unittest.mock import Mock
 
 import numpy as np
 import pytest
+from scipy import sparse
 from sklearn.datasets import make_classification
 import torch
 import torch.utils.data
 from torch import nn
 import torch.nn.functional as F
 from torch.utils.data import DataLoader
 
-from scipy import sparse
 from skorch.utils import data_from_dataset
 from skorch.utils import is_torch_data_type
 from skorch.utils import to_tensor
 from skorch.tests.conftest import pandas_installed
 
 
 class TestGetLen:
@@ -61,99 +62,24 @@
         {'0': [0, 1, 2], '1': (3, 4)},
         ([0, 1, 2], np.zeros(3), torch.zeros(2), {'0': (1, 2, 3)}),
     ])
     def test_inconsistent_lengths(self, get_len, data):
         with pytest.raises(ValueError):
             get_len(data)
 
+    def test_get_len_transformers_tokenizer(self, get_len):
+        transformers = pytest.importorskip('transformers')
 
-class TestUsesPlaceholderY:
-
-    @pytest.fixture
-    def uses_placeholder_y(self):
-        from skorch.dataset import uses_placeholder_y
-        return uses_placeholder_y
-
-    @pytest.fixture
-    def dataset_cls(self):
-        from skorch.dataset import Dataset
-        return Dataset
-
-    @pytest.fixture
-    def custom_dataset_cls(self):
-        from skorch.dataset import Dataset
-        class CustomDataset(Dataset):
-            # pylint: disable=super-init-not-called
-            def __init__(self):
-                pass
-        return CustomDataset
-
-    @pytest.fixture
-    def cv_split_cls(self):
-        from skorch.dataset import CVSplit
-        return CVSplit
-
-    def test_dataset_uses_y_placeholder(
-            self, dataset_cls, data, uses_placeholder_y):
-        X, _ = data
-        ds = dataset_cls(X, y=None)
-        assert uses_placeholder_y(ds)
-
-    def test_dataset_uses_non_y_placeholder(
-            self, dataset_cls, data, uses_placeholder_y):
-        X, y = data
-        ds = dataset_cls(X, y)
-        assert not uses_placeholder_y(ds)
-
-    def test_custom_dataset_uses_non_y_placeholder(
-            self, custom_dataset_cls, uses_placeholder_y):
-        ds = custom_dataset_cls()
-        assert not uses_placeholder_y(ds)
-
-    def test_subset_uses_placeholder_y(
-            self, dataset_cls, data, uses_placeholder_y,
-            cv_split_cls):
-        X, _ = data
-        ds = dataset_cls(X, y=None)
-        ds_train, ds_valid = cv_split_cls(cv=2)(ds)
-        assert uses_placeholder_y(ds_train)
-        assert uses_placeholder_y(ds_valid)
-
-    def test_subset_dataset_uses_non_y_placeholder(
-            self, dataset_cls, data, uses_placeholder_y,
-            cv_split_cls):
-        X, y = data
-        ds = dataset_cls(X, y)
-        ds_train, ds_valid = cv_split_cls(cv=2)(ds)
-        assert not uses_placeholder_y(ds_train)
-        assert not uses_placeholder_y(ds_valid)
-
-    def test_subset_of_subset_uses_placeholder_y(
-            self, dataset_cls, data, uses_placeholder_y,
-            cv_split_cls):
-        X, _ = data
-        ds = dataset_cls(X, y=None)
-        ds_split, _ = cv_split_cls(cv=4)(ds)
-        ds_train, ds_valid = cv_split_cls(cv=3)(ds_split)
-        assert uses_placeholder_y(ds_train)
-        assert uses_placeholder_y(ds_valid)
-
-    def test_subset_of_subset_uses_non_placeholder_y(
-            self, dataset_cls, data, uses_placeholder_y,
-            cv_split_cls):
-        X, y = data
-        ds = dataset_cls(X, y)
-        ds_split, _ = cv_split_cls(cv=4)(ds)
-        ds_train, ds_valid = cv_split_cls(cv=3)(ds_split)
-        assert not uses_placeholder_y(ds_train)
-        assert not uses_placeholder_y(ds_valid)
+        X = ['hello there'] * 10
+        tokenizer = transformers.AutoTokenizer.from_pretrained('bert-base-uncased')
+        tokens = tokenizer(X)
+        assert get_len(tokens) == 10
 
 
 class TestNetWithoutY:
-
     net_fixture_params = [
         {'classification': True, 'batch_size': 1},
         {'classification': False, 'batch_size': 1},
         {'classification': True, 'batch_size': 2},
         {'classification': False, 'batch_size': 2},
     ]
 
@@ -189,16 +115,16 @@
             def __iter__(self):
                 z = super().__iter__()
                 return ((x, torch.zeros(x.size(0), 1).float()) for x, _ in z)
         return Loader
 
     @pytest.fixture
     def train_split(self):
-        from skorch.dataset import CVSplit
-        return CVSplit(0.2, stratified=False)
+        from skorch.dataset import ValidSplit
+        return ValidSplit(0.2, stratified=False)
 
     @pytest.fixture(params=net_fixture_params)
     def net_1d(self, request, net_cls_1d, train_split):
         if request.param['classification']:
             from skorch import NeuralNetClassifier
             wrap_cls = NeuralNetClassifier
         else:
@@ -460,14 +386,87 @@
     def test_fit_predict_proba(self, net, data):
         X, y = data
         net.fit(X, y)
         y_proba = net.predict_proba(X)
         assert np.allclose(y_proba.sum(1), 1)
 
 
+class TestNetWithTokenizers:
+    """Huggingface tokenizers should work without special adjustments"""
+    @pytest.fixture(scope='session')
+    def tokenizer(self):
+        transformers = pytest.importorskip('transformers')
+        tokenizer = transformers.AutoTokenizer.from_pretrained('bert-base-uncased')
+        return tokenizer
+
+    @pytest.fixture(scope='session')
+    def data(self, tokenizer):
+        """A simple dataset that the model should be able to learn (or overfit)
+        on
+
+        """
+        X = [paragraph for paragraph in unittest.__doc__.split('\n') if paragraph]
+        Xt = tokenizer(
+            X,
+            max_length=12,
+            padding='max_length',
+            truncation=True,
+            return_token_type_ids=False,
+            return_tensors='pt',
+        )
+        y = np.array(['test' in x.lower() for x in X], dtype=np.int64)
+        return Xt, y
+
+    @pytest.fixture(scope='session')
+    def module_cls(self, tokenizer):
+        """Return a simple module using embedding + linear + softmax instead of
+        a full-fledged BERT module.
+
+        """
+        class MyModule(nn.Module):
+            def __init__(self):
+                super().__init__()
+                self.emb = nn.Embedding(tokenizer.vocab_size, 6)
+                self.dense = nn.Linear(6, 2)
+                self.sm = nn.Softmax(dim=-1)
+
+            # pylint: disable=arguments-differ
+            def forward(self, input_ids, attention_mask):
+                assert input_ids.shape == attention_mask.shape
+                X = self.emb(input_ids).mean(1)
+                return self.sm(self.dense(X))
+
+        return MyModule
+
+    @pytest.fixture(scope='session')
+    def net_cls(self):
+        from skorch import NeuralNetClassifier
+        return NeuralNetClassifier
+
+    @pytest.fixture(scope='module')
+    def net(self, net_cls, module_cls):
+        return net_cls(
+            module_cls,
+            optimizer=torch.optim.Adam,
+            max_epochs=5,
+            batch_size=8,
+            lr=0.1,
+        )
+
+    def test_fit_predict_proba(self, net, data):
+        X, y = data
+        net.fit(X, y)
+        y_proba = net.predict_proba(X)
+        assert np.allclose(y_proba.sum(1), 1)
+
+        train_losses = net.history[:, 'train_loss']
+        # make sure the network trained successfully with an arbitrary wide margin
+        assert train_losses[0] > 5 * train_losses[-1]
+
+
 class TestDataset:
     """Note: we don't need to test multi_indexing here, since that is
     already covered.
 
     """
     @pytest.fixture
     def dataset_cls(self):
@@ -592,15 +591,15 @@
         assert mock.call_count == 2  # once for train, once for valid
         assert mock.call_args_list[0][0][1] == data_split[0]
         assert mock.call_args_list[0][1]['training'] is True
         assert mock.call_args_list[1][0][1] == data_split[1]
         assert mock.call_args_list[1][1]['training'] is False
 
 
-class TestCVSplit:
+class TestValidSplit:
     num_samples = 100
 
     @staticmethod
     def assert_datasets_equal(ds0, ds1):
         """Generic function to test equality of dataset values."""
         assert len(ds0) == len(ds1)
         # pylint: disable=consider-using-enumerate
@@ -625,310 +624,297 @@
     def data(self, dataset_cls):
         X = np.random.random((self.num_samples, 10))
         assert self.num_samples % 4 == 0
         y = np.repeat([0, 1, 2, 3], self.num_samples // 4)
         return dataset_cls(X, y)
 
     @pytest.fixture
-    def cv_split_cls(self):
-        from skorch.dataset import CVSplit
-        return CVSplit
-
-    def test_reproducible(self, cv_split_cls, data):
-        dataset_train0, dataset_valid0 = cv_split_cls(5)(data)
-        dataset_train1, dataset_valid1 = cv_split_cls(5)(data)
+    def valid_split_cls(self):
+        from skorch.dataset import ValidSplit
+        return ValidSplit
+
+    def test_reproducible(self, valid_split_cls, data):
+        dataset_train0, dataset_valid0 = valid_split_cls(5)(data)
+        dataset_train1, dataset_valid1 = valid_split_cls(5)(data)
         self.assert_datasets_equal(dataset_train0, dataset_train1)
         self.assert_datasets_equal(dataset_valid0, dataset_valid1)
 
     @pytest.mark.parametrize('cv', [2, 4, 5, 10])
-    def test_different_kfolds(self, cv_split_cls, cv, data):
+    def test_different_kfolds(self, valid_split_cls, cv, data):
         if self.num_samples % cv != 0:
             raise ValueError("Num samples not divisible by {}".format(cv))
 
-        dataset_train, dataset_valid = cv_split_cls(cv)(data)
+        dataset_train, dataset_valid = valid_split_cls(cv)(data)
         assert len(dataset_train) + len(dataset_valid) == self.num_samples
         assert len(dataset_valid) == self.num_samples // cv
 
     @pytest.mark.parametrize('cv', [5, 0.2])
-    def test_stratified(self, cv_split_cls, data, cv):
+    def test_stratified(self, valid_split_cls, data, cv):
         num_expected = self.num_samples // 4
         y = np.hstack([np.repeat([0, 0, 0], num_expected),
                        np.repeat([1], num_expected)])
         data.y = y
 
-        dataset_train, dataset_valid = cv_split_cls(
+        dataset_train, dataset_valid = valid_split_cls(
             cv, stratified=True)(data, y)
         y_train = data_from_dataset(dataset_train)[1]
         y_valid = data_from_dataset(dataset_valid)[1]
 
         assert y_train.sum() == 0.8 * num_expected
         assert y_valid.sum() == 0.2 * num_expected
 
     @pytest.mark.parametrize('cv', [0.1, 0.2, 0.5, 0.75])
-    def test_different_fractions(self, cv_split_cls, cv, data):
+    def test_different_fractions(self, valid_split_cls, cv, data):
         if not (self.num_samples * cv).is_integer() != 0:
             raise ValueError("Num samples cannot be evenly distributed for "
                              "fraction {}".format(cv))
 
-        dataset_train, dataset_valid = cv_split_cls(cv)(data)
+        dataset_train, dataset_valid = valid_split_cls(cv)(data)
         assert len(dataset_train) + len(dataset_valid) == self.num_samples
         assert len(dataset_valid) == self.num_samples * cv
 
     @pytest.mark.parametrize('cv', [0.1, 0.2, 0.5, 0.75])
-    def test_fraction_no_y(self, cv_split_cls, data, cv):
+    def test_fraction_no_y(self, valid_split_cls, data, cv):
         if not (self.num_samples * cv).is_integer() != 0:
             raise ValueError("Num samples cannot be evenly distributed for "
                              "fraction {}".format(cv))
 
         m = int(cv * self.num_samples)
         n = int((1 - cv) * self.num_samples)
-        dataset_train, dataset_valid = cv_split_cls(
+        dataset_train, dataset_valid = valid_split_cls(
             cv, stratified=False)(data, None)
         assert len(dataset_valid) == m
         assert len(dataset_train) == n
 
-    def test_fraction_no_classifier(self, cv_split_cls, data):
+    def test_fraction_no_classifier(self, valid_split_cls, data):
         y = np.random.random(self.num_samples)
         data.y = y
 
         cv = 0.2
         m = int(cv * self.num_samples)
         n = int((1 - cv) * self.num_samples)
-        dataset_train, dataset_valid = cv_split_cls(
+        dataset_train, dataset_valid = valid_split_cls(
             cv, stratified=False)(data, y)
 
         assert len(dataset_valid) == m
         assert len(dataset_train) == n
 
     @pytest.mark.parametrize('cv', [0, -0.001, -0.2, -3])
-    def test_bad_values_raise(self, cv_split_cls, cv):
+    def test_bad_values_raise(self, valid_split_cls, cv):
         with pytest.raises(ValueError) as exc:
-            cv_split_cls(cv)
+            valid_split_cls(cv)
 
         expected = ("Numbers less than 0 are not allowed for cv "
-                    "but CVSplit got {}".format(cv))
+                    "but ValidSplit got {}".format(cv))
         assert exc.value.args[0] == expected
 
     @pytest.mark.parametrize('cv', [5, 0.2])
-    def test_not_stratified(self, cv_split_cls, data, cv):
+    def test_not_stratified(self, valid_split_cls, data, cv):
         num_expected = self.num_samples // 4
         y = np.hstack([np.repeat([0, 0, 0], num_expected),
                        np.repeat([1], num_expected)])
         data.y = y
 
-        dataset_train, dataset_valid = cv_split_cls(
+        dataset_train, dataset_valid = valid_split_cls(
             cv, stratified=False)(data, y)
         y_train = data_from_dataset(dataset_train)[1]
         y_valid = data_from_dataset(dataset_valid)[1]
 
         # when not stratified, we cannot know the distribution of targets
         assert y_train.sum() + y_valid.sum() == num_expected
 
-    def test_predefined_split(self, cv_split_cls, data):
+    def test_predefined_split(self, valid_split_cls, data):
         from sklearn.model_selection import PredefinedSplit
         indices = (data.y > 0).astype(int)
         split = PredefinedSplit(indices)
 
-        dataset_train, dataset_valid = cv_split_cls(split)(data)
+        dataset_train, dataset_valid = valid_split_cls(split)(data)
         y_train = data_from_dataset(dataset_train)[1]
         y_valid = data_from_dataset(dataset_valid)[1]
 
         assert (y_train > 0).all()
         assert (y_valid == 0).all()
 
-    def test_with_y_none(self, cv_split_cls, data):
+    def test_with_y_none(self, valid_split_cls, data):
         data.y = None
         m = self.num_samples // 5
         n = self.num_samples - m
-        dataset_train, dataset_valid = cv_split_cls(5)(data)
+        dataset_train, dataset_valid = valid_split_cls(5)(data)
 
         assert len(dataset_train) == n
         assert len(dataset_valid) == m
 
         y_train = data_from_dataset(dataset_train)[1]
         y_valid = data_from_dataset(dataset_valid)[1]
 
         assert y_train is None
         assert y_valid is None
 
-    def test_with_torch_tensors(self, cv_split_cls, data):
+    def test_with_torch_tensors(self, valid_split_cls, data):
         data.X = to_tensor(data.X, device='cpu')
         data.y = to_tensor(data.y, device='cpu')
         m = self.num_samples // 5
         n = self.num_samples - m
-        dataset_train, dataset_valid = cv_split_cls(5)(data)
+        dataset_train, dataset_valid = valid_split_cls(5)(data)
 
         assert len(dataset_valid) == m
         assert len(dataset_train) == n
 
-    def test_with_torch_tensors_and_stratified(self, cv_split_cls, data):
+    def test_with_torch_tensors_and_stratified(self, valid_split_cls, data):
         num_expected = self.num_samples // 4
         data.X = to_tensor(data.X, device='cpu')
         y = np.hstack([np.repeat([0, 0, 0], num_expected),
                        np.repeat([1], num_expected)])
         data.y = to_tensor(y, device='cpu')
 
-        dataset_train, dataset_valid = cv_split_cls(5, stratified=True)(data, y)
+        dataset_train, dataset_valid = valid_split_cls(5, stratified=True)(data, y)
         y_train = data_from_dataset(dataset_train)[1]
         y_valid = data_from_dataset(dataset_valid)[1]
 
         assert y_train.sum() == 0.8 * num_expected
         assert y_valid.sum() == 0.2 * num_expected
 
-    def test_with_list_of_arrays(self, cv_split_cls, data):
+    def test_with_list_of_arrays(self, valid_split_cls, data):
         data.X = [data.X, data.X]
         m = self.num_samples // 5
         n = self.num_samples - m
 
-        dataset_train, dataset_valid = cv_split_cls(5)(data)
+        dataset_train, dataset_valid = valid_split_cls(5)(data)
         X_train, y_train = data_from_dataset(dataset_train)
         X_valid, y_valid = data_from_dataset(dataset_valid)
 
         assert len(X_train[0]) == len(X_train[1]) == len(y_train) == n
         assert len(X_valid[0]) == len(X_valid[1]) == len(y_valid) == m
 
-    def test_with_dict(self, cv_split_cls, data):
+    def test_with_dict(self, valid_split_cls, data):
         data.X = {'1': data.X, '2': data.X}
-        dataset_train, dataset_valid = cv_split_cls(5)(data)
+        dataset_train, dataset_valid = valid_split_cls(5)(data)
 
         m = self.num_samples // 5
         n = self.num_samples - m
 
         X_train, y_train = data_from_dataset(dataset_train)
         X_valid, y_valid = data_from_dataset(dataset_valid)
 
         assert len(X_train['1']) == len(X_train['2']) == len(y_train) == n
         assert len(X_valid['1']) == len(X_valid['2']) == len(y_valid) == m
 
     @pytest.mark.skipif(not pandas_installed, reason='pandas is not installed')
-    def test_with_pandas(self, cv_split_cls, data):
+    def test_with_pandas(self, valid_split_cls, data):
         import pandas as pd
 
         data.X = pd.DataFrame(
             data.X,
             columns=[str(i) for i in range(data.X.shape[1])],
         )
-        dataset_train, dataset_valid = cv_split_cls(5)(data)
+        dataset_train, dataset_valid = valid_split_cls(5)(data)
 
         m = self.num_samples // 5
         X_train, y_train = data_from_dataset(dataset_train)
         X_valid, y_valid = data_from_dataset(dataset_valid)
 
         assert len(X_train) + len(X_valid) == self.num_samples
         assert len(y_train) + len(y_valid) == self.num_samples
         assert len(X_valid) == len(y_valid) == m
 
-    def test_y_str_val_stratified(self, cv_split_cls, data):
+    def test_y_str_val_stratified(self, valid_split_cls, data):
         y = np.array(['a', 'a', 'a', 'b'] * (self.num_samples // 4))
         if len(data.X) != len(y):
             raise ValueError
         data.y = y
 
-        dataset_train, dataset_valid = cv_split_cls(
+        dataset_train, dataset_valid = valid_split_cls(
             5, stratified=True)(data, y)
         y_train = data_from_dataset(dataset_train)[1]
         y_valid = data_from_dataset(dataset_valid)[1]
 
         assert np.isclose(np.mean(y_train == 'b'), 0.25)
         assert np.isclose(np.mean(y_valid == 'b'), 0.25)
 
-    def test_y_list_of_arr_does_not_raise(self, cv_split_cls, data):
+    def test_y_list_of_arr_does_not_raise(self, valid_split_cls, data):
         y = [np.zeros(self.num_samples), np.ones(self.num_samples)]
         data.y = y
-        cv_split_cls(5, stratified=False)(data)
+        valid_split_cls(5, stratified=False)(data)
 
-    def test_y_list_of_arr_stratified(self, cv_split_cls, data):
+    def test_y_list_of_arr_stratified(self, valid_split_cls, data):
         y = [np.zeros(self.num_samples), np.ones(self.num_samples)]
         data.y = y
         with pytest.raises(ValueError) as exc:
-            cv_split_cls(5, stratified=True)(data, y)
+            valid_split_cls(5, stratified=True)(data, y)
 
         expected = "Stratified CV requires explicitly passing a suitable y."
         assert exc.value.args[0] == expected
 
-    def test_y_dict_does_not_raise(self, cv_split_cls, data):
+    def test_y_dict_does_not_raise(self, valid_split_cls, data):
         y = {'a': np.zeros(self.num_samples), 'b': np.ones(self.num_samples)}
         data.y = y
 
-        cv_split_cls(5, stratified=False)(data)
+        valid_split_cls(5, stratified=False)(data)
 
-    def test_y_dict_stratified_raises(self, cv_split_cls, data):
+    def test_y_dict_stratified_raises(self, valid_split_cls, data):
         X = data[0]
         y = {'a': np.zeros(len(X)), 'b': np.ones(len(X))}
 
         with pytest.raises(ValueError):
             # an sklearn error is raised
-            cv_split_cls(5, stratified=True)(X, y)
+            valid_split_cls(5, stratified=True)(X, y)
 
     @pytest.mark.parametrize('cv', [5, 0.2])
     @pytest.mark.parametrize('X', [np.zeros((100, 10)), torch.zeros((100, 10))])
-    def test_y_none_stratified(self, cv_split_cls, data, cv, X):
+    def test_y_none_stratified(self, valid_split_cls, data, cv, X):
         data.X = X
         with pytest.raises(ValueError) as exc:
-            cv_split_cls(cv, stratified=True)(data, None)
+            valid_split_cls(cv, stratified=True)(data, None)
 
         expected = "Stratified CV requires explicitly passing a suitable y."
         assert exc.value.args[0] == expected
 
     def test_shuffle_split_reproducible_with_random_state(
-            self, cv_split_cls, dataset_cls):
+            self, valid_split_cls, dataset_cls):
         n = self.num_samples
         X, y = np.random.random((n, 10)), np.random.randint(0, 10, size=n)
-        cv = cv_split_cls(0.2, stratified=False)
+        cv = valid_split_cls(0.2, stratified=False)
 
         dst0, dsv0 = cv(dataset_cls(X, y))
         dst1, dsv1 = cv(dataset_cls(X, y))
 
         Xt0, yt0 = data_from_dataset(dst0)
         Xv0, yv0 = data_from_dataset(dsv0)
         Xt1, yt1 = data_from_dataset(dst1)
         Xv1, yv1 = data_from_dataset(dsv1)
 
         assert not np.allclose(Xt0, Xt1)
         assert not np.allclose(Xv0, Xv1)
         assert not np.allclose(yt0, yt1)
         assert not np.allclose(yv0, yv1)
 
-    def test_group_kfold(self, cv_split_cls, data):
+    def test_group_kfold(self, valid_split_cls, data):
         from sklearn.model_selection import GroupKFold
 
         X, y = data.X, data.y
         n = self.num_samples // 2
         groups = np.asarray(
             [0 for _ in range(n)] + [1 for _ in range(self.num_samples - n)])
 
-        dataset_train, dataset_valid = cv_split_cls(
+        dataset_train, dataset_valid = valid_split_cls(
             GroupKFold(n_splits=2))(data, groups=groups)
         X_train, y_train = data_from_dataset(dataset_train)
         X_valid, y_valid = data_from_dataset(dataset_valid)
 
         assert np.allclose(X[:n], X_train)
         assert np.allclose(y[:n], y_train)
         assert np.allclose(X[n:], X_valid)
         assert np.allclose(y[n:], y_valid)
 
-    @pytest.mark.parametrize(
-        'args, kwargs, expect_warning',
-        [
-            ([], {}, False),
-            ([], {"random_state": 0}, True),
-            ([10], {"random_state": 0}, True),
-            ([0.7], {"random_state": 0}, False),
-            ([[]], {}, False),
-            ([[]], {"random_state": 0}, True),
-        ])
-    def test_random_state_not_used_warning(
-            self, cv_split_cls, args, kwargs, expect_warning):
-        with pytest.warns(None) as record:
-            cv_split_cls(*args, **kwargs)
-
-        if expect_warning:
-            assert len(record) == 1
-            warning = record[0].message
-            assert isinstance(warning, FutureWarning)
-            assert warning.args[0] == (
-                "Setting a random_state has no effect since cv is not a float. "
-                "This will raise an error in a future. You should leave "
-                "random_state to its default (None), or set cv to a float value."
-            )
-        else:
-            assert not record
+    def test_random_state_not_used_raises(self, valid_split_cls):
+        # Since there is no randomness involved, raise a ValueError when
+        # random_state is set, same as sklearn is now doing.
+        msg = (
+            r"Setting a random_state has no effect since cv is not a float. "
+            r"You should leave random_state to its default \(None\), or set cv "
+            r"to a float value."
+        )
+        with pytest.raises(ValueError, match=msg):
+            valid_split_cls(5, random_state=0)
+
+    def test_random_state_and_float_does_not_raise(self, valid_split_cls):
+        valid_split_cls(0.5, random_state=0)  # does not raise
```

### Comparing `skorch-0.9.0/skorch/tests/test_helper.py` & `skorch-1.0.0/skorch/tests/test_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -169,16 +169,15 @@
         net = NeuralNetClassifier(classifier_module)
         X, y = data
         X = sldict_cls(X=X)
         params = {
             'lr': [0.01, 0.02],
             'max_epochs': [10, 20],
         }
-        gs = GridSearchCV(net, params, refit=True, cv=3, scoring='accuracy',
-                          iid=True)
+        gs = GridSearchCV(net, params, refit=True, cv=3, scoring='accuracy')
         gs.fit(X, y)
         print(gs.best_score_, gs.best_params_)
 
     def test_copy(self, sldict, sldict_cls):
         copied = sldict.copy()
         assert copied.shape == sldict.shape
         assert isinstance(copied, sldict_cls)
@@ -261,20 +260,31 @@
         )
         sldict1 = sldict_cls(
             a=np.arange(3),
             b=np.arange(3, 6),
         )
         assert sldict0 != sldict1
 
+    def test_subclass_getitem_returns_instance_of_itself(self, sldict_cls):
+        class MySliceDict(sldict_cls):
+            pass
+
+        sldict = MySliceDict(a=np.zeros(3))
+        sliced = sldict[:2]
+        assert isinstance(sliced, MySliceDict)
+
 
 class TestSliceDataset:
-    @pytest.fixture(scope='class')
-    def data(self):
+    @pytest.fixture(scope='class', params=['numpy', 'torch'])
+    def data(self, request):
         X, y = make_classification(100, 20, n_informative=10, random_state=0)
-        return X.astype(np.float32), y
+        X = X.astype(np.float32)
+        if request.param == 'numpy':
+            return X, y
+        return torch.from_numpy(X), torch.from_numpy(y)
 
     @pytest.fixture
     def X(self, data):
         return data[0]
 
     @pytest.fixture
     def y(self, data):
@@ -320,19 +330,27 @@
         slice(0, None),
         slice(-1, None),
         slice(None, None, -1),
         [0],
         [55],
         [-3],
         [0, 10, 3, -8, 3],
-        np.ones(100, dtype=np.bool),
+        np.ones(100, dtype=bool),
         # boolean mask array of length 100
-        np.array([0, 0, 1, 0] * 25, dtype=np.bool),
+        np.array([0, 0, 1, 0] * 25, dtype=bool),
     ])
     def test_len_and_shape_sliced(self, slds, y, sl):
+        # torch tensors don't support negative steps, skip test
+        if (
+                isinstance(sl, slice)
+                and (sl == slice(None, None, -1))
+                and isinstance(y, torch.Tensor)
+        ):
+            return
+
         assert len(slds[sl]) == len(y[sl])
         assert slds[sl].shape == (len(y[sl]),)
 
     @pytest.mark.parametrize('n', [0, 1])
     def test_slice_non_int_is_slicedataset(self, slds_cls, custom_ds, n):
         slds = slds_cls(custom_ds, idx=n)
         sl = np.arange(7, 55, 3)
@@ -352,45 +370,51 @@
     @pytest.mark.parametrize('n', [0, 1])
     @pytest.mark.parametrize('sl0, sl1', [
         ([55], 0),
         (slice(0, 1), 0),
         (slice(-1, None), 0),
         ([55], -1),
         ([0, 10, 3, -8, 3], 1),
-        (np.ones(100, dtype=np.bool), 5),
+        (np.ones(100, dtype=bool), 5),
         # boolean mask array of length 100
-        (np.array([0, 0, 1, 0] * 25, dtype=np.bool), 6),
+        (np.array([0, 0, 1, 0] * 25, dtype=bool), 6),
     ])
     def test_slice_twice(self, slds_cls, custom_ds, X, y, sl0, sl1, n):
         data = X if n == 0 else y
         slds = slds_cls(custom_ds, idx=n)
         sliced = slds[sl0][sl1]
         x = data[sl0][sl1]
         assert np.allclose(sliced, x)
 
     @pytest.mark.parametrize('n', [0, 1])
     @pytest.mark.parametrize('sl0, sl1, sl2', [
         (slice(0, 50), slice(10, 20), 5),
         ([0, 10, 3, -8, 3], [1, 2, 3], 2),
-        (np.ones(100, dtype=np.bool), np.arange(10, 40), 29),
+        (np.ones(100, dtype=bool), np.arange(10, 40), 29),
     ])
     def test_slice_three_times(self, slds_cls, custom_ds, X, y, sl0, sl1, sl2, n):
         data = y if n else X
         slds = slds_cls(custom_ds, idx=n)
         sliced = slds[sl0][sl1][sl2]
         x = data[sl0][sl1][sl2]
         assert np.allclose(sliced, x)
 
     def test_explicitly_pass_indices_at_init(self, slds_cls, custom_ds, X):
+        from skorch.utils import to_numpy
         # test passing indices directy to __init__
         slds = slds_cls(custom_ds, indices=np.arange(10))
         sliced0 = slds[5:]
-        assert np.allclose(sliced0, X[5:10])
-
         sliced1 = sliced0[2]
+
+        # comparison method depends on array type
+        if isinstance(sliced1, torch.Tensor):
+            sliced0 = to_numpy(sliced0)
+            sliced1 = to_numpy(sliced1)
+
+        assert np.allclose(sliced0, X[5:10])
         assert np.allclose(sliced1, X[7])
 
     def test_access_element_out_of_bounds(self, slds_cls, custom_ds):
         slds = slds_cls(custom_ds, idx=2)
         with pytest.raises(IndexError) as exc:
             # pylint: disable=pointless-statement
             slds[0]
@@ -419,28 +443,32 @@
             train_split=False,
             verbose=0,
         )
         params = {
             'lr': [0.01, 0.02],
             'max_epochs': [10, 20],
         }
-        gs = GridSearchCV(net, params, refit=False, cv=3, scoring='accuracy', iid=True)
+        gs = GridSearchCV(
+            net, params, refit=False, cv=3, scoring='accuracy', error_score='raise'
+        )
         gs.fit(slds, y)  # does not raise
 
     def test_grid_search_with_slds_and_internal_split_works(
             self, slds, y, classifier_module):
         from sklearn.model_selection import GridSearchCV
         from skorch import NeuralNetClassifier
 
         net = NeuralNetClassifier(classifier_module)
         params = {
             'lr': [0.01, 0.02],
             'max_epochs': [10, 20],
         }
-        gs = GridSearchCV(net, params, refit=True, cv=3, scoring='accuracy', iid=True)
+        gs = GridSearchCV(
+            net, params, refit=True, cv=3, scoring='accuracy', error_score='raise'
+        )
         gs.fit(slds, y)  # does not raise
 
     def test_grid_search_with_slds_X_and_slds_y(
             self, slds, slds_y, classifier_module):
         from sklearn.model_selection import GridSearchCV
         from skorch import NeuralNetClassifier
 
@@ -449,27 +477,69 @@
             train_split=False,
             verbose=0,
         )
         params = {
             'lr': [0.01, 0.02],
             'max_epochs': [10, 20],
         }
-        gs = GridSearchCV(net, params, refit=False, cv=3, scoring='accuracy', iid=True)
+        gs = GridSearchCV(
+            net, params, refit=False, cv=3, scoring='accuracy', error_score='raise'
+        )
         gs.fit(slds, slds_y)  # does not raise
 
     def test_index_with_2d_array_raises(self, slds):
         i = np.arange(4).reshape(2, 2)
         with pytest.raises(IndexError) as exc:
             # pylint: disable=pointless-statement
             slds[i]
 
         msg = ("SliceDataset only supports slicing with 1 "
                "dimensional arrays, got 2 dimensions instead.")
         assert exc.value.args[0] == msg
 
+    @pytest.mark.parametrize('n', [0, 1])
+    def test_slicedataset_to_numpy(self, slds_cls, custom_ds, n):
+        from skorch.utils import to_numpy
+
+        slds = slds_cls(custom_ds, idx=n)
+        expected = custom_ds.X if n == 0 else custom_ds.y
+        result = to_numpy(slds)
+        np.testing.assert_array_equal(result, expected)
+
+    @pytest.mark.parametrize('n', [0, 1])
+    @pytest.mark.parametrize('dtype', [None, np.float16, np.int32, np.complex64])
+    def test_slicedataset_asarray(self, slds_cls, custom_ds, n, dtype):
+        torch_to_numpy_dtype_dict = {
+            torch.int64: np.int64,
+            torch.float32: np.float32,
+        }
+
+        slds = slds_cls(custom_ds, idx=n)
+        array = np.asarray(slds, dtype=dtype)
+        expected = custom_ds.X if n == 0 else custom_ds.y
+        assert array.shape == expected.shape
+
+        if dtype is not None:
+            assert array.dtype == dtype
+        else:
+            # if no dtype indicated, use original dtype of the data, or the
+            # numpy equivalent if a torch dtype
+            expected_dtype = torch_to_numpy_dtype_dict.get(expected.dtype, expected.dtype)
+            assert array.dtype == expected_dtype
+
+    @pytest.mark.parametrize('sl', [slice(0, 2), np.arange(3)])
+    def test_subclass_getitem_returns_instance_of_itself(self, slds_cls, custom_ds, sl):
+        class MySliceDataset(slds_cls):
+            pass
+
+        slds = MySliceDataset(custom_ds, idx=0)
+        sliced = slds[sl]
+
+        assert isinstance(sliced, MySliceDataset)
+
 
 class TestPredefinedSplit():
 
     @pytest.fixture
     def predefined_split(self):
         from skorch.helper import predefined_split
         return predefined_split
```

### Comparing `skorch-0.9.0/skorch/tests/test_scoring.py` & `skorch-1.0.0/skorch/tests/test_scoring.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Tests for scoring.py"""
+
 import pytest
 import numpy as np
 import torch
 
 
 class TestLossScoring:
     @pytest.fixture(scope="module")
@@ -91,27 +93,27 @@
         X, y = data
         y_val_proba = torch.as_tensor(scored_net_fit.predict_proba(X))
         loss_value = scored_net_fit.get_loss(y_val_proba, y)
         score_value = scored_net_fit.score(X, y)
         assert np.allclose(score_value, loss_value.item())
 
     def test_scored_net_with_reduction_none(
-        self, scored_net_cls, module_cls, reduction, data
+            self, scored_net_cls, module_cls, reduction, data
     ):
         X, y = data
         net = scored_net_cls(
             module_cls, lr=0.01, criterion__reduction=reduction
         ).fit(X, y)
         net.set_params(criterion__reduction="sum")
         loss_value = net.score(X, y)
         net.set_params(criterion__reduction="none")
         output = net.score(X, y)
         assert output.shape[0] == X.shape[0]
         assert np.allclose(output.sum(), loss_value)
 
     def test_score_unknown_reduction_raises(
-        self, loss_scoring_fn, net_fit, data
+            self, loss_scoring_fn, net_fit, data
     ):
         X, y = data
         net_fit.set_params(criterion__reduction="unk")
         with pytest.raises(ValueError, match="for reduction but got"):
             loss_scoring_fn(net_fit, X, y)
```

### Comparing `skorch-0.9.0/skorch/tests/test_setter.py` & `skorch-1.0.0/skorch/tests/test_setter.py`

 * *Files identical despite different names*

### Comparing `skorch-0.9.0/skorch/tests/test_toy.py` & `skorch-1.0.0/skorch/tests/test_toy.py`

 * *Files identical despite different names*

### Comparing `skorch-0.9.0/skorch/tests/test_utils.py` & `skorch-1.0.0/skorch/tests/flycheck_test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Test for utils.py"""
 
+from copy import deepcopy
+
 import numpy as np
 import pytest
 from scipy import sparse
 import torch
 from torch.nn.utils.rnn import PackedSequence
 from torch.nn.utils.rnn import pack_padded_sequence
 
 from skorch.tests.conftest import pandas_installed
-from copy import deepcopy
+
 
 class TestToTensor:
     @pytest.fixture
     def to_tensor(self):
         from skorch.utils import to_tensor
         return to_tensor
 
@@ -94,16 +96,16 @@
                 (z, torch.as_tensor(z).to('cuda')),
                 (
                     {'a': x, 'b': y, 'c': z},
                     {'a': x, 'b': y, 'c': torch.as_tensor(z).to('cuda')}
                 ),
                 (torch.as_tensor(55), torch.as_tensor(55).to('cuda')),
                 (
-                    pack_padded_sequence(x, y),
-                    pack_padded_sequence(x, y).to('cuda')
+                    pack_padded_sequence(x, y.to('cpu')),
+                    pack_padded_sequence(x, y.to('cpu')).to('cuda')
                 ),
         ]:
             yield X, expected, device
 
     @pytest.mark.parametrize('X, expected, device', parameters())
     def test_tensor_conversion_cuda(self, to_tensor, X, expected, device):
         result = to_tensor(X, device)
@@ -182,25 +184,35 @@
         x_numpy = to_numpy(x_dict)
         self.compare_array_to_tensor(x_numpy['a'], x_dict['a'])
         self.compare_array_to_tensor(x_numpy['b'][0], x_dict['b'][0])
         self.compare_array_to_tensor(x_numpy['b'][1], x_dict['b'][1])
 
     @pytest.mark.parametrize('x_invalid', [
         1,
-        [1,2,3],
-        (1,2,3),
+        [1, 2, 3],
+        (1, 2, 3),
         {'a': 1},
     ])
     def test_invalid_inputs(self, to_numpy, x_invalid):
         # Inputs that are invalid for the scope of to_numpy.
         with pytest.raises(TypeError) as e:
             to_numpy(x_invalid)
         expected = "Cannot convert this data type to a numpy array."
         assert e.value.args[0] == expected
 
+    @pytest.mark.skipif(
+        not (hasattr(torch.backends, "mps") and torch.backends.mps.is_available()),
+        reason='Skipped because mps is not available as a torch backend'
+    )
+    def test_mps_support(self, to_numpy, x_tensor):
+        device = torch.device('mps')
+        x_tensor.to(device)
+        x_numpy = to_numpy(x_tensor)
+        self.compare_array_to_tensor(x_numpy, x_tensor)
+
 
 class TestToDevice:
     @pytest.fixture
     def to_device(self):
         from skorch.utils import to_device
         return to_device
 
@@ -226,15 +238,16 @@
         return pack_padded_sequence(value, length)
 
     @pytest.fixture
     def x_list(self):
         return [torch.zeros(3), torch.ones(2, 4)]
 
     def check_device_type(self, tensor, device_input, prev_device):
-        """assert expected device type conditioned on the input argument for `to_device`"""
+        """assert expected device type conditioned on the input argument for
+        `to_device`"""
         if None is device_input:
             assert tensor.device.type == prev_device
 
         else:
             assert tensor.device.type == device_input
 
     @pytest.mark.parametrize('device_from, device_to', [
@@ -292,15 +305,15 @@
     def test_check_device_dict_torch_tensor(
             self, to_device, x_dict, device_from, device_to):
         if 'cuda' in (device_from, device_to) and not torch.cuda.is_available():
             pytest.skip()
 
         original_x_dict = deepcopy(x_dict)
 
-        prev_devices=[None for _ in range(len(list(x_dict.keys())))]
+        prev_devices = [None for _ in range(len(list(x_dict.keys())))]
         if None in (device_from, device_to):
             prev_devices = [x.device.type for x in x_dict.values()]
 
         new_x_dict = to_device(x_dict, device=device_from)
         for xi, prev_d in zip(new_x_dict.values(), prev_devices):
             self.check_device_type(xi, device_from, prev_d)
 
@@ -484,14 +497,32 @@
 
     def test_subset_with_y_none(self, data_from_dataset, data, subset):
         subset.dataset.y = None
         X, y = data_from_dataset(subset)
         assert (X == data[0][[1, 3]]).all()
         assert y is None
 
+    def test_with_tensordataset_2_vals(self, data_from_dataset, tensors):
+        dataset = torch.utils.data.dataset.TensorDataset(*data)
+        X, y = data_from_dataset(dataset)
+        assert (X == data[0]).all()
+        assert (y == data[1]).all()
+
+    def test_with_tensordataset_1_val_raises(self, data_from_dataset, data):
+        dataset = torch.utils.data.dataset.TensorDataset(data[0])
+        msg = "Could not access X and y from dataset."
+        with pytest.raises(AttributeError, match=msg):
+            data_from_dataset(dataset)
+
+    def test_with_tensordataset_3_vals_raises(self, data_from_dataset, data):
+        dataset = torch.utils.data.dataset.TensorDataset(*data, data[0])
+        msg = "Could not access X and y from dataset."
+        with pytest.raises(AttributeError, match=msg):
+            data_from_dataset(dataset)
+
 
 class TestMultiIndexing:
     @pytest.fixture
     def multi_indexing(self):
         from skorch.dataset import multi_indexing
         return multi_indexing
 
@@ -804,16 +835,16 @@
         assert first_return == expected_list
         assert second_return == expected_list
 
 
 class TestInferPredictNonlinearity:
     @pytest.fixture
     def infer_predict_nonlinearity(self):
-        from skorch.utils import _infer_predict_nonlinearty
-        return _infer_predict_nonlinearty
+        from skorch.utils import _infer_predict_nonlinearity
+        return _infer_predict_nonlinearity
 
     @pytest.fixture
     def net_clf_cls(self):
         from skorch import NeuralNetClassifier
         return NeuralNetClassifier
 
     @pytest.fixture
@@ -841,27 +872,29 @@
         # CrossEntropyLoss criteron: nonlinearity should return valid probabilities
         net = net_clf_cls(module_cls, criterion=torch.nn.CrossEntropyLoss).initialize()
         fn = infer_predict_nonlinearity(net)
 
         X = torch.rand((20, 5))
         out = fn(X).numpy()
         assert np.allclose(out.sum(axis=1), 1.0)
+        # pylint: disable=misplaced-comparison-constant
         assert ((0 <= out) & (out <= 1.0)).all()
 
     def test_infer_neural_binary_net_classifier_default(
             self, infer_predict_nonlinearity, net_bin_clf_cls, module_cls):
         # BCEWithLogitsLoss should return valid probabilities
         net = net_bin_clf_cls(module_cls).initialize()
         fn = infer_predict_nonlinearity(net)
 
         X = torch.rand(20)  # binary classifier returns 1-dim output
         X = 10 * X - 5.0  # random values from -5 to 5
         out = fn(X).numpy()
         assert out.shape == (20, 2)  # output should be 2-dim
         assert np.allclose(out.sum(axis=1), 1.0)
+        # pylint: disable=misplaced-comparison-constant
         assert ((0 <= out) & (out <= 1.0)).all()
 
     def test_infer_neural_net_regressor_default(
             self, infer_predict_nonlinearity, net_regr_cls, module_cls):
         # default NeuralNetRegressor: no output nonlinearity
         net = net_regr_cls(module_cls).initialize()
         fn = infer_predict_nonlinearity(net)
```

### Comparing `skorch-0.9.0/skorch/toy.py` & `skorch-1.0.0/skorch/toy.py`

 * *Files identical despite different names*

### Comparing `skorch-0.9.0/skorch/utils.py` & `skorch-1.0.0/skorch/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 """skorch utilities.
 
 Should not have any dependency on other skorch packages.
 
 """
 
-from collections.abc import Sequence
+from collections.abc import Mapping, Sequence
 from contextlib import contextmanager
-from distutils.version import LooseVersion
 from enum import Enum
 from functools import partial
+import io
 from itertools import tee
 import pathlib
 import warnings
 
 import numpy as np
 from scipy import sparse
 import sklearn
+from sklearn.exceptions import NotFittedError
+from sklearn.utils import _safe_indexing as safe_indexing
+from sklearn.utils.validation import check_is_fitted as sk_check_is_fitted
 import torch
+from torch.nn import BCELoss
 from torch.nn import BCEWithLogitsLoss
 from torch.nn import CrossEntropyLoss
 from torch.nn.utils.rnn import PackedSequence
 from torch.utils.data.dataset import Subset
 
 from skorch.exceptions import DeviceWarning
 from skorch.exceptions import NotInitializedError
 
-if LooseVersion(sklearn.__version__) >= '0.22.0':
-    from sklearn.utils import _safe_indexing as safe_indexing
-else:
-    from sklearn.utils import safe_indexing
+try:
+    import torch_geometric
+    TORCH_GEOMETRIC_INSTALLED = True
+except ImportError:
+    TORCH_GEOMETRIC_INSTALLED = False
 
 
 class Ansi(Enum):
     BLUE = '\033[94m'
     CYAN = '\033[36m'
     GREEN = '\033[32m'
     MAGENTA = '\033[35m'
@@ -45,14 +50,19 @@
     return isinstance(x, (torch.Tensor, PackedSequence))
 
 
 def is_dataset(x):
     return isinstance(x, torch.utils.data.Dataset)
 
 
+def is_geometric_data_type(x):
+    from torch_geometric.data import Data
+    return isinstance(x, Data)
+
+
 # pylint: disable=not-callable
 def to_tensor(X, device, accept_sparse=False):
     """Turn input data to torch tensor.
 
     Parameters
     ----------
     X : input data
@@ -79,15 +89,20 @@
     output : torch Tensor
 
     """
     to_tensor_ = partial(to_tensor, device=device)
 
     if is_torch_data_type(X):
         return to_device(X, device)
-    if isinstance(X, dict):
+    if TORCH_GEOMETRIC_INSTALLED and is_geometric_data_type(X):
+        return to_device(X, device)
+    if hasattr(X, 'convert_to_tensors'):
+        # huggingface transformers BatchEncoding
+        return X.convert_to_tensors('pt')
+    if isinstance(X, Mapping):
         return {key: to_tensor_(val) for key, val in X.items()}
     if isinstance(X, (list, tuple)):
         return [to_tensor_(x) for x in X]
     if np.isscalar(X):
         return torch.as_tensor(X, device=device)
     if isinstance(X, Sequence):
         return torch.as_tensor(np.array(X), device=device)
@@ -99,51 +114,65 @@
                 X.nonzero(), X.data, size=X.shape).to(device)
         raise TypeError("Sparse matrices are not supported. Set "
                         "accept_sparse=True to allow sparse matrices.")
 
     raise TypeError("Cannot convert this data type to a torch tensor.")
 
 
+def _is_slicedataset(X):
+    # Cannot use isinstance because we don't want to depend on helper.py.
+    return hasattr(X, 'dataset') and hasattr(X, 'idx') and hasattr(X, 'indices')
+
+
 def to_numpy(X):
     """Generic function to convert a pytorch tensor to numpy.
 
     This function tries to unpack the tensor(s) from supported
     data structures (e.g., dicts, lists, etc.) but doesn't go
     beyond.
 
     Returns X when it already is a numpy array.
 
     """
     if isinstance(X, np.ndarray):
         return X
 
-    if isinstance(X, dict):
+    if isinstance(X, Mapping):
         return {key: to_numpy(val) for key, val in X.items()}
 
     if is_pandas_ndframe(X):
         return X.values
 
     if isinstance(X, (tuple, list)):
         return type(X)(to_numpy(x) for x in X)
 
+    if _is_slicedataset(X):
+        return np.asarray(X)
+
     if not is_torch_data_type(X):
         raise TypeError("Cannot convert this data type to a numpy array.")
 
     if X.is_cuda:
         X = X.cpu()
 
+    if hasattr(X, 'is_mps') and X.is_mps:
+        X = X.cpu()
+
     if X.requires_grad:
         X = X.detach()
 
     return X.numpy()
 
 
 def to_device(X, device):
     """Generic function to modify the device type of the tensor(s) or module.
 
+    PyTorch distribution objects are left untouched, since they don't support an
+    API to move between devices.
+
     Parameters
     ----------
     X : input data
         Deals with X being a:
 
          * torch tensor
          * tuple of torch tensors
@@ -155,20 +184,25 @@
         The compute device to be used. If device=None, return the input
         unmodified
 
     """
     if device is None:
         return X
 
-    if isinstance(X, dict):
-        return {key: to_device(val,device) for key, val in X.items()}
+    if isinstance(X, Mapping):
+        # dict-like but not a dict
+        return type(X)({key: to_device(val, device) for key, val in X.items()})
 
     # PackedSequence class inherits from a namedtuple
     if isinstance(X, (tuple, list)) and (type(X) != PackedSequence):
         return type(X)(to_device(x, device) for x in X)
+
+    if isinstance(X, torch.distributions.distribution.Distribution):
+        return X
+
     return X.to(device)
 
 
 def get_dim(y):
     """Return the number of dimensions of a torch tensor or numpy
     array-like object.
 
@@ -182,15 +216,15 @@
 def is_pandas_ndframe(x):
     # the sklearn way of determining this
     return hasattr(x, 'iloc')
 
 
 def flatten(arr):
     for item in arr:
-        if isinstance(item, (tuple, list, dict)):
+        if isinstance(item, (tuple, list, Mapping)):
             yield from flatten(item)
         else:
             yield item
 
 
 # pylint: disable=unused-argument
 def _indexing_none(data, i):
@@ -239,15 +273,15 @@
     instead of doing it repeatedly for each batch, thus saving some
     time.
 
     """
     if data is None:
         return _indexing_none
 
-    if isinstance(data, dict):
+    if isinstance(data, Mapping):
         # dictionary of containers
         return _indexing_dict
 
     if isinstance(data, (list, tuple)):
         try:
             # list or tuple of containers
             # TODO: Is there a better way than just to try to index? This
@@ -402,24 +436,32 @@
       If not None, use this function for indexing into the X data. If
       None, try to automatically determine how to index data.
 
     y_indexing : function/callable or None (default=None)
       If not None, use this function for indexing into the y data. If
       None, try to automatically determine how to index data.
 
+    Raises
+    ------
+    AttributeError
+      If X and y could not be accessed from the dataset.
+
     """
     X, y = _none, _none
 
     if isinstance(dataset, Subset):
         X, y = data_from_dataset(
             dataset.dataset, X_indexing=X_indexing, y_indexing=y_indexing)
         X = multi_indexing(X, dataset.indices, indexing=X_indexing)
         y = multi_indexing(y, dataset.indices, indexing=y_indexing)
     elif hasattr(dataset, 'X') and hasattr(dataset, 'y'):
         X, y = dataset.X, dataset.y
+    elif isinstance(dataset, torch.utils.data.dataset.TensorDataset):
+        if len(items := dataset.tensors) == 2:
+            X, y = items
 
     if (X is _none) or (y is _none):
         raise AttributeError("Could not access X and y from dataset.")
     return X, y
 
 
 def is_skorch_dataset(ds):
@@ -440,22 +482,23 @@
     target extractor.
     """
 
 
 @contextmanager
 def open_file_like(f, mode):
     """Wrapper for opening a file"""
-    new_fd = isinstance(f, (str, pathlib.Path))
-    if new_fd:
-        f = open(f, mode)
+    if isinstance(f, (str, pathlib.Path)):
+        file_like = open(f, mode)
+    else:
+        file_like = f
+
     try:
-        yield f
+        yield file_like
     finally:
-        if new_fd:
-            f.close()
+        file_like.close()
 
 
 # pylint: disable=unused-argument
 def train_loss_score(net, X=None, y=None):
     return net.history[-1, 'batches', -1, 'train_loss']
 
 
@@ -487,15 +530,15 @@
             self.step = step
 
     def get_step(self):
         """Return the stored step."""
         return self.step
 
 
-def _make_split(X, valid_ds, **kwargs):
+def _make_split(X, y=None, valid_ds=None, **kwargs):
     """Used by ``predefined_split`` to allow for pickling"""
     return X, valid_ds
 
 
 def freeze_parameter(param):
     """Convenience function to freeze a passed torch parameter.
     Used by ``skorch.callbacks.Freezer``
@@ -527,41 +570,52 @@
             'are available. Loading on device "{}" instead.'.format(
                 fallback_device,
             ), DeviceWarning)
         map_location = torch.device(fallback_device)
     return map_location
 
 
-def check_is_fitted(estimator, attributes, msg=None, all_or_any=all):
+def check_is_fitted(estimator, attributes=None, msg=None, all_or_any=all):
     """Checks whether the net is initialized.
 
     Note: This calls ``sklearn.utils.validation.check_is_fitted``
     under the hood, using exactly the same arguments and logic. The
     only difference is that this function has an adapted error message
     and raises a ``skorch.exception.NotInitializedError`` instead of
     an ``sklearn.exceptions.NotFittedError``.
 
     """
-    if msg is None:
-        msg = ("This %(name)s instance is not initialized yet. Call "
-               "'initialize' or 'fit' with appropriate arguments "
-               "before using this method.")
-
-    if not isinstance(attributes, (list, tuple)):
-        attributes = [attributes]
+    try:
+        sk_check_is_fitted(estimator, attributes, msg=msg, all_or_any=all_or_any)
+    except NotFittedError as exc:
+        if msg is None:
+            msg = ("This %(name)s instance is not initialized yet. Call "
+                   "'initialize' or 'fit' with appropriate arguments "
+                   "before using this method.")
 
-    if not all_or_any([hasattr(estimator, attr) for attr in attributes]):
-        raise NotInitializedError(msg % {'name': type(estimator).__name__})
+        raise NotInitializedError(msg % {'name': type(estimator).__name__}) from exc
 
 
 def _identity(x):
     """Return input as is, the identity operation"""
     return x
 
 
+def _make_2d_probs(prob):
+    """Create a 2d probability array from a 1d vector
+
+    This is needed because by convention, even for binary classification
+    problems, sklearn expects 2 probabilities to be returned per row, one for
+    class 0 and one for class 1.
+
+    """
+    y_proba = torch.stack((1 - prob, prob), 1)
+    return y_proba
+
+
 def _sigmoid_then_2d(x):
     """Transform 1-dim logits to valid y_proba
 
     Sigmoid is applied to x to transform it to probabilities. Then
     concatenate the probabilities with 1 - these probabilities to
     return a correctly formed ``y_proba``. This is required for
     sklearn, which expects probabilities to be 2d arrays whose sum
@@ -576,40 +630,77 @@
     -------
     y_proba : torch.tensor
       A 2 dimensional float tensor of probabilities that sum up to 1
       on axis 1.
 
     """
     prob = torch.sigmoid(x)
-    y_proba = torch.stack((1 - prob, prob), 1)
-    return y_proba
+    return _make_2d_probs(prob)
+
+
+# TODO only needed if multiclass GP classfication is added
+# def _transpose(x):
+    # return x.T
 
 
-def _infer_predict_nonlinearty(net):
+# pylint: disable=protected-access
+def _infer_predict_nonlinearity(net):
     """Infers the correct nonlinearity to apply for this net
 
     The nonlinearity is applied only when calling
     :func:`~skorch.classifier.NeuralNetClassifier.predict` or
     :func:`~skorch.classifier.NeuralNetClassifier.predict_proba`.
 
     """
     # Implementation: At the moment, this function "dispatches" only
     # based on the criterion, not the class of the net. We still pass
     # the whole net as input in case we want to modify this at a
     # future point in time.
-    criterion = net.criterion_
+    if len(net._criteria) != 1:
+        # don't know which criterion to consider, don't try to guess
+        return _identity
+
+    criterion = getattr(net, net._criteria[0] + '_')
 
     if isinstance(criterion, CrossEntropyLoss):
         return partial(torch.softmax, dim=-1)
 
     if isinstance(criterion, BCEWithLogitsLoss):
         return _sigmoid_then_2d
 
+    if isinstance(criterion, BCELoss):
+        return _make_2d_probs
+
     return _identity
 
+    # TODO: Add the code below to _infer_predict_nonlinearity if multiclass GP
+    # classfication is added.
+    # likelihood = getattr(net, 'likelihood_', None)
+    # if likelihood is None:
+    #     return _identity
+    # nonlin = _identity
+    # try:
+    #     import gpytorch
+    #     if isinstance(likelihood, gpytorch.likelihoods.SoftmaxLikelihood):
+    #         # SoftmaxLikelihood returns batch second order
+    #         nonlin = _transpose
+    # except ImportError:
+    #     # there is no gpytorch install
+    #     pass
+    # except AttributeError:
+    #     # gpytorch and pytorch are incompatible
+    #     msg = (
+    #         "Importing gpytorch failed. This is probably because its version is "
+    #         "incompatible with the installed torch version. Please visit "
+    #         "https://github.com/cornellius-gp/gpytorch#installation to check "
+    #         "which versions are compatible"
+    #     )
+    #     warnings.warn(msg)
+    # return nonlin
+
 
 class TeeGenerator:
     """Stores a generator and calls ``tee`` on it to create new generators
     when ``TeeGenerator`` is iterated over to let you iterate over the given
     generator more than once.
 
     """
```

### Comparing `skorch-0.9.0/skorch.egg-info/SOURCES.txt` & `skorch-1.0.0/skorch.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,45 +3,58 @@
 README.rst
 VERSION
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 skorch/__init__.py
+skorch/_doctor.py
+skorch/_version.py
 skorch/classifier.py
 skorch/cli.py
 skorch/dataset.py
 skorch/exceptions.py
+skorch/flycheck_dataset.py
 skorch/helper.py
+skorch/hf.py
 skorch/history.py
 skorch/net.py
+skorch/probabilistic.py
 skorch/regressor.py
 skorch/scoring.py
 skorch/setter.py
 skorch/toy.py
 skorch/utils.py
 skorch.egg-info/PKG-INFO
 skorch.egg-info/SOURCES.txt
 skorch.egg-info/dependency_links.txt
 skorch.egg-info/not-zip-safe
 skorch.egg-info/requires.txt
 skorch.egg-info/top_level.txt
 skorch/callbacks/__init__.py
 skorch/callbacks/base.py
+skorch/callbacks/flycheck_lr_scheduler.py
 skorch/callbacks/logging.py
 skorch/callbacks/lr_scheduler.py
 skorch/callbacks/regularization.py
 skorch/callbacks/scoring.py
 skorch/callbacks/training.py
+skorch/llm/__init__.py
+skorch/llm/classifier.py
+skorch/llm/prompts.py
 skorch/tests/__init__.py
 skorch/tests/conftest.py
+skorch/tests/flycheck_test_utils.py
 skorch/tests/test_classifier.py
 skorch/tests/test_cli.py
 skorch/tests/test_dataset.py
+skorch/tests/test_doctor.py
 skorch/tests/test_helper.py
+skorch/tests/test_hf.py
 skorch/tests/test_history.py
 skorch/tests/test_net.py
+skorch/tests/test_probabilistic.py
 skorch/tests/test_regressor.py
 skorch/tests/test_scoring.py
 skorch/tests/test_setter.py
 skorch/tests/test_toy.py
 skorch/tests/test_utils.py
```

