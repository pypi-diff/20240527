# Comparing `tmp/wsgenerator-1.0.0.tar.gz` & `tmp/wsgenerator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsgenerator-1.0.0.tar", last modified: Mon May 20 23:28:33 2024, max compression
+gzip compressed data, was "wsgenerator-1.0.1.tar", last modified: Mon May 27 01:29:54 2024, max compression
```

## Comparing `wsgenerator-1.0.0.tar` & `wsgenerator-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 23:28:33.639935 wsgenerator-1.0.0/
--rw-rw-rw-   0        0        0     1101 2024-05-19 17:43:11.000000 wsgenerator-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3099 2024-05-20 23:28:33.633876 wsgenerator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2420 2024-05-20 00:29:13.000000 wsgenerator-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-20 23:28:33.639935 wsgenerator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1005 2024-05-20 00:59:37.000000 wsgenerator-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 23:28:33.631414 wsgenerator-1.0.0/wsgenerator/
--rw-rw-rw-   0        0        0       28 2024-05-20 23:16:55.000000 wsgenerator-1.0.0/wsgenerator/__init__.py
--rw-rw-rw-   0        0        0    14014 2024-05-20 00:28:00.000000 wsgenerator-1.0.0/wsgenerator/wsgenerator.py
-drwxrwxrwx   0        0        0        0 2024-05-20 23:28:33.633876 wsgenerator-1.0.0/wsgenerator.egg-info/
--rw-rw-rw-   0        0        0     3099 2024-05-20 23:28:33.000000 wsgenerator-1.0.0/wsgenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-05-20 23:28:33.000000 wsgenerator-1.0.0/wsgenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 23:28:33.000000 wsgenerator-1.0.0/wsgenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-20 23:28:33.000000 wsgenerator-1.0.0/wsgenerator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 01:29:54.425098 wsgenerator-1.0.1/
+-rw-rw-rw-   0        0        0     1101 2024-05-19 17:43:11.000000 wsgenerator-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3099 2024-05-27 01:29:54.423898 wsgenerator-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2420 2024-05-20 00:29:13.000000 wsgenerator-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 01:29:54.425098 wsgenerator-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2024-05-27 01:29:39.000000 wsgenerator-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:29:54.407900 wsgenerator-1.0.1/wsgenerator/
+-rw-rw-rw-   0        0        0       28 2024-05-20 23:16:55.000000 wsgenerator-1.0.1/wsgenerator/__init__.py
+-rw-rw-rw-   0        0        0    14021 2024-05-27 01:26:41.000000 wsgenerator-1.0.1/wsgenerator/wsgenerator.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:29:54.422900 wsgenerator-1.0.1/wsgenerator.egg-info/
+-rw-rw-rw-   0        0        0     3099 2024-05-27 01:29:54.000000 wsgenerator-1.0.1/wsgenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-27 01:29:54.000000 wsgenerator-1.0.1/wsgenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 01:29:54.000000 wsgenerator-1.0.1/wsgenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 01:29:54.000000 wsgenerator-1.0.1/wsgenerator.egg-info/top_level.txt
```

### Comparing `wsgenerator-1.0.0/LICENSE` & `wsgenerator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wsgenerator-1.0.0/PKG-INFO` & `wsgenerator-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsgenerator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Module for generating word search puzzles
 Home-page: https://github.com/pgolo/wsgenerator
 Author: Pavel Golovatenko-Abramov
 Author-email: p.golovatenko@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wsgenerator-1.0.0/README.md` & `wsgenerator-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wsgenerator-1.0.0/setup.py` & `wsgenerator-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ext_modules = None
 with open('README.md', mode='r', encoding='utf8') as f:
     long_description = f.read()
 
 setup(
     name='wsgenerator',
-    version='1.0.0',
+    version='1.0.1',
     description='Module for generating word search puzzles',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/pgolo/wsgenerator',
     author='Pavel Golovatenko-Abramov',
     author_email='p.golovatenko@gmail.com',
     packages=['wsgenerator'],
```

### Comparing `wsgenerator-1.0.0/wsgenerator/wsgenerator.py` & `wsgenerator-1.0.1/wsgenerator/wsgenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     while True:
         solution, y, x, direction, letters = placements(grid, _words, grid_height, grid_width, _points)
         if solution:
             hints[word] = (y, x, direction, letters)
         else:
             return [], None, None, None, None
         if word_index < len(words) - 1:
-            temp, _, _, _, _ = trace_grids(solution, words, word_index + 1, grid_height, grid_width, hints, points)
+            temp, _, _, _, _ = trace_grids(solution, words, word_index + 1, grid_height, grid_width, hints, points, level)
             if len(temp) > 0:
                 return temp, None, None, None, None
             del hints[word]
         else:
             return solution, None, None, None, None
 
 def make_puzzle(height: int, width: int, words: list, grid: list, level: int=0):
```

### Comparing `wsgenerator-1.0.0/wsgenerator.egg-info/PKG-INFO` & `wsgenerator-1.0.1/wsgenerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsgenerator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Module for generating word search puzzles
 Home-page: https://github.com/pgolo/wsgenerator
 Author: Pavel Golovatenko-Abramov
 Author-email: p.golovatenko@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

