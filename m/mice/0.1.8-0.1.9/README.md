# Comparing `tmp/mice-0.1.8.tar.gz` & `tmp/mice-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mice-0.1.8.tar", last modified: Wed Oct  6 13:25:13 2021, max compression
+gzip compressed data, was "mice-0.1.9.tar", last modified: Wed Oct  6 13:29:35 2021, max compression
```

## Comparing `mice-0.1.8.tar` & `mice-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:25:13.014310 mice-0.1.8/
--rw-rw-r--   0 andre     (1000) andre     (1000)    34756 2021-03-28 11:34:43.000000 mice-0.1.8/LICENSE
--rw-rw-r--   0 andre     (1000) andre     (1000)       56 2021-09-30 15:24:08.000000 mice-0.1.8/MANIFEST.in
--rw-rw-r--   0 andre     (1000) andre     (1000)     1889 2021-10-06 13:25:13.014310 mice-0.1.8/PKG-INFO
--rw-rw-r--   0 andre     (1000) andre     (1000)     1587 2021-10-06 13:22:02.000000 mice-0.1.8/README.rst
--rw-rw-r--   0 andre     (1000) andre     (1000)       42 2021-10-04 07:55:34.000000 mice-0.1.8/REQUIREMENTS
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:25:13.006309 mice-0.1.8/docs/
--rw-rw-r--   0 andre     (1000) andre     (1000)      638 2021-09-30 15:24:08.000000 mice-0.1.8/docs/Makefile
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:25:13.006309 mice-0.1.8/docs/build/
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:25:13.006309 mice-0.1.8/docs/build/doctrees/
--rw-rw-r--   0 andre     (1000) andre     (1000)    27027 2021-10-05 15:04:26.000000 mice-0.1.8/docs/build/doctrees/environment.pickle
--rw-rw-r--   0 andre     (1000) andre     (1000)     5576 2021-10-05 14:54:03.000000 mice-0.1.8/docs/build/doctrees/index.doctree
--rw-rw-r--   0 andre     (1000) andre     (1000)     4401 2021-10-05 14:54:03.000000 mice-0.1.8/docs/build/doctrees/intro.doctree
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:25:13.010309 mice-0.1.8/docs/build/html/
--rw-rw-r--   0 andre     (1000) andre     (1000)      230 2021-10-05 15:04:26.000000 mice-0.1.8/docs/build/html/.buildinfo
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:25:13.010309 mice-0.1.8/docs/build/html/_sources/
--rw-rw-r--   0 andre     (1000) andre     (1000)      568 2021-10-04 14:04:38.000000 mice-0.1.8/docs/build/html/_sources/index.rst.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)      660 2021-09-30 15:24:08.000000 mice-0.1.8/docs/build/html/_sources/intro.rst.txt
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:25:13.010309 mice-0.1.8/docs/build/html/_static/
--rw-rw-r--   0 andre     (1000) andre     (1000)    14638 2021-10-05 15:04:26.000000 mice-0.1.8/docs/build/html/_static/basic.css
--rw-rw-r--   0 andre     (1000) andre     (1000)     9630 2021-09-26 07:36:39.000000 mice-0.1.8/docs/build/html/_static/doctools.js
--rw-rw-r--   0 andre     (1000) andre     (1000)      353 2021-10-05 15:04:26.000000 mice-0.1.8/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 andre     (1000) andre     (1000)      286 2021-09-26 07:36:39.000000 mice-0.1.8/docs/build/html/_static/file.png
--rw-rw-r--   0 andre     (1000) andre     (1000)   287630 2021-09-26 07:36:39.000000 mice-0.1.8/docs/build/html/_static/jquery-3.5.1.js
--rw-rw-r--   0 andre     (1000) andre     (1000)    89476 2021-09-26 07:36:39.000000 mice-0.1.8/docs/build/html/_static/jquery.js
--rw-rw-r--   0 andre     (1000) andre     (1000)    10854 2021-10-05 15:04:26.000000 mice-0.1.8/docs/build/html/_static/language_data.js
--rw-rw-r--   0 andre     (1000) andre     (1000)       90 2021-09-26 07:36:39.000000 mice-0.1.8/docs/build/html/_static/minus.png
--rw-rw-r--   0 andre     (1000) andre     (1000)       90 2021-09-26 07:36:39.000000 mice-0.1.8/docs/build/html/_static/plus.png
--rw-rw-r--   0 andre     (1000) andre     (1000)     4368 2021-10-05 15:04:26.000000 mice-0.1.8/docs/build/html/_static/pygments.css
--rw-rw-r--   0 andre     (1000) andre     (1000)    16733 2021-09-26 07:36:39.000000 mice-0.1.8/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 andre     (1000) andre     (1000)    68420 2021-09-26 07:36:39.000000 mice-0.1.8/docs/build/html/_static/underscore-1.13.1.js
--rw-rw-r--   0 andre     (1000) andre     (1000)    19530 2021-09-26 07:36:39.000000 mice-0.1.8/docs/build/html/_static/underscore.js
--rw-rw-r--   0 andre     (1000) andre     (1000)     9058 2021-10-06 11:05:16.000000 mice-0.1.8/docs/build/html/genindex.html
--rw-rw-r--   0 andre     (1000) andre     (1000)     5690 2021-10-05 15:04:26.000000 mice-0.1.8/docs/build/html/index.html
--rw-rw-r--   0 andre     (1000) andre     (1000)     5041 2021-10-05 14:54:03.000000 mice-0.1.8/docs/build/html/intro.html
--rw-rw-r--   0 andre     (1000) andre     (1000)      830 2021-10-05 15:04:26.000000 mice-0.1.8/docs/build/html/objects.inv
--rw-rw-r--   0 andre     (1000) andre     (1000)     3869 2021-10-05 15:04:26.000000 mice-0.1.8/docs/build/html/search.html
--rw-rw-r--   0 andre     (1000) andre     (1000)     8642 2021-10-05 15:04:26.000000 mice-0.1.8/docs/build/html/searchindex.js
--rw-rw-r--   0 andre     (1000) andre     (1000)      804 2021-09-30 15:24:08.000000 mice-0.1.8/docs/make.bat
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:25:13.010309 mice-0.1.8/docs/source/
--rw-rw-r--   0 andre     (1000) andre     (1000)     2018 2021-10-06 13:24:42.000000 mice-0.1.8/docs/source/conf.py
--rw-rw-r--   0 andre     (1000) andre     (1000)      568 2021-10-04 14:04:38.000000 mice-0.1.8/docs/source/index.rst
--rw-rw-r--   0 andre     (1000) andre     (1000)      660 2021-09-30 15:24:08.000000 mice-0.1.8/docs/source/intro.rst
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:25:13.010309 mice-0.1.8/mice/
--rw-rw-r--   0 andre     (1000) andre     (1000)       92 2021-10-05 06:44:01.000000 mice-0.1.8/mice/__init__.py
--rw-rw-r--   0 andre     (1000) andre     (1000)    20891 2021-10-05 06:37:18.000000 mice-0.1.8/mice/deltas.py
--rw-rw-r--   0 andre     (1000) andre     (1000)    25752 2021-10-06 12:48:29.000000 mice-0.1.8/mice/mice.py
--rw-rw-r--   0 andre     (1000) andre     (1000)     3504 2021-10-05 11:35:52.000000 mice-0.1.8/mice/plot_mice.py
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:25:13.010309 mice-0.1.8/mice.egg-info/
--rw-rw-r--   0 andre     (1000) andre     (1000)     1889 2021-10-06 13:25:12.000000 mice-0.1.8/mice.egg-info/PKG-INFO
--rw-rw-r--   0 andre     (1000) andre     (1000)     1237 2021-10-06 13:25:12.000000 mice-0.1.8/mice.egg-info/SOURCES.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)        1 2021-10-06 13:25:12.000000 mice-0.1.8/mice.egg-info/dependency_links.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)       42 2021-10-06 13:25:12.000000 mice-0.1.8/mice.egg-info/requires.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)        5 2021-10-06 13:25:12.000000 mice-0.1.8/mice.egg-info/top_level.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)      185 2021-10-05 14:17:04.000000 mice-0.1.8/pyproject.toml
--rw-rw-r--   0 andre     (1000) andre     (1000)       38 2021-10-06 13:25:13.014310 mice-0.1.8/setup.cfg
--rw-rw-r--   0 andre     (1000) andre     (1000)      769 2021-10-06 13:24:40.000000 mice-0.1.8/setup.py
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:29:35.292666 mice-0.1.9/
+-rw-rw-r--   0 andre     (1000) andre     (1000)    34756 2021-03-28 11:34:43.000000 mice-0.1.9/LICENSE
+-rw-rw-r--   0 andre     (1000) andre     (1000)       56 2021-09-30 15:24:08.000000 mice-0.1.9/MANIFEST.in
+-rw-rw-r--   0 andre     (1000) andre     (1000)     1890 2021-10-06 13:29:35.292666 mice-0.1.9/PKG-INFO
+-rw-rw-r--   0 andre     (1000) andre     (1000)     1588 2021-10-06 13:28:28.000000 mice-0.1.9/README.rst
+-rw-rw-r--   0 andre     (1000) andre     (1000)       42 2021-10-04 07:55:34.000000 mice-0.1.9/REQUIREMENTS
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:29:35.288666 mice-0.1.9/docs/
+-rw-rw-r--   0 andre     (1000) andre     (1000)      638 2021-09-30 15:24:08.000000 mice-0.1.9/docs/Makefile
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:29:35.288666 mice-0.1.9/docs/build/
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:29:35.288666 mice-0.1.9/docs/build/doctrees/
+-rw-rw-r--   0 andre     (1000) andre     (1000)    27027 2021-10-05 15:04:26.000000 mice-0.1.9/docs/build/doctrees/environment.pickle
+-rw-rw-r--   0 andre     (1000) andre     (1000)     5576 2021-10-05 14:54:03.000000 mice-0.1.9/docs/build/doctrees/index.doctree
+-rw-rw-r--   0 andre     (1000) andre     (1000)     4401 2021-10-05 14:54:03.000000 mice-0.1.9/docs/build/doctrees/intro.doctree
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:29:35.288666 mice-0.1.9/docs/build/html/
+-rw-rw-r--   0 andre     (1000) andre     (1000)      230 2021-10-05 15:04:26.000000 mice-0.1.9/docs/build/html/.buildinfo
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:29:35.288666 mice-0.1.9/docs/build/html/_sources/
+-rw-rw-r--   0 andre     (1000) andre     (1000)      568 2021-10-04 14:04:38.000000 mice-0.1.9/docs/build/html/_sources/index.rst.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)      660 2021-09-30 15:24:08.000000 mice-0.1.9/docs/build/html/_sources/intro.rst.txt
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:29:35.292666 mice-0.1.9/docs/build/html/_static/
+-rw-rw-r--   0 andre     (1000) andre     (1000)    14638 2021-10-05 15:04:26.000000 mice-0.1.9/docs/build/html/_static/basic.css
+-rw-rw-r--   0 andre     (1000) andre     (1000)     9630 2021-09-26 07:36:39.000000 mice-0.1.9/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 andre     (1000) andre     (1000)      353 2021-10-05 15:04:26.000000 mice-0.1.9/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 andre     (1000) andre     (1000)      286 2021-09-26 07:36:39.000000 mice-0.1.9/docs/build/html/_static/file.png
+-rw-rw-r--   0 andre     (1000) andre     (1000)   287630 2021-09-26 07:36:39.000000 mice-0.1.9/docs/build/html/_static/jquery-3.5.1.js
+-rw-rw-r--   0 andre     (1000) andre     (1000)    89476 2021-09-26 07:36:39.000000 mice-0.1.9/docs/build/html/_static/jquery.js
+-rw-rw-r--   0 andre     (1000) andre     (1000)    10854 2021-10-05 15:04:26.000000 mice-0.1.9/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 andre     (1000) andre     (1000)       90 2021-09-26 07:36:39.000000 mice-0.1.9/docs/build/html/_static/minus.png
+-rw-rw-r--   0 andre     (1000) andre     (1000)       90 2021-09-26 07:36:39.000000 mice-0.1.9/docs/build/html/_static/plus.png
+-rw-rw-r--   0 andre     (1000) andre     (1000)     4368 2021-10-05 15:04:26.000000 mice-0.1.9/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 andre     (1000) andre     (1000)    16733 2021-09-26 07:36:39.000000 mice-0.1.9/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 andre     (1000) andre     (1000)    68420 2021-09-26 07:36:39.000000 mice-0.1.9/docs/build/html/_static/underscore-1.13.1.js
+-rw-rw-r--   0 andre     (1000) andre     (1000)    19530 2021-09-26 07:36:39.000000 mice-0.1.9/docs/build/html/_static/underscore.js
+-rw-rw-r--   0 andre     (1000) andre     (1000)     9058 2021-10-06 11:05:16.000000 mice-0.1.9/docs/build/html/genindex.html
+-rw-rw-r--   0 andre     (1000) andre     (1000)     5690 2021-10-05 15:04:26.000000 mice-0.1.9/docs/build/html/index.html
+-rw-rw-r--   0 andre     (1000) andre     (1000)     5041 2021-10-05 14:54:03.000000 mice-0.1.9/docs/build/html/intro.html
+-rw-rw-r--   0 andre     (1000) andre     (1000)      830 2021-10-05 15:04:26.000000 mice-0.1.9/docs/build/html/objects.inv
+-rw-rw-r--   0 andre     (1000) andre     (1000)     3869 2021-10-05 15:04:26.000000 mice-0.1.9/docs/build/html/search.html
+-rw-rw-r--   0 andre     (1000) andre     (1000)     8642 2021-10-05 15:04:26.000000 mice-0.1.9/docs/build/html/searchindex.js
+-rw-rw-r--   0 andre     (1000) andre     (1000)      804 2021-09-30 15:24:08.000000 mice-0.1.9/docs/make.bat
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:29:35.292666 mice-0.1.9/docs/source/
+-rw-rw-r--   0 andre     (1000) andre     (1000)     2018 2021-10-06 13:29:04.000000 mice-0.1.9/docs/source/conf.py
+-rw-rw-r--   0 andre     (1000) andre     (1000)      568 2021-10-04 14:04:38.000000 mice-0.1.9/docs/source/index.rst
+-rw-rw-r--   0 andre     (1000) andre     (1000)      660 2021-09-30 15:24:08.000000 mice-0.1.9/docs/source/intro.rst
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:29:35.292666 mice-0.1.9/mice/
+-rw-rw-r--   0 andre     (1000) andre     (1000)       92 2021-10-05 06:44:01.000000 mice-0.1.9/mice/__init__.py
+-rw-rw-r--   0 andre     (1000) andre     (1000)    20891 2021-10-05 06:37:18.000000 mice-0.1.9/mice/deltas.py
+-rw-rw-r--   0 andre     (1000) andre     (1000)    25752 2021-10-06 12:48:29.000000 mice-0.1.9/mice/mice.py
+-rw-rw-r--   0 andre     (1000) andre     (1000)     3504 2021-10-05 11:35:52.000000 mice-0.1.9/mice/plot_mice.py
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2021-10-06 13:29:35.292666 mice-0.1.9/mice.egg-info/
+-rw-rw-r--   0 andre     (1000) andre     (1000)     1890 2021-10-06 13:29:34.000000 mice-0.1.9/mice.egg-info/PKG-INFO
+-rw-rw-r--   0 andre     (1000) andre     (1000)     1237 2021-10-06 13:29:34.000000 mice-0.1.9/mice.egg-info/SOURCES.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)        1 2021-10-06 13:29:34.000000 mice-0.1.9/mice.egg-info/dependency_links.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)       42 2021-10-06 13:29:34.000000 mice-0.1.9/mice.egg-info/requires.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)        5 2021-10-06 13:29:34.000000 mice-0.1.9/mice.egg-info/top_level.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)      185 2021-10-05 14:17:04.000000 mice-0.1.9/pyproject.toml
+-rw-rw-r--   0 andre     (1000) andre     (1000)       38 2021-10-06 13:29:35.292666 mice-0.1.9/setup.cfg
+-rw-rw-r--   0 andre     (1000) andre     (1000)      769 2021-10-06 13:29:07.000000 mice-0.1.9/setup.py
```

### Comparing `mice-0.1.8/LICENSE` & `mice-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/PKG-INFO` & `mice-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mice
-Version: 0.1.8
+Version: 0.1.9
 Summary: Multi-iteration Stochastic Estimator
 Home-page: https://bitbucket.org/agcarlon/mice
 Author: Andre Gustavo Carlon
 Author-email: agcarlon@gmail.com
 License: GPL v3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -48,10 +48,10 @@
     >>> x = 10
     >>> for i in range(10):
     ...    grad = df(x)
     ...    x = x - grad
 
 
 However, it is flexible enough to tackle more complex problems.
-For more information on how to use MICE and examples, check the `documentation <https://mice.readthedocs.io>`_.
+For more information on how to use MICE and examples, check the `documentation <https://mice.readthedocs.io/>`_.
```

### Comparing `mice-0.1.8/README.rst` & `mice-0.1.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -36,8 +36,8 @@
     >>> x = 10
     >>> for i in range(10):
     ...    grad = df(x)
     ...    x = x - grad
 
 
 However, it is flexible enough to tackle more complex problems.
-For more information on how to use MICE and examples, check the `documentation <https://mice.readthedocs.io>`_.
+For more information on how to use MICE and examples, check the `documentation <https://mice.readthedocs.io/>`_.
```

### Comparing `mice-0.1.8/docs/Makefile` & `mice-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/doctrees/environment.pickle` & `mice-0.1.9/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/doctrees/index.doctree` & `mice-0.1.9/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/doctrees/intro.doctree` & `mice-0.1.9/docs/build/doctrees/intro.doctree`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/_sources/index.rst.txt` & `mice-0.1.9/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/_sources/intro.rst.txt` & `mice-0.1.9/docs/build/html/_sources/intro.rst.txt`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/_static/basic.css` & `mice-0.1.9/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/_static/doctools.js` & `mice-0.1.9/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/_static/jquery-3.5.1.js` & `mice-0.1.9/docs/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/_static/jquery.js` & `mice-0.1.9/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/_static/language_data.js` & `mice-0.1.9/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/_static/pygments.css` & `mice-0.1.9/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/_static/searchtools.js` & `mice-0.1.9/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/_static/underscore-1.13.1.js` & `mice-0.1.9/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/_static/underscore.js` & `mice-0.1.9/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/genindex.html` & `mice-0.1.9/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/index.html` & `mice-0.1.9/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/intro.html` & `mice-0.1.9/docs/build/html/intro.html`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/objects.inv` & `mice-0.1.9/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/search.html` & `mice-0.1.9/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/build/html/searchindex.js` & `mice-0.1.9/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/make.bat` & `mice-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/source/conf.py` & `mice-0.1.9/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 project = 'MICE'
 copyright = '2021, Andre G. Carlon'
 author = 'Andre G. Carlon'
 
 # The full version, including alpha/beta/rc tags
-release = '0.1.8'
+release = '0.1.9'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `mice-0.1.8/docs/source/index.rst` & `mice-0.1.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/docs/source/intro.rst` & `mice-0.1.9/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/mice/deltas.py` & `mice-0.1.9/mice/deltas.py`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/mice/mice.py` & `mice-0.1.9/mice/mice.py`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/mice/plot_mice.py` & `mice-0.1.9/mice/plot_mice.py`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/mice.egg-info/PKG-INFO` & `mice-0.1.9/mice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mice
-Version: 0.1.8
+Version: 0.1.9
 Summary: Multi-iteration Stochastic Estimator
 Home-page: https://bitbucket.org/agcarlon/mice
 Author: Andre Gustavo Carlon
 Author-email: agcarlon@gmail.com
 License: GPL v3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -48,10 +48,10 @@
     >>> x = 10
     >>> for i in range(10):
     ...    grad = df(x)
     ...    x = x - grad
 
 
 However, it is flexible enough to tackle more complex problems.
-For more information on how to use MICE and examples, check the `documentation <https://mice.readthedocs.io>`_.
+For more information on how to use MICE and examples, check the `documentation <https://mice.readthedocs.io/>`_.
```

### Comparing `mice-0.1.8/mice.egg-info/SOURCES.txt` & `mice-0.1.9/mice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mice-0.1.8/setup.py` & `mice-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open('REQUIREMENTS') as f:
     requirements = f.read()
 
 
 setup(
     name='mice',
-    version='0.1.8',
+    version='0.1.9',
     description='Multi-iteration Stochastic Estimator',
     long_description_content_type="text/markdown",
     long_description=readme,
     author='Andre Gustavo Carlon',
     author_email='agcarlon@gmail.com',
     url='https://bitbucket.org/agcarlon/mice',
     license='GPL v3',
```

