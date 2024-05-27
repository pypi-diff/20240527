# Comparing `tmp/promptic-0.1.0.tar.gz` & `tmp/promptic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.1.0.tar` & `promptic-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.0/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.0/LICENSE
--rw-r--r--   0        0        0     2974 2024-05-27 07:03:11.566431 promptic-0.1.0/README.md
--rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.0/promptic.py
--rw-r--r--   0        0        0      506 2024-05-27 07:09:25.355651 promptic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      306 1970-01-01 00:00:00.000000 promptic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.1/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2974 2024-05-27 07:03:11.566431 promptic-0.1.1/README.md
+-rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.1/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 07:10:50.809224 promptic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3322 1970-01-01 00:00:00.000000 promptic-0.1.1/PKG-INFO
```

### Comparing `promptic-0.1.0/.gitignore` & `promptic-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.1.0/LICENSE` & `promptic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.1.0/README.md` & `promptic-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `promptic-0.1.0/promptic.py` & `promptic-0.1.1/promptic.py`

 * *Files identical despite different names*

