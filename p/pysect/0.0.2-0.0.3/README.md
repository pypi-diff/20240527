# Comparing `tmp/pysect-0.0.2.tar.gz` & `tmp/pysect-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysect-0.0.2.tar", last modified: Tue May 21 02:05:14 2024, max compression
+gzip compressed data, was "pysect-0.0.3.tar", last modified: Mon May 27 05:52:31 2024, max compression
```

## Comparing `pysect-0.0.2.tar` & `pysect-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,43 @@
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 02:05:14.624680 pysect-0.0.2/
--rwxrwx---   0 anonoei    (501) staff       (20)     1051 2024-05-19 23:54:50.000000 pysect-0.0.2/LICENSE
--rw-r--r--   0 anonoei    (501) staff       (20)     1581 2024-05-21 02:05:14.624327 pysect-0.0.2/PKG-INFO
--rwxrwx---   0 anonoei    (501) staff       (20)      492 2024-05-21 02:03:35.000000 pysect-0.0.2/README.md
--rw-r--r--   0 anonoei    (501) staff       (20)     1395 2024-05-21 02:04:32.000000 pysect-0.0.2/pyproject.toml
--rw-r--r--   0 anonoei    (501) staff       (20)       38 2024-05-21 02:05:14.624743 pysect-0.0.2/setup.cfg
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 02:05:14.618037 pysect-0.0.2/src/
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 02:05:14.619836 pysect-0.0.2/src/pysect/
--rw-r--r--   0 anonoei    (501) staff       (20)      173 2024-05-21 02:04:32.000000 pysect-0.0.2/src/pysect/__init__.py
--rw-r--r--   0 anonoei    (501) staff       (20)      675 2024-05-21 01:51:45.000000 pysect-0.0.2/src/pysect/main.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 02:05:14.621290 pysect-0.0.2/src/pysect/primitives/
--rw-r--r--   0 anonoei    (501) staff       (20)      294 2024-05-21 01:52:08.000000 pysect-0.0.2/src/pysect/primitives/coord.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 02:05:14.622006 pysect-0.0.2/src/pysect/sect/
--rw-r--r--   0 anonoei    (501) staff       (20)        0 2024-05-20 09:39:52.000000 pysect-0.0.2/src/pysect/sect/__init__.py
--rw-r--r--   0 anonoei    (501) staff       (20)       60 2024-05-20 04:06:39.000000 pysect-0.0.2/src/pysect/sect/config.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 02:05:14.622664 pysect-0.0.2/src/pysect/sect/primitives/
--rw-r--r--   0 anonoei    (501) staff       (20)        0 2024-05-20 09:40:02.000000 pysect-0.0.2/src/pysect/sect/primitives/__init__.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1947 2024-05-20 10:16:57.000000 pysect-0.0.2/src/pysect/sect/primitives/mesh.py
--rw-r--r--   0 anonoei    (501) staff       (20)      738 2024-05-20 09:40:23.000000 pysect-0.0.2/src/pysect/sect/primitives/stl.py
--rw-r--r--   0 anonoei    (501) staff       (20)        0 2024-05-20 03:11:04.000000 pysect-0.0.2/src/pysect/sect/sect.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 02:05:14.623091 pysect-0.0.2/src/pysect/sect/serial/
--rw-r--r--   0 anonoei    (501) staff       (20)        0 2024-05-20 09:40:01.000000 pysect-0.0.2/src/pysect/sect/serial/__init__.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2255 2024-05-20 09:40:08.000000 pysect-0.0.2/src/pysect/sect/serial/stl.py
--rw-r--r--   0 anonoei    (501) staff       (20)      470 2024-05-20 09:34:37.000000 pysect-0.0.2/src/pysect/sect/slice.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 02:05:14.623466 pysect-0.0.2/src/pysect.egg-info/
--rw-r--r--   0 anonoei    (501) staff       (20)     1581 2024-05-21 02:05:14.000000 pysect-0.0.2/src/pysect.egg-info/PKG-INFO
--rw-r--r--   0 anonoei    (501) staff       (20)      550 2024-05-21 02:05:14.000000 pysect-0.0.2/src/pysect.egg-info/SOURCES.txt
--rw-r--r--   0 anonoei    (501) staff       (20)        1 2024-05-21 02:05:14.000000 pysect-0.0.2/src/pysect.egg-info/dependency_links.txt
--rw-r--r--   0 anonoei    (501) staff       (20)       80 2024-05-21 02:05:14.000000 pysect-0.0.2/src/pysect.egg-info/requires.txt
--rw-r--r--   0 anonoei    (501) staff       (20)        7 2024-05-21 02:05:14.000000 pysect-0.0.2/src/pysect.egg-info/top_level.txt
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-27 05:52:31.037063 pysect-0.0.3/
+-rwxrwx---   0 anonoei    (501) staff       (20)     1051 2024-05-19 23:54:50.000000 pysect-0.0.3/LICENSE
+-rw-r--r--   0 anonoei    (501) staff       (20)     1581 2024-05-27 05:52:31.036692 pysect-0.0.3/PKG-INFO
+-rwxrwx---   0 anonoei    (501) staff       (20)      492 2024-05-21 02:03:35.000000 pysect-0.0.3/README.md
+-rwxrwx---   0 anonoei    (501) staff       (20)     1395 2024-05-27 05:52:23.000000 pysect-0.0.3/pyproject.toml
+-rw-r--r--   0 anonoei    (501) staff       (20)       38 2024-05-27 05:52:31.037138 pysect-0.0.3/setup.cfg
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-27 05:52:31.027822 pysect-0.0.3/src/
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-27 05:52:31.029877 pysect-0.0.3/src/pysect/
+-rwxrwx---   0 anonoei    (501) staff       (20)      173 2024-05-27 05:52:23.000000 pysect-0.0.3/src/pysect/__init__.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-27 05:52:31.031795 pysect-0.0.3/src/pysect/config/
+-rwxrwx---   0 anonoei    (501) staff       (20)        0 2024-05-27 04:44:15.000000 pysect-0.0.3/src/pysect/config/__init__.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1177 2024-05-27 05:41:32.000000 pysect-0.0.3/src/pysect/config/config.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-27 05:52:31.032257 pysect-0.0.3/src/pysect/filament/
+-rwxrwx---   0 anonoei    (501) staff       (20)        0 2024-05-27 04:44:17.000000 pysect-0.0.3/src/pysect/filament/__init__.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      431 2024-05-27 05:38:59.000000 pysect-0.0.3/src/pysect/filament/filament.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1140 2024-05-21 03:35:17.000000 pysect-0.0.3/src/pysect/main.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-27 05:52:31.032687 pysect-0.0.3/src/pysect/primitives/
+-rwxrwx---   0 anonoei    (501) staff       (20)        0 2024-05-27 04:44:18.000000 pysect-0.0.3/src/pysect/primitives/__init__.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      294 2024-05-21 01:52:08.000000 pysect-0.0.3/src/pysect/primitives/coord.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-27 05:52:31.033115 pysect-0.0.3/src/pysect/printer/
+-rwxrwx---   0 anonoei    (501) staff       (20)        0 2024-05-27 04:44:21.000000 pysect-0.0.3/src/pysect/printer/__init__.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1075 2024-05-27 05:39:11.000000 pysect-0.0.3/src/pysect/printer/printer.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-27 05:52:31.033949 pysect-0.0.3/src/pysect/sect/
+-rwxrwx---   0 anonoei    (501) staff       (20)        0 2024-05-20 09:39:52.000000 pysect-0.0.3/src/pysect/sect/__init__.py
+-rwxrwx---   0 anonoei    (501) staff       (20)       81 2024-05-21 03:17:16.000000 pysect-0.0.3/src/pysect/sect/config.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-27 05:52:31.034620 pysect-0.0.3/src/pysect/sect/primitives/
+-rwxrwx---   0 anonoei    (501) staff       (20)        0 2024-05-20 09:40:02.000000 pysect-0.0.3/src/pysect/sect/primitives/__init__.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2643 2024-05-21 03:04:27.000000 pysect-0.0.3/src/pysect/sect/primitives/mesh.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      738 2024-05-20 09:40:23.000000 pysect-0.0.3/src/pysect/sect/primitives/stl.py
+-rwxrwx---   0 anonoei    (501) staff       (20)        0 2024-05-20 03:11:04.000000 pysect-0.0.3/src/pysect/sect/sect.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-27 05:52:31.035006 pysect-0.0.3/src/pysect/sect/serial/
+-rwxrwx---   0 anonoei    (501) staff       (20)        0 2024-05-20 09:40:01.000000 pysect-0.0.3/src/pysect/sect/serial/__init__.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2255 2024-05-20 09:40:08.000000 pysect-0.0.3/src/pysect/sect/serial/stl.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      465 2024-05-21 03:26:48.000000 pysect-0.0.3/src/pysect/sect/slice.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-27 05:52:31.035459 pysect-0.0.3/src/pysect/slice/
+-rwxrwx---   0 anonoei    (501) staff       (20)        0 2024-05-27 04:44:29.000000 pysect-0.0.3/src/pysect/slice/__init__.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      624 2024-05-27 05:39:21.000000 pysect-0.0.3/src/pysect/slice/slice.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-27 05:52:31.035762 pysect-0.0.3/src/pysect.egg-info/
+-rw-r--r--   0 anonoei    (501) staff       (20)     1581 2024-05-27 05:52:31.000000 pysect-0.0.3/src/pysect.egg-info/PKG-INFO
+-rwxrwx---   0 anonoei    (501) staff       (20)      822 2024-05-27 05:52:31.000000 pysect-0.0.3/src/pysect.egg-info/SOURCES.txt
+-rwxrwx---   0 anonoei    (501) staff       (20)        1 2024-05-27 05:52:31.000000 pysect-0.0.3/src/pysect.egg-info/dependency_links.txt
+-rwxrwx---   0 anonoei    (501) staff       (20)       80 2024-05-27 05:52:31.000000 pysect-0.0.3/src/pysect.egg-info/requires.txt
+-rwxrwx---   0 anonoei    (501) staff       (20)        7 2024-05-27 05:52:31.000000 pysect-0.0.3/src/pysect.egg-info/top_level.txt
```

### Comparing `pysect-0.0.2/LICENSE` & `pysect-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysect-0.0.2/PKG-INFO` & `pysect-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysect
-Version: 0.0.2
+Version: 0.0.3
 Summary: A standalone 3D object slicer
 Author-email: Anonoei <dev@anonoei.com>
 Project-URL: Homepage, https://github.com/anonoei/pysect
 Project-URL: Documentation, https://anonoei.github.io/pysect/
 Project-URL: Repository, https://github.com/Anonoei/pysect.git
 Project-URL: Issues, https://github.com/Anonoei/pysect/issues
 Project-URL: Source, https://github.com/anonoei/pysect
```

### Comparing `pysect-0.0.2/pyproject.toml` & `pysect-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysect"
-version = "0.0.2"
+version = "0.0.3"
 description = "A standalone 3D object slicer"
 dependencies = ["pyboiler_anonoei", "numpy", "matplotlib"]
 requires-python = ">=3.6"
 authors = [
     {name = "Anonoei", email="dev@anonoei.com"}
 ]
 readme = "README.md"
@@ -31,15 +31,15 @@
 Issues = "https://github.com/Anonoei/pysect/issues"
 Source = "https://github.com/anonoei/pysect"
 
 [project.optional-dependencies]
 dev = ["twine", "build", "black", "bumpver", "pytest", "pdoc3"]
 
 [tool.bumpver]
-current_version = "0.0.2"
+current_version = "0.0.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `pysect-0.0.2/src/pysect/sect/primitives/stl.py` & `pysect-0.0.3/src/pysect/sect/primitives/stl.py`

 * *Files identical despite different names*

### Comparing `pysect-0.0.2/src/pysect/sect/serial/stl.py` & `pysect-0.0.3/src/pysect/sect/serial/stl.py`

 * *Files identical despite different names*

### Comparing `pysect-0.0.2/src/pysect.egg-info/PKG-INFO` & `pysect-0.0.3/src/pysect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysect
-Version: 0.0.2
+Version: 0.0.3
 Summary: A standalone 3D object slicer
 Author-email: Anonoei <dev@anonoei.com>
 Project-URL: Homepage, https://github.com/anonoei/pysect
 Project-URL: Documentation, https://anonoei.github.io/pysect/
 Project-URL: Repository, https://github.com/Anonoei/pysect.git
 Project-URL: Issues, https://github.com/Anonoei/pysect/issues
 Project-URL: Source, https://github.com/anonoei/pysect
```

### Comparing `pysect-0.0.2/src/pysect.egg-info/SOURCES.txt` & `pysect-0.0.3/src/pysect.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,26 @@
 src/pysect/__init__.py
 src/pysect/main.py
 src/pysect.egg-info/PKG-INFO
 src/pysect.egg-info/SOURCES.txt
 src/pysect.egg-info/dependency_links.txt
 src/pysect.egg-info/requires.txt
 src/pysect.egg-info/top_level.txt
+src/pysect/config/__init__.py
+src/pysect/config/config.py
+src/pysect/filament/__init__.py
+src/pysect/filament/filament.py
+src/pysect/primitives/__init__.py
 src/pysect/primitives/coord.py
+src/pysect/printer/__init__.py
+src/pysect/printer/printer.py
 src/pysect/sect/__init__.py
 src/pysect/sect/config.py
 src/pysect/sect/sect.py
 src/pysect/sect/slice.py
 src/pysect/sect/primitives/__init__.py
 src/pysect/sect/primitives/mesh.py
 src/pysect/sect/primitives/stl.py
 src/pysect/sect/serial/__init__.py
-src/pysect/sect/serial/stl.py
+src/pysect/sect/serial/stl.py
+src/pysect/slice/__init__.py
+src/pysect/slice/slice.py
```

