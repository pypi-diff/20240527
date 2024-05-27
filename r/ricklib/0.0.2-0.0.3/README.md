# Comparing `tmp/ricklib-0.0.2.tar.gz` & `tmp/ricklib-0.0.3.tar.gz`

## Comparing `ricklib-0.0.2.tar` & `ricklib-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ricklib-0.0.2/src/ricklib/__init__.py
--rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 ricklib-0.0.2/src/ricklib/pngenerator.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ricklib-0.0.2/tests/graphic_test.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 ricklib-0.0.2/LICENSE
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ricklib-0.0.2/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 ricklib-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ricklib-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ricklib-0.0.3/src/ricklib/__init__.py
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 ricklib-0.0.3/src/ricklib/audio.py
+-rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 ricklib-0.0.3/src/ricklib/pngenerator.py
+-rw-r--r--   0        0        0   352844 2020-02-02 00:00:00.000000 ricklib-0.0.3/tests/audio.wav
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 ricklib-0.0.3/tests/graphic_test.py
+-rw-r--r--   0        0        0   125130 2020-02-02 00:00:00.000000 ricklib-0.0.3/tests/testc.png
+-rw-r--r--   0        0        0    65865 2020-02-02 00:00:00.000000 ricklib-0.0.3/tests/testg.png
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 ricklib-0.0.3/LICENSE
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 ricklib-0.0.3/README.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ricklib-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 ricklib-0.0.3/PKG-INFO
```

### Comparing `ricklib-0.0.2/src/ricklib/pngenerator.py` & `ricklib-0.0.3/src/ricklib/pngenerator.py`

 * *Files identical despite different names*

### Comparing `ricklib-0.0.2/LICENSE` & `ricklib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ricklib-0.0.2/pyproject.toml` & `ricklib-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ricklib"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
-  { name="Richard (Rick) Howell", email="rick.howell.arts@gmail.com" },
+  {name="Richard (Rick) Howell", email="rick.howell.arts@gmail.com"},
 ]
 description = "A small package for personal use including useful operations."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+license = {file = "LICENSE"}
 
 [project.urls]
 Homepage = "https://github.com/rick-howell/ricklib"
 Issues = "https://github.com/rick-howell/ricklib/issues"
```

