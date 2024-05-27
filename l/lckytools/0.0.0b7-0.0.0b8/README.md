# Comparing `tmp/lckytools-0.0.0b7.tar.gz` & `tmp/lckytools-0.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lckytools-0.0.0b7.tar", max compression
+gzip compressed data, was "lckytools-0.0.0b8.tar", max compression
```

## Comparing `lckytools-0.0.0b7.tar` & `lckytools-0.0.0b8.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1096 2024-05-27 01:00:50.888092 lckytools-0.0.0b7/LICENSE
--rw-r--r--   0        0        0     1238 2024-05-27 02:10:10.610498 lckytools-0.0.0b7/pyproject.toml
--rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0b7/README.md
--rw-r--r--   0        0        0        0 2024-05-27 00:52:12.425121 lckytools-0.0.0b7/src/lckytools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0b7/src/lckytools/NN/__init__.py
--rw-r--r--   0        0        0      121 2024-05-27 02:09:46.372713 lckytools-0.0.0b7/src/lckytools/NN/metrics/__init__.py
--rw-r--r--   0        0        0      808 2024-05-27 02:10:02.414496 lckytools-0.0.0b7/src/lckytools/NN/metrics/confusion_matrix.py
--rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0b7/src/lckytools/NN/torch/__init__.py
--rw-r--r--   0        0        0       34 2024-05-27 01:45:10.349737 lckytools-0.0.0b7/src/lckytools/NN/torch/summary_model.py
--rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 lckytools-0.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-27 01:00:50.888092 lckytools-0.0.0b8/LICENSE
+-rw-r--r--   0        0        0     1238 2024-05-27 02:13:53.463028 lckytools-0.0.0b8/pyproject.toml
+-rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0b8/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 00:52:12.425121 lckytools-0.0.0b8/src/lckytools/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-27 02:13:47.450724 lckytools-0.0.0b8/src/lckytools/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0b8/src/lckytools/NN/__init__.py
+-rw-r--r--   0        0        0      144 2024-05-27 02:10:58.751794 lckytools-0.0.0b8/src/lckytools/NN/metrics/__init__.py
+-rw-r--r--   0        0        0      829 2024-05-27 02:10:59.000094 lckytools-0.0.0b8/src/lckytools/NN/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0b8/src/lckytools/NN/torch/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-27 01:45:10.349737 lckytools-0.0.0b8/src/lckytools/NN/torch/summary_model.py
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 lckytools-0.0.0b8/PKG-INFO
```

### Comparing `lckytools-0.0.0b7/LICENSE` & `lckytools-0.0.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0b7/pyproject.toml` & `lckytools-0.0.0b8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lckytools"
-version = "0.0.0b7"
+version = "0.0.0b8"
 description = "A collection of helpful utility functions and tools."
 authors = ["Your Name <your.email@example.com>"]
 license = "MIT"
 
 readme = "README.md"
 homepage = "https://github.com/yourusername/lckytools"
 repository = "https://github.com/yourusername/lckytools"
```

### Comparing `lckytools-0.0.0b7/README.md` & `lckytools-0.0.0b8/README.md`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0b7/src/lckytools/NN/metrics/confusion_matrix.py` & `lckytools-0.0.0b8/src/lckytools/NN/metrics/confusion_matrix.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 
     sns.heatmap(df_cm, annot=True, fmt="0.0f")
     plt.xlabel("Predicted Class", fontsize=14)
     plt.ylabel("Actual Class", fontsize=14)
     plt.title("Confusion Matrix", fontsize=16)
 
 
-def test
+def test():
+    print("asd")
```

### Comparing `lckytools-0.0.0b7/PKG-INFO` & `lckytools-0.0.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lckytools
-Version: 0.0.0b7
+Version: 0.0.0b8
 Summary: A collection of helpful utility functions and tools.
 Home-page: https://github.com/yourusername/lckytools
 License: MIT
 Author: Your Name
 Author-email: your.email@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

