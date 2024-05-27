# Comparing `tmp/undumper-0.0.3.tar.gz` & `tmp/undumper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undumper-0.0.3.tar", max compression
+gzip compressed data, was "undumper-0.0.4.tar", max compression
```

## Comparing `undumper-0.0.3.tar` & `undumper-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2024-05-27 16:39:55.216790 undumper-0.0.3/LICENSE
--rw-r--r--   0        0        0     2928 2024-05-27 16:39:55.220790 undumper-0.0.3/README.md
--rw-r--r--   0        0        0      445 2024-05-27 16:39:55.220790 undumper-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-27 16:39:55.220790 undumper-0.0.3/undumper/__init__.py
--rw-r--r--   0        0        0     6830 2024-05-27 16:39:55.220790 undumper-0.0.3/undumper/undumper.py
--rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 undumper-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-27 17:06:57.356917 undumper-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2928 2024-05-27 17:06:57.356917 undumper-0.0.4/README.md
+-rw-r--r--   0        0        0      445 2024-05-27 17:06:57.356917 undumper-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 17:06:57.356917 undumper-0.0.4/undumper/__init__.py
+-rw-r--r--   0        0        0     6829 2024-05-27 17:06:57.356917 undumper-0.0.4/undumper/undumper.py
+-rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 undumper-0.0.4/PKG-INFO
```

### Comparing `undumper-0.0.3/LICENSE` & `undumper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `undumper-0.0.3/README.md` & `undumper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `undumper-0.0.3/undumper/undumper.py` & `undumper-0.0.4/undumper/undumper.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                 mode = Modes.GRID_S
                 checkLoop = loopCount
             if mode == Modes.GRID_S and (loopCount - checkLoop) == 1:
                 unDumped["GRID SIZE"] = line.split() 
             if "GRID CELLS" in line:
                 mode = Modes.GRID_C
                 checkLoop = loopCount
-                gridName = line.split()[3] u
+                gridName = line.split()[3] 
                 unDumped[gridName] = {}
                 gridID = 1
             if mode == Modes.GRID_C and (loopCount - checkLoop) >= 1:
                 unDumped[gridName][gridID] = line
                 gridID += 1
             if frameCount > 1 and unDumped and (loopCount - frameLength) % (gridID + 10) == 0:
                 yield unDumped
```

### Comparing `undumper-0.0.3/PKG-INFO` & `undumper-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unDumper
-Version: 0.0.3
+Version: 0.0.4
 Summary: A fast and memory-efficient LAMMPS dump file reader with great developer experience
 License: MIT
 Author: Mohid Farooqi
 Author-email: mu2farooqi@uwaterloo.ca
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

