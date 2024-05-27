# Comparing `tmp/font_fjallaone-0.1.4.tar.gz` & `tmp/font_fjallaone-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "font_fjallaone-0.1.4.tar", max compression
+gzip compressed data, was "font_fjallaone-0.1.5.tar", max compression
```

## Comparing `font_fjallaone-0.1.4.tar` & `font_fjallaone-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1904 2024-05-06 16:37:44.936934 font_fjallaone-0.1.4/README.md
--rw-r--r--   0        0        0      397 2024-05-06 16:37:44.936934 font_fjallaone-0.1.4/font_fjallaone/__init__.py
--rw-r--r--   0        0        0    34848 2024-05-06 16:37:44.936934 font_fjallaone-0.1.4/font_fjallaone/files/FjallaOne-Regular.ttf
--rw-r--r--   0        0        0     1348 2024-05-06 16:38:00.424793 font_fjallaone-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2306 1970-01-01 00:00:00.000000 font_fjallaone-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1904 2024-05-27 21:52:44.579599 font_fjallaone-0.1.5/README.md
+-rw-r--r--   0        0        0      397 2024-05-27 21:52:44.579599 font_fjallaone-0.1.5/font_fjallaone/__init__.py
+-rw-r--r--   0        0        0    34848 2024-05-27 21:52:44.579599 font_fjallaone-0.1.5/font_fjallaone/files/FjallaOne-Regular.ttf
+-rw-r--r--   0        0        0     1348 2024-05-27 21:52:56.583556 font_fjallaone-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2306 1970-01-01 00:00:00.000000 font_fjallaone-0.1.5/PKG-INFO
```

### Comparing `font_fjallaone-0.1.4/README.md` & `font_fjallaone-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `font_fjallaone-0.1.4/font_fjallaone/files/FjallaOne-Regular.ttf` & `font_fjallaone-0.1.5/font_fjallaone/files/FjallaOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `font_fjallaone-0.1.4/pyproject.toml` & `font_fjallaone-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "font-fjallaone"
-version = "v0.1.4" # 0.0.0 placeholder is replaced on release
+version = "v0.1.5" # 0.0.0 placeholder is replaced on release
 description = "Fjalla One from from Sorkin Type as distributed by Google Fonts"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 readme = "README.md"
 packages = [
     { include = "font_fjallaone"},
 ]
 include = ["font_fjallaone/files"]
```

### Comparing `font_fjallaone-0.1.4/PKG-INFO` & `font_fjallaone-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: font-fjallaone
-Version: 0.1.4
+Version: 0.1.5
 Summary: Fjalla One from from Sorkin Type as distributed by Google Fonts
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

