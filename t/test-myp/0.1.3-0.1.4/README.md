# Comparing `tmp/test_myp-0.1.3.tar.gz` & `tmp/test_myp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_myp-0.1.3.tar", max compression
+gzip compressed data, was "test_myp-0.1.4.tar", max compression
```

## Comparing `test_myp-0.1.3.tar` & `test_myp-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        2 2024-05-27 18:14:00.824358 test_myp-0.1.3/README.md
--rw-r--r--   0        0        0      288 2024-05-27 18:14:09.924450 test_myp-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       61 2024-05-27 18:14:00.824358 test_myp-0.1.3/test_myp/__init__.py
--rw-r--r--   0        0        0       85 2024-05-27 18:14:00.824358 test_myp-0.1.3/test_myp/version.py
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 test_myp-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-05-27 18:17:00.089859 test_myp-0.1.4/README.md
+-rw-r--r--   0        0        0      288 2024-05-27 18:17:08.633898 test_myp-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-05-27 18:17:00.089859 test_myp-0.1.4/test_myp/__init__.py
+-rw-r--r--   0        0        0       85 2024-05-27 18:17:00.089859 test_myp-0.1.4/test_myp/version.py
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 test_myp-0.1.4/PKG-INFO
```

