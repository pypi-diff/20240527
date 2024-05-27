# Comparing `tmp/pip2deb-2.0.2.tar.gz` & `tmp/pip2deb-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip2deb-2.0.2.tar", last modified: Mon May 27 15:56:18 2024, max compression
+gzip compressed data, was "pip2deb-2.0.3.tar", last modified: Mon May 27 16:02:04 2024, max compression
```

## Comparing `pip2deb-2.0.2.tar` & `pip2deb-2.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 15:56:18.058532 pip2deb-2.0.2/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-2.0.2/LICENSE
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1417 2024-05-27 15:56:18.058532 pip2deb-2.0.2/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-2.0.2/README.rst
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     4807 2024-05-27 15:56:02.000000 pip2deb-2.0.2/pip2deb
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 15:56:18.058532 pip2deb-2.0.2/pip2deb.egg-info/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1417 2024-05-27 15:56:18.000000 pip2deb-2.0.2/pip2deb.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      159 2024-05-27 15:56:18.000000 pip2deb-2.0.2/pip2deb.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 15:56:18.000000 pip2deb-2.0.2/pip2deb.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 15:56:18.000000 pip2deb-2.0.2/pip2deb.egg-info/top_level.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-27 15:56:18.058532 pip2deb-2.0.2/setup.cfg
--rw-r--r--   0 whoami    (1002) whoami    (1002)      791 2024-05-27 15:56:07.000000 pip2deb-2.0.2/setup.py
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 16:02:03.998464 pip2deb-2.0.3/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-2.0.3/LICENSE
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1417 2024-05-27 16:02:03.998464 pip2deb-2.0.3/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-2.0.3/README.rst
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     4807 2024-05-27 16:01:34.000000 pip2deb-2.0.3/pip2deb
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 16:02:03.998464 pip2deb-2.0.3/pip2deb.egg-info/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1417 2024-05-27 16:02:03.000000 pip2deb-2.0.3/pip2deb.egg-info/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      159 2024-05-27 16:02:03.000000 pip2deb-2.0.3/pip2deb.egg-info/SOURCES.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 16:02:03.000000 pip2deb-2.0.3/pip2deb.egg-info/dependency_links.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 16:02:03.000000 pip2deb-2.0.3/pip2deb.egg-info/top_level.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-27 16:02:03.998464 pip2deb-2.0.3/setup.cfg
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      791 2024-05-27 16:01:55.000000 pip2deb-2.0.3/setup.py
```

### Comparing `pip2deb-2.0.2/LICENSE` & `pip2deb-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pip2deb-2.0.2/PKG-INFO` & `pip2deb-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 2.0.2
+Version: 2.0.3
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-2.0.2/README.rst` & `pip2deb-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pip2deb-2.0.2/pip2deb` & `pip2deb-2.0.3/pip2deb`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     else
         dpkg -i --force-overwrite ${package_name} &>/dev/null || abort
         msg "${green}${blue}${package_name}${green} Successfully Installed"
     fi
 }
 
 # Überprüfung der Eingabeparameter
-if [ "$#" -ne 3 ]; then
+if [ "$#" -ne 2 ]; then
     msg "Usage: $0 <name> <distro> <flags>"
     exit 1
 fi
 
 # Unterstützte Distributionen
 case "${distro}" in
     debian|ubuntu)
```

### Comparing `pip2deb-2.0.2/pip2deb.egg-info/PKG-INFO` & `pip2deb-2.0.3/pip2deb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 2.0.2
+Version: 2.0.3
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-2.0.2/setup.py` & `pip2deb-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def readme():
     with open('README.rst', 'r') as f:
         content = f.read()
     return content
 
 setup(
     name="pip2deb",
-    version="2.0.2",
+    version="2.0.3",
     decription="A Simple Tool to Pack Python Project into a Debian Package, For Debian/Ubuntu and Termux",
     long_description=readme(),
     url='https://github.com/pacspedd/pip2deb',
     author="PacSpedd",
     author_email="pacspedd@outlook.com",
     license='MIT',
     classifiers=[
```

