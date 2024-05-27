# Comparing `tmp/pyosintleak-1.0.1.tar.gz` & `tmp/pyosintleak-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyosintleak-1.0.1.tar", last modified: Fri Apr 19 14:22:56 2024, max compression
+gzip compressed data, was "pyosintleak-1.0.2.tar", last modified: Mon May 27 17:54:31 2024, max compression
```

## Comparing `pyosintleak-1.0.1.tar` & `pyosintleak-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 14:22:56.929045 pyosintleak-1.0.1/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2907 2024-04-19 14:22:56.927546 pyosintleak-1.0.1/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2139 2024-04-17 19:14:55.000000 pyosintleak-1.0.1/README.md
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 14:22:56.805141 pyosintleak-1.0.1/pyosintleak/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3441 2024-04-19 14:17:53.000000 pyosintleak-1.0.1/pyosintleak/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 14:22:56.896963 pyosintleak-1.0.1/pyosintleak/cli/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7478 2024-04-19 14:17:30.000000 pyosintleak-1.0.1/pyosintleak/cli/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 14:22:56.922484 pyosintleak-1.0.1/pyosintleak.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2907 2024-04-19 14:22:56.000000 pyosintleak-1.0.1/pyosintleak.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      340 2024-04-19 14:22:56.000000 pyosintleak-1.0.1/pyosintleak.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-19 14:22:56.000000 pyosintleak-1.0.1/pyosintleak.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       51 2024-04-19 14:22:56.000000 pyosintleak-1.0.1/pyosintleak.egg-info/entry_points.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-17 19:11:11.000000 pyosintleak-1.0.1/pyosintleak.egg-info/not-zip-safe
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       18 2024-04-19 14:22:56.000000 pyosintleak-1.0.1/pyosintleak.egg-info/requires.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       12 2024-04-19 14:22:56.000000 pyosintleak-1.0.1/pyosintleak.egg-info/top_level.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      289 2024-04-19 14:22:56.933053 pyosintleak-1.0.1/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1522 2024-04-19 14:17:46.000000 pyosintleak-1.0.1/setup.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 14:22:56.908968 pyosintleak-1.0.1/tests/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      230 2024-04-17 19:12:55.000000 pyosintleak-1.0.1/tests/test.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 17:54:31.114315 pyosintleak-1.0.2/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3011 2024-05-27 17:54:31.111316 pyosintleak-1.0.2/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2246 2024-05-27 17:51:39.000000 pyosintleak-1.0.2/README.md
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 17:54:30.933565 pyosintleak-1.0.2/pyosintleak/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3534 2024-05-27 13:36:34.000000 pyosintleak-1.0.2/pyosintleak/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 17:54:31.049545 pyosintleak-1.0.2/pyosintleak/cli/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7478 2024-05-27 13:36:24.000000 pyosintleak-1.0.2/pyosintleak/cli/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       47 2024-05-27 17:42:22.000000 pyosintleak-1.0.2/pyosintleak/config.json
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 17:54:31.073545 pyosintleak-1.0.2/pyosintleak.egg-info/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3011 2024-05-27 17:54:30.000000 pyosintleak-1.0.2/pyosintleak.egg-info/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      364 2024-05-27 17:54:30.000000 pyosintleak-1.0.2/pyosintleak.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-27 17:54:30.000000 pyosintleak-1.0.2/pyosintleak.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       51 2024-05-27 17:54:30.000000 pyosintleak-1.0.2/pyosintleak.egg-info/entry_points.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-17 19:11:11.000000 pyosintleak-1.0.2/pyosintleak.egg-info/not-zip-safe
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-27 17:54:30.000000 pyosintleak-1.0.2/pyosintleak.egg-info/requires.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       12 2024-05-27 17:54:30.000000 pyosintleak-1.0.2/pyosintleak.egg-info/top_level.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      289 2024-05-27 17:54:31.117815 pyosintleak-1.0.2/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1522 2024-05-27 13:36:47.000000 pyosintleak-1.0.2/setup.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 17:54:31.060546 pyosintleak-1.0.2/tests/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      230 2024-04-17 19:12:55.000000 pyosintleak-1.0.2/tests/test.py
```

### Comparing `pyosintleak-1.0.1/PKG-INFO` & `pyosintleak-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyosintleak
-Version: 1.0.1
+Version: 1.0.2
 Summary: pyosintleak is a library designed for utilizing the osintleak API, facilitating integration and automation of open-source intelligence operations.
 Home-page: https://github.com/osintleak/pyosintleak
-Download-URL: https://github.com/osintleak/pyosintleak/archive/v1.0.1.zip
+Download-URL: https://github.com/osintleak/pyosintleak/archive/v1.0.2.zip
 Author: OsintLeak
 Author-email: help@osintleak.com
 Keywords: osintleak,osint,leak,breach,search,ol,pentesting
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: colorama
 
 # pyosintleak
+![image](https://github.com/OsintLeak/pyosintleak/assets/28790962/c24e8b19-545e-4e05-b682-d6fc3b8b41cb)
 
 pyosintleak is a Python library designed to leverage the capabilities of the osintleak API, streamlining the integration and automation of open-source intelligence (OSINT) operations.
 
 ## Installation
 
 You can install pyosintleak using pip:
```

### Comparing `pyosintleak-1.0.1/README.md` & `pyosintleak-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # pyosintleak
+![image](https://github.com/OsintLeak/pyosintleak/assets/28790962/c24e8b19-545e-4e05-b682-d6fc3b8b41cb)
 
 pyosintleak is a Python library designed to leverage the capabilities of the osintleak API, streamlining the integration and automation of open-source intelligence (OSINT) operations.
 
 ## Installation
 
 You can install pyosintleak using pip:
 
@@ -65,8 +66,8 @@
 
 ```bash
 osintleak --help
 ```
 
 ## Contributing
 
-If you encounter any issues or have suggestions for improvements, please feel free to contribute by opening an issue or submitting a pull request on [GitHub](https://github.com/osintleak/pyosintleak). Your feedback is highly appreciated!
+If you encounter any issues or have suggestions for improvements, please feel free to contribute by opening an issue or submitting a pull request on [GitHub](https://github.com/osintleak/pyosintleak). Your feedback is highly appreciated!
```

### Comparing `pyosintleak-1.0.1/pyosintleak/__init__.py` & `pyosintleak-1.0.2/pyosintleak/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 class osintleak:
     BASE_URL = "https://osintleak.com/api/v1"
     API_KEY = None
     HEADERS = None
     USER_AGENT = f"OL-Python/{__version__}"
     AVAILABLE_SEARCH_TYPES = ['name', 'first_name', 'last_name', 'email', 'username', 'password', 'logname', 'phone', 'idcard', 'cc_holder', 'cc_number', 'ftp', 'ip', 'url']
@@ -12,15 +12,15 @@
 
     def __init__(self, key):
         self.API_KEY = key
         self.HEADERS = {
             "User-Agent": self.USER_AGENT
         }
 
-    def search(self, query, type, datasets=DATASETS, similar_search=False, from_date=None, to_date=None, page=1, page_size=20, meta='true'):
+    def search(self, query, type, datasets=DATASETS, similar_search=False, from_date=None, to_date=None, page=1, page_size=20, country=None, sort=None, meta='true'):
         if type not in self.AVAILABLE_SEARCH_TYPES:
             return {"status": "error", "message": f"Invalid search type. Available types are: {', '.join(self.AVAILABLE_SEARCH_TYPES)}"}
         
         stealerlogs = 'false'
         dbleaks = 'false'
         dbleaks2 = 'false'
         if "SL" in datasets:
@@ -45,16 +45,18 @@
                 "stealerlogs": stealerlogs,
                 "dbleaks": dbleaks,
                 "dbleaks2": dbleaks2,
                 "quick_search": quick_search,
                 "similar_search": similar_search,
                 "from_date": from_date,
                 "to_date": to_date,
+                "country": country,
                 "page": page,
                 "page_size": page_size,
+                "sort": sort,
                 "meta": meta
             }
             rep = requests.get(f"{self.BASE_URL}/search_api/", headers=self.HEADERS, params=PARAMS)
             if rep.status_code == 200:
                 return rep.json()
             elif rep.status_code == 404:
                 return {"status": "error", "message": "Result not found"}
```

### Comparing `pyosintleak-1.0.1/pyosintleak/cli/__init__.py` & `pyosintleak-1.0.2/pyosintleak/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyosintleak-1.0.1/pyosintleak.egg-info/PKG-INFO` & `pyosintleak-1.0.2/pyosintleak.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyosintleak
-Version: 1.0.1
+Version: 1.0.2
 Summary: pyosintleak is a library designed for utilizing the osintleak API, facilitating integration and automation of open-source intelligence operations.
 Home-page: https://github.com/osintleak/pyosintleak
-Download-URL: https://github.com/osintleak/pyosintleak/archive/v1.0.1.zip
+Download-URL: https://github.com/osintleak/pyosintleak/archive/v1.0.2.zip
 Author: OsintLeak
 Author-email: help@osintleak.com
 Keywords: osintleak,osint,leak,breach,search,ol,pentesting
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: colorama
 
 # pyosintleak
+![image](https://github.com/OsintLeak/pyosintleak/assets/28790962/c24e8b19-545e-4e05-b682-d6fc3b8b41cb)
 
 pyosintleak is a Python library designed to leverage the capabilities of the osintleak API, streamlining the integration and automation of open-source intelligence (OSINT) operations.
 
 ## Installation
 
 You can install pyosintleak using pip:
```

### Comparing `pyosintleak-1.0.1/setup.py` & `pyosintleak-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with io.open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     desc = f.read()
 
-ol_version = '1.0.1'
+ol_version = '1.0.2'
 
 setup(
     name='pyosintleak',
     version=ol_version,
     description='pyosintleak is a library designed for utilizing the osintleak API, facilitating integration and automation of open-source intelligence operations.',
     long_description=desc,
     long_description_content_type='text/markdown',
```

