# Comparing `tmp/common_test_ceair-0.0.1.tar.gz` & `tmp/common_test_ceair-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\JobFiles\NDC\all_project\common_test_one\dist\.tmp-puwve109\common_test_ceair-0.0.1.tar", last modified: Mon May 27 03:00:50 2024, max compression
+gzip compressed data, was "D:\JobFiles\NDC\all_project\common_test_one\dist\.tmp-owupwyb5\common_test_ceair-0.0.2.tar", last modified: Mon May 27 05:56:19 2024, max compression
```

## Comparing `common_test_ceair-0.0.1.tar` & `common_test_ceair-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 03:00:50.756820 common_test_ceair-0.0.1/
--rw-rw-rw-   0        0        0       64 2024-05-27 03:00:50.756820 common_test_ceair-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 03:00:50.751813 common_test_ceair-0.0.1/common_test_ceair/
--rw-rw-rw-   0        0        0       25 2024-05-27 02:56:11.000000 common_test_ceair-0.0.1/common_test_ceair/__init__.py
--rw-rw-rw-   0        0        0      272 2024-05-27 02:35:46.000000 common_test_ceair-0.0.1/common_test_ceair/study_1.py
-drwxrwxrwx   0        0        0        0 2024-05-27 03:00:50.756820 common_test_ceair-0.0.1/common_test_ceair.egg-info/
--rw-rw-rw-   0        0        0       64 2024-05-27 03:00:50.000000 common_test_ceair-0.0.1/common_test_ceair.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-05-27 03:00:50.000000 common_test_ceair-0.0.1/common_test_ceair.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 03:00:50.000000 common_test_ceair-0.0.1/common_test_ceair.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-27 03:00:50.000000 common_test_ceair-0.0.1/common_test_ceair.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2024-05-27 02:56:11.000000 common_test_ceair-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       99 2024-05-27 03:00:50.756820 common_test_ceair-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      118 2024-05-27 02:57:27.000000 common_test_ceair-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 05:56:19.833153 common_test_ceair-0.0.2/
+-rw-rw-rw-   0        0        0       84 2024-05-27 05:56:19.833153 common_test_ceair-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 05:56:19.817530 common_test_ceair-0.0.2/common_test_ceair/
+-rw-rw-rw-   0        0        0       25 2024-05-27 02:56:11.000000 common_test_ceair-0.0.2/common_test_ceair/__init__.py
+-rw-rw-rw-   0        0        0      272 2024-05-27 02:35:46.000000 common_test_ceair-0.0.2/common_test_ceair/study_1.py
+drwxrwxrwx   0        0        0        0 2024-05-27 05:56:19.833153 common_test_ceair-0.0.2/common_test_ceair.egg-info/
+-rw-rw-rw-   0        0        0       84 2024-05-27 05:56:19.000000 common_test_ceair-0.0.2/common_test_ceair.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-05-27 05:56:19.000000 common_test_ceair-0.0.2/common_test_ceair.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 05:56:19.000000 common_test_ceair-0.0.2/common_test_ceair.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-27 05:56:19.000000 common_test_ceair-0.0.2/common_test_ceair.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2024-05-27 05:50:30.000000 common_test_ceair-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       99 2024-05-27 05:56:19.833153 common_test_ceair-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      197 2024-05-27 05:51:12.000000 common_test_ceair-0.0.2/setup.py
```

