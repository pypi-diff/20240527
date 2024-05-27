# Comparing `tmp/whispertrades-0.1.0.tar.gz` & `tmp/whispertrades-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whispertrades-0.1.0.tar", last modified: Mon Apr 29 15:07:59 2024, max compression
+gzip compressed data, was "whispertrades-0.1.1.tar", last modified: Mon May 27 02:49:07 2024, max compression
```

## Comparing `whispertrades-0.1.0.tar` & `whispertrades-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:59.224859 whispertrades-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-29 15:07:50.000000 whispertrades-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-29 15:07:59.224859 whispertrades-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-29 15:07:50.000000 whispertrades-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:07:59.224859 whispertrades-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-29 15:07:50.000000 whispertrades-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:59.224859 whispertrades-0.1.0/whispertrades.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-29 15:07:59.000000 whispertrades-0.1.0/whispertrades.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-29 15:07:59.000000 whispertrades-0.1.0/whispertrades.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:07:59.000000 whispertrades-0.1.0/whispertrades.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 15:07:59.000000 whispertrades-0.1.0/whispertrades.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:07:59.000000 whispertrades-0.1.0/whispertrades.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:49:07.715279 whispertrades-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-27 02:49:03.000000 whispertrades-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-27 02:49:07.715279 whispertrades-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-27 02:49:03.000000 whispertrades-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 02:49:07.715279 whispertrades-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-27 02:49:03.000000 whispertrades-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:49:07.715279 whispertrades-0.1.1/whispertrades.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-27 02:49:07.000000 whispertrades-0.1.1/whispertrades.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-27 02:49:07.000000 whispertrades-0.1.1/whispertrades.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 02:49:07.000000 whispertrades-0.1.1/whispertrades.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-27 02:49:07.000000 whispertrades-0.1.1/whispertrades.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 02:49:07.000000 whispertrades-0.1.1/whispertrades.egg-info/top_level.txt
```

### Comparing `whispertrades-0.1.0/LICENSE` & `whispertrades-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whispertrades-0.1.0/PKG-INFO` & `whispertrades-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: whispertrades
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for Whispertrades API
 Home-page: https://github.com/aliencaocao/whispertrades
 Author: Billy Cao
 Author-email: aliencaocao@gmail.com
 Maintainer: Billy Cao
 Maintainer-email: aliencaocao@gmail.com
 License: Apache 2.0
+Project-URL: Documentation, https://whispertrades.readthedocs.io/
+Project-URL: Issues, https://github.com/aliencaocao/whispertrades/issues
+Project-URL: Releases, https://github.com/aliencaocao/whispertrades/releases
+Project-URL: Source Code, https://github.com/aliencaocao/whispertrades
 Keywords: whispertrades api python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `whispertrades-0.1.0/README.md` & `whispertrades-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Whispertrades API Python Wrapper
+[![PyPI version](https://badge.fury.io/py/whispertrades.svg)](https://badge.fury.io/py/whispertrades)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whispertrades)](https://pypi.org/project/whispertrades/)
+[![PyPI - Downloads](https://static.pepy.tech/personalized-badge/whispertrades?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pypi.org/project/whispertrades/)
 [![Documentation Status](https://readthedocs.org/projects/whispertrades/badge/?style=flat-square)](https://whispertrades.readthedocs.io/)
 
 ## About
 [Whispertrades](https://whispertrades.com/) is an advanced automated options trading and backtesting platform. This is an **unofficial** Python wrapper for its [API](https://docs.whispertrades.com/i1-R-overview). It builds on `Pydantic` for strong typing support to ease development, and `requests` library for HTTP requests.
 
 ## Installation
-### Using pip (To be uploaded)
+### Using pip
 ```bash
 pip install whispertrades
 ```
 ### From source (for latest features and development)
 ```bash
 pip install git+https://github.com/aliencaocao/whispertrades
 ```
@@ -66,8 +69,8 @@
 
 http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
-limitations under the License.
+limitations under the License.
```

### Comparing `whispertrades-0.1.0/setup.py` & `whispertrades-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='whispertrades',
-    version='0.1.0',
+    version='0.1.1',
     description='A Python package for Whispertrades API',
     long_description='A python package for Whispertrades API. Built on pydantic and requests. Requires Python 3.8+.',
     author='Billy Cao',
     author_email='aliencaocao@gmail.com',
     maintainer='Billy Cao',
     maintainer_email='aliencaocao@gmail.com',
     url='https://github.com/aliencaocao/whispertrades',
@@ -27,10 +27,16 @@
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Intended Audience :: Developers',
         'Intended Audience :: Financial and Insurance Industry',
         'Topic :: Office/Business :: Financial :: Investment',
         'Topic :: Software Development :: Libraries :: Application Frameworks'
     ],
+    project_urls={
+        "Documentation": "https://whispertrades.readthedocs.io/",
+        "Issues": "https://github.com/aliencaocao/whispertrades/issues",
+        "Releases": "https://github.com/aliencaocao/whispertrades/releases",
+        "Source Code": "https://github.com/aliencaocao/whispertrades",
+    },
     license='Apache 2.0',
     keywords='whispertrades api python'
 )
```

### Comparing `whispertrades-0.1.0/whispertrades.egg-info/PKG-INFO` & `whispertrades-0.1.1/whispertrades.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: whispertrades
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for Whispertrades API
 Home-page: https://github.com/aliencaocao/whispertrades
 Author: Billy Cao
 Author-email: aliencaocao@gmail.com
 Maintainer: Billy Cao
 Maintainer-email: aliencaocao@gmail.com
 License: Apache 2.0
+Project-URL: Documentation, https://whispertrades.readthedocs.io/
+Project-URL: Issues, https://github.com/aliencaocao/whispertrades/issues
+Project-URL: Releases, https://github.com/aliencaocao/whispertrades/releases
+Project-URL: Source Code, https://github.com/aliencaocao/whispertrades
 Keywords: whispertrades api python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

