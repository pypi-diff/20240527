# Comparing `tmp/lckytools-0.0.0b1.tar.gz` & `tmp/lckytools-0.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lckytools-0.0.0b1.tar", max compression
+gzip compressed data, was "lckytools-0.0.0b2.tar", max compression
```

## Comparing `lckytools-0.0.0b1.tar` & `lckytools-0.0.0b2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-26 12:41:59.726540 lckytools-0.0.0b1/LICENSE
--rw-r--r--   0        0        0     1172 2024-05-27 00:50:41.770484 lckytools-0.0.0b1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-26 12:41:53.421109 lckytools-0.0.0b1/README.md
--rw-r--r--   0        0        0        0 2024-05-27 00:52:12.425121 lckytools-0.0.0b1/src/lckytools/__init__.py
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 lckytools-0.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-27 01:00:50.888092 lckytools-0.0.0b2/LICENSE
+-rw-r--r--   0        0        0     1167 2024-05-27 01:18:41.478578 lckytools-0.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0b2/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 00:52:12.425121 lckytools-0.0.0b2/src/lckytools/__init__.py
+-rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 lckytools-0.0.0b2/PKG-INFO
```

### Comparing `lckytools-0.0.0b1/pyproject.toml` & `lckytools-0.0.0b2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lckytools"
-version = "0.0.0-beta-1"
+version = "0.0.0b2"
 description = "A collection of helpful utility functions and tools."
 authors = ["Your Name <your.email@example.com>"]
 license = "MIT"
 
 readme = "README.md"
 homepage = "https://github.com/yourusername/lckytools"
 repository = "https://github.com/yourusername/lckytools"
```

