# Comparing `tmp/lckytools-0.0.0b2.tar.gz` & `tmp/lckytools-0.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lckytools-0.0.0b2.tar", max compression
+gzip compressed data, was "lckytools-0.0.0b3.tar", max compression
```

## Comparing `lckytools-0.0.0b2.tar` & `lckytools-0.0.0b3.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0     1096 2024-05-27 01:00:50.888092 lckytools-0.0.0b2/LICENSE
--rw-r--r--   0        0        0     1167 2024-05-27 01:18:41.478578 lckytools-0.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0b2/README.md
--rw-r--r--   0        0        0        0 2024-05-27 00:52:12.425121 lckytools-0.0.0b2/src/lckytools/__init__.py
--rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 lckytools-0.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-27 01:00:50.888092 lckytools-0.0.0b3/LICENSE
+-rw-r--r--   0        0        0     1238 2024-05-27 01:39:53.951981 lckytools-0.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0b3/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 00:52:12.425121 lckytools-0.0.0b3/src/lckytools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0b3/src/lckytools/NN/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0b3/src/lckytools/NN/metrics/__init__.py
+-rw-r--r--   0        0        0      794 2024-05-27 01:33:41.944308 lckytools-0.0.0b3/src/lckytools/NN/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0b3/src/lckytools/NN/torch/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-27 01:35:29.762996 lckytools-0.0.0b3/src/lckytools/NN/torch/summary_model.py
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 lckytools-0.0.0b3/PKG-INFO
```

### Comparing `lckytools-0.0.0b2/LICENSE` & `lckytools-0.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0b2/pyproject.toml` & `lckytools-0.0.0b3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lckytools"
-version = "0.0.0b2"
+version = "0.0.0b3"
 description = "A collection of helpful utility functions and tools."
 authors = ["Your Name <your.email@example.com>"]
 license = "MIT"
 
 readme = "README.md"
 homepage = "https://github.com/yourusername/lckytools"
 repository = "https://github.com/yourusername/lckytools"
@@ -19,16 +19,20 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 
 [tool.poetry.dependencies]
+numpy = "^1.26.2"
+pandas = "^2.1.4"
 python = "^3.7"
-# Add your package dependencies here
+scikit-learn = "^1.3.2"
+seaborn = "^0.13.0"
+torchsummary = "^1.5.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 # Add your development dependencies here
 
 [tool.poetry.scripts]
 # Add any command-line scripts provided by your package here
```

### Comparing `lckytools-0.0.0b2/README.md` & `lckytools-0.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0b2/PKG-INFO` & `lckytools-0.0.0b3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lckytools
-Version: 0.0.0b2
+Version: 0.0.0b3
 Summary: A collection of helpful utility functions and tools.
 Home-page: https://github.com/yourusername/lckytools
 License: MIT
 Author: Your Name
 Author-email: your.email@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -15,14 +15,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: numpy (>=1.26.2,<2.0.0)
+Requires-Dist: pandas (>=2.1.4,<3.0.0)
+Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
+Requires-Dist: seaborn (>=0.13.0,<0.14.0)
+Requires-Dist: torchsummary (>=1.5.1,<2.0.0)
 Project-URL: Documentation, https://yourusername.github.io/lckytools
 Project-URL: Repository, https://github.com/yourusername/lckytools
 Description-Content-Type: text/markdown
 
 # LckyTools
 
 this sentence below I use chatGPT to generate it, it's not real, but looks like real, I will update it later.
```

