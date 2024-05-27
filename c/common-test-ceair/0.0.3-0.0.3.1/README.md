# Comparing `tmp/common_test_ceair-0.0.3.tar.gz` & `tmp/common_test_ceair-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\JobFiles\NDC\all_project\common_test_one\dist\.tmp-j06_o5kc\common_test_ceair-0.0.3.tar", last modified: Mon May 27 06:32:27 2024, max compression
+gzip compressed data, was "D:\JobFiles\NDC\all_project\common_test_one\dist\.tmp-dvnprzut\common_test_ceair-0.0.3.1.tar", last modified: Mon May 27 06:41:48 2024, max compression
```

## Comparing `common_test_ceair-0.0.3.tar` & `common_test_ceair-0.0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 06:32:27.775775 common_test_ceair-0.0.3/
--rw-rw-rw-   0        0        0       89 2024-05-27 06:32:27.775775 common_test_ceair-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 06:32:27.775775 common_test_ceair-0.0.3/common_test_ceair/
--rw-rw-rw-   0        0        0       25 2024-05-27 02:56:11.000000 common_test_ceair-0.0.3/common_test_ceair/__init__.py
--rw-rw-rw-   0        0        0      272 2024-05-27 02:35:46.000000 common_test_ceair-0.0.3/common_test_ceair/study_1.py
-drwxrwxrwx   0        0        0        0 2024-05-27 06:32:27.775775 common_test_ceair-0.0.3/common_test_ceair.egg-info/
--rw-rw-rw-   0        0        0       89 2024-05-27 06:32:27.000000 common_test_ceair-0.0.3/common_test_ceair.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-27 06:32:27.000000 common_test_ceair-0.0.3/common_test_ceair.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 06:32:27.000000 common_test_ceair-0.0.3/common_test_ceair.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 06:32:27.000000 common_test_ceair-0.0.3/common_test_ceair.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-27 06:32:27.000000 common_test_ceair-0.0.3/common_test_ceair.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       87 2024-05-27 06:32:20.000000 common_test_ceair-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 06:32:27.775775 common_test_ceair-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 06:41:48.410856 common_test_ceair-0.0.3.1/
+-rw-rw-rw-   0        0        0       91 2024-05-27 06:41:48.410856 common_test_ceair-0.0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 06:41:48.404756 common_test_ceair-0.0.3.1/common_test_ceair/
+-rw-rw-rw-   0        0        0       25 2024-05-27 02:56:11.000000 common_test_ceair-0.0.3.1/common_test_ceair/__init__.py
+-rw-rw-rw-   0        0        0      130 2024-05-27 06:41:03.000000 common_test_ceair-0.0.3.1/common_test_ceair/study_1.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:41:48.410856 common_test_ceair-0.0.3.1/common_test_ceair.egg-info/
+-rw-rw-rw-   0        0        0       91 2024-05-27 06:41:48.000000 common_test_ceair-0.0.3.1/common_test_ceair.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-27 06:41:48.000000 common_test_ceair-0.0.3.1/common_test_ceair.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 06:41:48.000000 common_test_ceair-0.0.3.1/common_test_ceair.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 06:41:48.000000 common_test_ceair-0.0.3.1/common_test_ceair.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-27 06:41:48.000000 common_test_ceair-0.0.3.1/common_test_ceair.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       89 2024-05-27 06:41:44.000000 common_test_ceair-0.0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 06:41:48.410856 common_test_ceair-0.0.3.1/setup.cfg
```

