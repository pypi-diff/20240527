# Comparing `tmp/trackerstatus-0.1.5.tar.gz` & `tmp/trackerstatus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackerstatus-0.1.5.tar", max compression
+gzip compressed data, was "trackerstatus-0.2.0.tar", max compression
```

## Comparing `trackerstatus-0.1.5.tar` & `trackerstatus-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-10-04 14:19:57.000000 trackerstatus-0.1.5/LICENSE
--rw-r--r--   0        0        0     1014 2023-02-07 14:40:53.000000 trackerstatus-0.1.5/README.md
--rw-r--r--   0        0        0      425 2023-09-14 23:16:24.718343 trackerstatus-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      174 2023-09-14 23:21:13.362911 trackerstatus-0.1.5/trackerstatus/MAINTAINERS.md
--rw-r--r--   0        0        0        0 2022-10-03 03:40:05.000000 trackerstatus-0.1.5/trackerstatus/__init__.py
--rw-r--r--   0        0        0     3776 2023-04-03 15:30:18.083182 trackerstatus-0.1.5/trackerstatus/api.py
--rw-r--r--   0        0        0     1622 1970-01-01 00:00:00.000000 trackerstatus-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-27 01:54:50.901064 trackerstatus-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3667 2024-05-27 01:54:50.901064 trackerstatus-0.2.0/README.md
+-rw-r--r--   0        0        0      543 2024-05-27 01:54:50.901064 trackerstatus-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1901 2024-05-27 01:54:50.901064 trackerstatus-0.2.0/trackerstatus/MAINTAINERS.md
+-rw-r--r--   0        0        0      198 2024-05-27 01:54:50.901064 trackerstatus-0.2.0/trackerstatus/__init__.py
+-rw-r--r--   0        0        0     1161 2024-05-27 01:54:50.905064 trackerstatus-0.2.0/trackerstatus/core.py
+-rw-r--r--   0        0        0        0 2024-05-27 01:54:50.905064 trackerstatus-0.2.0/trackerstatus/endpoints/__init__.py
+-rw-r--r--   0        0        0     2143 2024-05-27 01:54:50.905064 trackerstatus-0.2.0/trackerstatus/endpoints/btn.py
+-rw-r--r--   0        0        0      596 2024-05-27 01:54:50.905064 trackerstatus-0.2.0/trackerstatus/endpoints/status.py
+-rw-r--r--   0        0        0     4206 1970-01-01 00:00:00.000000 trackerstatus-0.2.0/PKG-INFO
```

### Comparing `trackerstatus-0.1.5/LICENSE` & `trackerstatus-0.2.0/LICENSE`

 * *Files identical despite different names*

