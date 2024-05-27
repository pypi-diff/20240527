# Comparing `tmp/oakestra_utils-0.1.1.tar.gz` & `tmp/oakestra_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oakestra_utils-0.1.1.tar", max compression
+gzip compressed data, was "oakestra_utils-0.1.2.tar", max compression
```

## Comparing `oakestra_utils-0.1.1.tar` & `oakestra_utils-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        7 2024-05-26 16:17:24.143594 oakestra_utils-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-26 16:18:54.275596 oakestra_utils-0.1.1/oakestra_utils/__init__.py
--rw-r--r--   0        0        0      402 2024-05-26 16:47:58.939629 oakestra_utils-0.1.1/oakestra_utils/types.py
--rw-r--r--   0        0        0      360 2024-05-26 16:57:17.087640 oakestra_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 oakestra_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-05-26 16:17:24.143594 oakestra_utils-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-26 16:18:54.275596 oakestra_utils-0.1.2/oakestra_utils/__init__.py
+-rw-r--r--   0        0        0      430 2024-05-26 17:56:36.427665 oakestra_utils-0.1.2/oakestra_utils/types.py
+-rw-r--r--   0        0        0      360 2024-05-26 18:00:44.191662 oakestra_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 oakestra_utils-0.1.2/PKG-INFO
```

