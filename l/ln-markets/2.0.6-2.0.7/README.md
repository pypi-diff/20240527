# Comparing `tmp/ln_markets-2.0.6.tar.gz` & `tmp/ln_markets-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ln_markets-2.0.6.tar", last modified: Tue May  7 16:29:45 2024, max compression
+gzip compressed data, was "ln_markets-2.0.7.tar", last modified: Mon May 27 10:56:27 2024, max compression
```

## Comparing `ln_markets-2.0.6.tar` & `ln_markets-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-05-07 16:29:45.937348 ln_markets-2.0.6/
--rw-r--r--   0 romain     (501) staff       (20)     1067 2023-12-19 14:58:01.000000 ln_markets-2.0.6/LICENSE
--rw-r--r--   0 romain     (501) staff       (20)    14919 2024-05-07 16:29:45.937222 ln_markets-2.0.6/PKG-INFO
--rw-r--r--   0 romain     (501) staff       (20)    14026 2024-05-07 16:29:24.000000 ln_markets-2.0.6/README.md
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-05-07 16:29:45.936995 ln_markets-2.0.6/ln_markets.egg-info/
--rw-r--r--   0 romain     (501) staff       (20)    14919 2024-05-07 16:29:45.000000 ln_markets-2.0.6/ln_markets.egg-info/PKG-INFO
--rw-r--r--   0 romain     (501) staff       (20)      309 2024-05-07 16:29:45.000000 ln_markets-2.0.6/ln_markets.egg-info/SOURCES.txt
--rw-r--r--   0 romain     (501) staff       (20)        1 2024-05-07 16:29:45.000000 ln_markets-2.0.6/ln_markets.egg-info/dependency_links.txt
--rw-r--r--   0 romain     (501) staff       (20)       26 2024-05-07 16:29:45.000000 ln_markets-2.0.6/ln_markets.egg-info/requires.txt
--rw-r--r--   0 romain     (501) staff       (20)       10 2024-05-07 16:29:45.000000 ln_markets-2.0.6/ln_markets.egg-info/top_level.txt
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-05-07 16:29:45.936687 ln_markets-2.0.6/lnmarkets/
--rw-r--r--   0 romain     (501) staff       (20)        1 2023-12-19 14:58:01.000000 ln_markets-2.0.6/lnmarkets/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)    13721 2024-05-07 16:29:24.000000 ln_markets-2.0.6/lnmarkets/rest.py
--rw-r--r--   0 romain     (501) staff       (20)     2359 2023-12-19 14:58:01.000000 ln_markets-2.0.6/lnmarkets/websockets.py
--rw-r--r--   0 romain     (501) staff       (20)      104 2023-12-19 14:58:01.000000 ln_markets-2.0.6/pyproject.toml
--rw-r--r--   0 romain     (501) staff       (20)       89 2024-05-07 16:29:45.937525 ln_markets-2.0.6/setup.cfg
--rw-r--r--   0 romain     (501) staff       (20)     1192 2024-05-07 16:29:24.000000 ln_markets-2.0.6/setup.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-05-07 16:29:45.936812 ln_markets-2.0.6/tests/
--rw-r--r--   0 romain     (501) staff       (20)        1 2023-12-19 14:58:01.000000 ln_markets-2.0.6/tests/test_node_state.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-05-27 10:56:27.386669 ln_markets-2.0.7/
+-rw-r--r--   0 romain     (501) staff       (20)     1067 2023-12-19 14:58:01.000000 ln_markets-2.0.7/LICENSE
+-rw-r--r--   0 romain     (501) staff       (20)    14919 2024-05-27 10:56:27.386549 ln_markets-2.0.7/PKG-INFO
+-rw-r--r--   0 romain     (501) staff       (20)    14026 2024-05-07 16:29:24.000000 ln_markets-2.0.7/README.md
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-05-27 10:56:27.386335 ln_markets-2.0.7/ln_markets.egg-info/
+-rw-r--r--   0 romain     (501) staff       (20)    14919 2024-05-27 10:56:27.000000 ln_markets-2.0.7/ln_markets.egg-info/PKG-INFO
+-rw-r--r--   0 romain     (501) staff       (20)      309 2024-05-27 10:56:27.000000 ln_markets-2.0.7/ln_markets.egg-info/SOURCES.txt
+-rw-r--r--   0 romain     (501) staff       (20)        1 2024-05-27 10:56:27.000000 ln_markets-2.0.7/ln_markets.egg-info/dependency_links.txt
+-rw-r--r--   0 romain     (501) staff       (20)       26 2024-05-27 10:56:27.000000 ln_markets-2.0.7/ln_markets.egg-info/requires.txt
+-rw-r--r--   0 romain     (501) staff       (20)       10 2024-05-27 10:56:27.000000 ln_markets-2.0.7/ln_markets.egg-info/top_level.txt
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-05-27 10:56:27.385877 ln_markets-2.0.7/lnmarkets/
+-rw-r--r--   0 romain     (501) staff       (20)        1 2023-12-19 14:58:01.000000 ln_markets-2.0.7/lnmarkets/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)    13924 2024-05-27 10:55:48.000000 ln_markets-2.0.7/lnmarkets/rest.py
+-rw-r--r--   0 romain     (501) staff       (20)     2359 2023-12-19 14:58:01.000000 ln_markets-2.0.7/lnmarkets/websockets.py
+-rw-r--r--   0 romain     (501) staff       (20)      104 2023-12-19 14:58:01.000000 ln_markets-2.0.7/pyproject.toml
+-rw-r--r--   0 romain     (501) staff       (20)       89 2024-05-27 10:56:27.386838 ln_markets-2.0.7/setup.cfg
+-rw-r--r--   0 romain     (501) staff       (20)     1192 2024-05-27 10:55:48.000000 ln_markets-2.0.7/setup.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-05-27 10:56:27.386023 ln_markets-2.0.7/tests/
+-rw-r--r--   0 romain     (501) staff       (20)        1 2023-12-19 14:58:01.000000 ln_markets-2.0.7/tests/test_node_state.py
```

### Comparing `ln_markets-2.0.6/LICENSE` & `ln_markets-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ln_markets-2.0.6/PKG-INFO` & `ln_markets-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ln-markets
-Version: 2.0.6
+Version: 2.0.7
 Summary: LN Markets API python implementation
 Home-page: https://github.com/ln-markets/api-python
 Author: Romain ROUPHAEL
 License: MIT
 Keywords: lnmarkets trading rest api bitcoin lightning network futures options
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ln_markets-2.0.6/README.md` & `ln_markets-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ln_markets-2.0.6/ln_markets.egg-info/PKG-INFO` & `ln_markets-2.0.7/ln_markets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ln-markets
-Version: 2.0.6
+Version: 2.0.7
 Summary: LN Markets API python implementation
 Home-page: https://github.com/ln-markets/api-python
 Author: Romain ROUPHAEL
 License: MIT
 Keywords: lnmarkets trading rest api bitcoin lightning network futures options
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ln_markets-2.0.6/lnmarkets/rest.py` & `ln_markets-2.0.7/lnmarkets/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,14 +396,21 @@
     
     def new_withdraw(self, params):
         method = 'POST'
         path = '/user/withdraw'
         credentials = True
 
         return self.before_request_api(method, path, params, credentials)
+
+    def new_withdraw_usd(self, params):
+        method = 'POST'
+        path = '/user/withdraw/usd'
+        credentials = True
+
+        return self.before_request_api(method, path, params, credentials)
     
     def new_internal_transfer(self, params):
         method = 'POST'
         path = '/user/transfer'
         credentials = True
 
         return self.before_request_api(method, path, params, credentials)
```

### Comparing `ln_markets-2.0.6/lnmarkets/websockets.py` & `ln_markets-2.0.7/lnmarkets/websockets.py`

 * *Files identical despite different names*

### Comparing `ln_markets-2.0.6/setup.py` & `ln_markets-2.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ln-markets',
-    version='2.0.6',
+    version='2.0.7',
     packages=['lnmarkets'],
     description='LN Markets API python implementation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ln-markets/api-python',
     author='Romain ROUPHAEL',
     license='MIT',
```

