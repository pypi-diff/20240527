# Comparing `tmp/pip2deb-2.0.4.tar.gz` & `tmp/pip2deb-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip2deb-2.0.4.tar", last modified: Mon May 27 19:24:14 2024, max compression
+gzip compressed data, was "pip2deb-2.0.5.tar", last modified: Mon May 27 20:46:53 2024, max compression
```

## Comparing `pip2deb-2.0.4.tar` & `pip2deb-2.0.5.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 19:24:14.070098 pip2deb-2.0.4/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-2.0.4/LICENSE
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1417 2024-05-27 19:24:14.070098 pip2deb-2.0.4/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-2.0.4/README.rst
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     4861 2024-05-27 19:17:45.000000 pip2deb-2.0.4/pip2deb
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 19:24:14.070098 pip2deb-2.0.4/pip2deb.egg-info/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1417 2024-05-27 19:24:14.000000 pip2deb-2.0.4/pip2deb.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      159 2024-05-27 19:24:14.000000 pip2deb-2.0.4/pip2deb.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 19:24:14.000000 pip2deb-2.0.4/pip2deb.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 19:24:14.000000 pip2deb-2.0.4/pip2deb.egg-info/top_level.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-27 19:24:14.070098 pip2deb-2.0.4/setup.cfg
--rw-r--r--   0 whoami    (1002) whoami    (1002)      791 2024-05-27 19:23:51.000000 pip2deb-2.0.4/setup.py
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 20:46:53.262330 pip2deb-2.0.5/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-2.0.5/LICENSE
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1417 2024-05-27 20:46:53.262330 pip2deb-2.0.5/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-2.0.5/README.rst
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     4861 2024-05-27 19:17:45.000000 pip2deb-2.0.5/bash-pip2deb
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     4861 2024-05-27 19:17:45.000000 pip2deb-2.0.5/pip2deb-bash
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     4230 2024-05-27 20:44:02.000000 pip2deb-2.0.5/pip2deb-python
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 20:46:53.262330 pip2deb-2.0.5/pip2deb.egg-info/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1417 2024-05-27 20:46:53.000000 pip2deb-2.0.5/pip2deb.egg-info/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      207 2024-05-27 20:46:53.000000 pip2deb-2.0.5/pip2deb.egg-info/SOURCES.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 20:46:53.000000 pip2deb-2.0.5/pip2deb.egg-info/dependency_links.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 20:46:53.000000 pip2deb-2.0.5/pip2deb.egg-info/top_level.txt
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     4230 2024-05-27 20:44:02.000000 pip2deb-2.0.5/python-pip2deb
+-rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-27 20:46:53.262330 pip2deb-2.0.5/setup.cfg
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      848 2024-05-27 20:46:42.000000 pip2deb-2.0.5/setup.py
```

### Comparing `pip2deb-2.0.4/LICENSE` & `pip2deb-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pip2deb-2.0.4/PKG-INFO` & `pip2deb-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 2.0.4
+Version: 2.0.5
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-2.0.4/README.rst` & `pip2deb-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `pip2deb-2.0.4/pip2deb` & `pip2deb-2.0.5/bash-pip2deb`

 * *Files identical despite different names*

### Comparing `pip2deb-2.0.4/pip2deb.egg-info/PKG-INFO` & `pip2deb-2.0.5/pip2deb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 2.0.4
+Version: 2.0.5
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-2.0.4/setup.py` & `pip2deb-2.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 def readme():
     with open('README.rst', 'r') as f:
         content = f.read()
     return content
 
 setup(
     name="pip2deb",
-    version="2.0.4",
+    version="2.0.5",
     decription="A Simple Tool to Pack Python Project into a Debian Package, For Debian/Ubuntu and Termux",
     long_description=readme(),
     url='https://github.com/pacspedd/pip2deb',
     author="PacSpedd",
     author_email="pacspedd@outlook.com",
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.8'
     ],
     packages=find_packages(),
-    scripts=['pip2deb']
+    scripts=['pip2deb-bash', 'pip2deb-python', 'python-pip2deb', 'bash-pip2deb']
 )
```

