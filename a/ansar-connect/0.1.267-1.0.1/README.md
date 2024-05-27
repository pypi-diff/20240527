# Comparing `tmp/ansar_connect-0.1.267.tar.gz` & `tmp/ansar_connect-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.267.tar", last modified: Sun May 26 20:21:59 2024, max compression
+gzip compressed data, was "ansar_connect-1.0.1.tar", last modified: Mon May 27 05:41:25 2024, max compression
```

## Comparing `ansar_connect-0.1.267.tar` & `ansar_connect-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.267/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/PKG-INFO
--rwxrwxr-x   0 scott     (1000) scott     (1000)      577 2024-05-23 01:07:25.000000 ansar_connect-0.1.267/README.md
--rwxrwxr-x   0 scott     (1000) scott     (1000)      764 2024-05-26 07:28:48.000000 ansar_connect-0.1.267/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/setup.cfg
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2251 2024-05-26 07:28:40.000000 ansar_connect-0.1.267/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.267/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.267/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9946 2024-05-26 20:11:05.000000 ansar_connect-0.1.267/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.267/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-26 20:21:56.000000 ansar_connect-0.1.267/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14103 2024-05-26 20:11:05.000000 ansar_connect-0.1.267/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-0.1.267/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.267/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.267/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.267/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    15870 2024-05-26 20:11:05.000000 ansar_connect-0.1.267/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.267/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    23196 2024-05-26 20:11:05.000000 ansar_connect-0.1.267/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.267/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9679 2024-05-26 07:36:57.000000 ansar_connect-0.1.267/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.267/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.267/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.267/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    42336 2024-05-26 07:25:14.000000 ansar_connect-0.1.267/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.267/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.267/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.267/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.267/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-26 20:21:59.000000 ansar_connect-0.1.267/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-26 20:21:59.000000 ansar_connect-0.1.267/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-26 20:21:59.000000 ansar_connect-0.1.267/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-26 20:21:59.000000 ansar_connect-0.1.267/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-26 20:21:59.000000 ansar_connect-0.1.267/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-26 20:21:59.000000 ansar_connect-0.1.267/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-27 05:41:25.390176 ansar_connect-1.0.1/
+-rw-rw-r--   0 scott     (1000) scott     (1000)      271 2024-05-27 03:58:46.000000 ansar_connect-1.0.1/CHANGES.rst
+-rw-rw-r--   0 scott     (1000) scott     (1000)       32 2024-05-27 02:47:17.000000 ansar_connect-1.0.1/COPYRIGHT.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-1.0.1/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)      224 2024-05-27 02:47:17.000000 ansar_connect-1.0.1/MANIFEST.in
+-rw-r--r--   0 scott     (1000) scott     (1000)     2408 2024-05-27 05:41:25.390176 ansar_connect-1.0.1/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      854 2024-05-27 03:59:46.000000 ansar_connect-1.0.1/README.rst
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     1430 2024-05-27 04:14:18.000000 ansar_connect-1.0.1/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-27 05:41:25.390176 ansar_connect-1.0.1/setup.cfg
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2617 2024-05-27 04:59:38.000000 ansar_connect-1.0.1/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-27 05:41:25.390176 ansar_connect-1.0.1/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-27 05:41:25.390176 ansar_connect-1.0.1/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-27 05:41:25.390176 ansar_connect-1.0.1/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-1.0.1/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-1.0.1/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9946 2024-05-26 20:11:05.000000 ansar_connect-1.0.1/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-1.0.1/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-27 05:41:25.390176 ansar_connect-1.0.1/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3003 2024-05-27 05:41:22.000000 ansar_connect-1.0.1/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14103 2024-05-26 20:11:05.000000 ansar_connect-1.0.1/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-1.0.1/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-1.0.1/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-1.0.1/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-1.0.1/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    15870 2024-05-26 20:11:05.000000 ansar_connect-1.0.1/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-1.0.1/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    23196 2024-05-26 20:11:05.000000 ansar_connect-1.0.1/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-1.0.1/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9679 2024-05-26 07:36:57.000000 ansar_connect-1.0.1/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-1.0.1/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-1.0.1/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-1.0.1/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    42336 2024-05-26 07:25:14.000000 ansar_connect-1.0.1/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-1.0.1/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-1.0.1/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-1.0.1/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-1.0.1/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-27 05:41:25.390176 ansar_connect-1.0.1/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2408 2024-05-27 05:41:25.000000 ansar_connect-1.0.1/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1060 2024-05-27 05:41:25.000000 ansar_connect-1.0.1/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-27 05:41:25.000000 ansar_connect-1.0.1/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-27 05:41:25.000000 ansar_connect-1.0.1/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-27 05:41:25.000000 ansar_connect-1.0.1/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-27 05:41:25.000000 ansar_connect-1.0.1/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.267/LICENSE` & `ansar_connect-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/setup.py` & `ansar_connect-1.0.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,81 @@
 # Standard PyPi packaging.
 # Build materials and push to pypi.org.
 # Author: Scott Woods <scott.18.ansar@gmail.com.com>
 import sys
+import os
 import setuptools
 import re
 
+here = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(here, 'README.rst')) as f:
+    README = f.read()
+
 #
 #
 VERSION_PATTERN = re.compile(r'([0-9]+)\.([0-9]+)\.([0-9]+)')
 
 #
 #
-with open("PACKAGE", "r", encoding="utf-8") as f:
+with open(os.path.join(here, 'PACKAGE')) as f:
     p = f.read()
 PACKAGE = p[:-1]
 
 #
 #
-with open("DESCRIPTION", "r", encoding="utf-8") as f:
+with open(os.path.join(here, 'DESCRIPTION')) as f:
     d = f.read()
 DESCRIPTION = d[:-1]
 
 #
 #
-with open("VERSION", "r", encoding="utf-8") as f:
+with open(os.path.join(here, 'VERSION')) as f:
     line = [t for t in f]
 VERSION = line[-1][:-1]
 
 if not VERSION_PATTERN.match(VERSION):
     print('Version "%s" does not meet semantic requirements' % (VERSION,))
     sys.exit(1)
 
-with open("README.md", "r", encoding="utf-8") as f:
-    long_description = f.read()
-
 with open("DOC_LATEST_LINK", "r", encoding="utf-8") as f:
     d = f.read()
 DOC_LINK = d[:-1]
 
 REQUIRES = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
     "ansar-create>=0.1.98",
 ]
 
 setuptools.setup(
     name=PACKAGE,
     version=VERSION,
     author="Scott Woods",
-    author_email="scott.18.ansar@gmail.com.com",
+    author_email="ansar.library.management@gmail.com",
     description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description=README,
+    #long_description_content_type="text/markdown",
     #project_urls={
     #    "Documentation": DOC_LINK,
     #},
-    #classifiers=[
-    #    "Development Status :: 4 - Beta",
-    #    "Intended Audience :: Developers",
-    #    "Programming Language :: Python :: 3",
-    #    "License :: OSI Approved :: MIT License",
-    #    "Operating System :: OS Independent",
-    #    "Topic :: Software Development :: Libraries",
-    #],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: Linux",
+        "Operating System :: macOS",
+        "Topic :: Software Development :: Libraries",
+    ],
     # Where multiple packages might be found, esp if using standard
     # layout for "find_packages".
     package_dir={
         "": "src",
     },
     # First folder under "where" defines the name of the
     # namespace. Folders under that (with __init__.py files)
```

### Comparing `ansar_connect-0.1.267/src/ansar/command/ansar_command.py` & `ansar_connect-1.0.1/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/command/ansar_directory.py` & `ansar_connect-1.0.1/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/command/ansar_group.py` & `ansar_connect-1.0.1/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/command/shared_directory.py` & `ansar_connect-1.0.1/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/__init__.py` & `ansar_connect-1.0.1/src/ansar/connect/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-"""Tools and runtime for asynchronous programming.
+"""Tools and runtime for network messaging.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: bb665d21b8f0dbd57df14a1b012560fbd544a2f4
-Version: 0.1.266 (2024-05-27@08:21:56+NZST)
+Commit: ef95e1d78a16b38211c4d6386fc0571e34d12dff
+Version: 1.0.0 (2024-05-27@17:41:22+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.267/src/ansar/connect/connect_directory.py` & `ansar_connect-1.0.1/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/directory.py` & `ansar_connect-1.0.1/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/directory_if.py` & `ansar_connect-1.0.1/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/foh_if.py` & `ansar_connect-1.0.1/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/group_if.py` & `ansar_connect-1.0.1/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/grouping.py` & `ansar_connect-1.0.1/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/moving.py` & `ansar_connect-1.0.1/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/networking.py` & `ansar_connect-1.0.1/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/networking_if.py` & `ansar_connect-1.0.1/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/node.py` & `ansar_connect-1.0.1/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/plumbing.py` & `ansar_connect-1.0.1/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/procedure.py` & `ansar_connect-1.0.1/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/product.py` & `ansar_connect-1.0.1/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/socketry.py` & `ansar_connect-1.0.1/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/standard.py` & `ansar_connect-1.0.1/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/transporting.py` & `ansar_connect-1.0.1/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/transporting_if.py` & `ansar_connect-1.0.1/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar/connect/wan.py` & `ansar_connect-1.0.1/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.267/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-1.0.1/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+CHANGES.rst
+COPYRIGHT.txt
 LICENSE
-README.md
+MANIFEST.in
+README.rst
 pyproject.toml
 setup.py
 src/ansar/command/ansar_command.py
 src/ansar/command/ansar_directory.py
 src/ansar/command/ansar_group.py
 src/ansar/command/shared_directory.py
 src/ansar/connect/__init__.py
```

