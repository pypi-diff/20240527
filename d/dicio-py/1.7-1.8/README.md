# Comparing `tmp/dicio_py-1.7.tar.gz` & `tmp/dicio_py-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicio_py-1.7.tar", last modified: Mon May 27 13:32:53 2024, max compression
+gzip compressed data, was "dicio_py-1.8.tar", last modified: Mon May 27 13:44:56 2024, max compression
```

## Comparing `dicio_py-1.7.tar` & `dicio_py-1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 13:32:53.438630 dicio_py-1.7/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-1.7/LICENSE
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 13:32:53.438630 dicio_py-1.7/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-1.7/README.md
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 13:32:53.434630 dicio_py-1.7/dicio_my/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:28:37.000000 dicio_py-1.7/dicio_my/__init__.py
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     3916 2024-05-27 13:32:07.000000 dicio_py-1.7/dicio_my/__main__.py
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 13:32:53.438630 dicio_py-1.7/dicio_py.egg-info/
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 13:32:53.000000 dicio_py-1.7/dicio_py.egg-info/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      196 2024-05-27 13:32:53.000000 dicio_py-1.7/dicio_py.egg-info/SOURCES.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 13:32:53.000000 dicio_py-1.7/dicio_py.egg-info/dependency_links.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        9 2024-05-27 13:32:53.000000 dicio_py-1.7/dicio_py.egg-info/top_level.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 13:32:53.438630 dicio_py-1.7/setup.cfg
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      647 2024-05-27 13:32:23.000000 dicio_py-1.7/setup.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 13:44:56.648593 dicio_py-1.8/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-1.8/LICENSE
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 13:44:56.648593 dicio_py-1.8/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-1.8/README.md
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 13:44:56.644593 dicio_py-1.8/dicio_my/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:28:37.000000 dicio_py-1.8/dicio_my/__init__.py
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     3877 2024-05-27 13:40:43.000000 dicio_py-1.8/dicio_my/__main__.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 13:44:56.648593 dicio_py-1.8/dicio_py.egg-info/
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 13:44:56.000000 dicio_py-1.8/dicio_py.egg-info/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      196 2024-05-27 13:44:56.000000 dicio_py-1.8/dicio_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 13:44:56.000000 dicio_py-1.8/dicio_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        9 2024-05-27 13:44:56.000000 dicio_py-1.8/dicio_py.egg-info/top_level.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 13:44:56.648593 dicio_py-1.8/setup.cfg
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      647 2024-05-27 13:43:18.000000 dicio_py-1.8/setup.py
```

### Comparing `dicio_py-1.7/LICENSE` & `dicio_py-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dicio_py-1.7/PKG-INFO` & `dicio_py-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 1.7
+Version: 1.8
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dicio_py-1.7/README.md` & `dicio_py-1.8/README.md`

 * *Files identical despite different names*

### Comparing `dicio_py-1.7/dicio_my/__main__.py` & `dicio_py-1.8/dicio_my/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,10 +99,7 @@
     print_with_color("A palavra que você pesquisou não foi encontrada", 'RED')
     exit()
 
 HTML = PAGE_WORD.read().decode('utf-8')
 HTML_MEANING = get_content_of_tag(HTML, '<p class="significado textonovo">', '</p>')
 
 print_results()
-
-if __name__ == "__main__":
-    main()
```

### Comparing `dicio_py-1.7/dicio_py.egg-info/PKG-INFO` & `dicio_py-1.8/dicio_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 1.7
+Version: 1.8
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dicio_py-1.7/setup.py` & `dicio_py-1.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dicio-py",
-    version="1.7",
+    version="1.8",
     author="Jetrom17",
     author_email="Jeiel@duck.com",
     description="Dicionário via CLI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Jetrom17/dicio-py",
     packages=setuptools.find_packages(),
```

