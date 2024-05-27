# Comparing `tmp/pip2deb-1.8.tar.gz` & `tmp/pip2deb-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip2deb-1.8.tar", last modified: Mon May 27 14:48:43 2024, max compression
+gzip compressed data, was "pip2deb-1.9.tar", last modified: Mon May 27 14:56:50 2024, max compression
```

## Comparing `pip2deb-1.8.tar` & `pip2deb-1.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 14:48:43.771734 pip2deb-1.8/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-1.8/LICENSE
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-27 14:48:43.771734 pip2deb-1.8/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-1.8/README.rst
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2769 2024-05-27 14:48:06.000000 pip2deb-1.8/pip2deb
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2759 2024-05-26 21:15:49.000000 pip2deb-1.8/pip2deb-sub
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 14:48:43.771734 pip2deb-1.8/pip2deb.egg-info/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-27 14:48:43.000000 pip2deb-1.8/pip2deb.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      171 2024-05-27 14:48:43.000000 pip2deb-1.8/pip2deb.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 14:48:43.000000 pip2deb-1.8/pip2deb.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 14:48:43.000000 pip2deb-1.8/pip2deb.egg-info/top_level.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-27 14:48:43.771734 pip2deb-1.8/setup.cfg
--rw-r--r--   0 whoami    (1002) whoami    (1002)      788 2024-05-27 14:42:29.000000 pip2deb-1.8/setup.py
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 14:56:50.789019 pip2deb-1.9/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-1.9/LICENSE
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-27 14:56:50.789019 pip2deb-1.9/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-1.9/README.rst
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2772 2024-05-27 14:55:09.000000 pip2deb-1.9/pip2deb
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 14:56:50.789019 pip2deb-1.9/pip2deb.egg-info/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-27 14:56:50.000000 pip2deb-1.9/pip2deb.egg-info/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      159 2024-05-27 14:56:50.000000 pip2deb-1.9/pip2deb.egg-info/SOURCES.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 14:56:50.000000 pip2deb-1.9/pip2deb.egg-info/dependency_links.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 14:56:50.000000 pip2deb-1.9/pip2deb.egg-info/top_level.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-27 14:56:50.789019 pip2deb-1.9/setup.cfg
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      789 2024-05-27 14:56:38.000000 pip2deb-1.9/setup.py
```

### Comparing `pip2deb-1.8/LICENSE` & `pip2deb-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pip2deb-1.8/PKG-INFO` & `pip2deb-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 1.8
+Version: 1.9
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-1.8/README.rst` & `pip2deb-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `pip2deb-1.8/pip2deb` & `pip2deb-1.9/pip2deb`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 blue="\033[01;34m"
 cyan="\033[01;36m"
 reset="\033[0m"
 cursive="\033[01;33m"
 bold="\033[01m"
 
 msg() {
-    echo "${green}[${red}*${green}]${cyan} ${@:1} ${reset}" 2>&1
+    echo -e "${green}[${red}*${green}]${cyan} ${@:1} ${reset}" 2>&1
 }
 
 if [ "$#" -ne 2 ]; then
     msg "Usage: $0 <name> <distro>"
     exit 1
 fi
```

### Comparing `pip2deb-1.8/pip2deb.egg-info/PKG-INFO` & `pip2deb-1.9/pip2deb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 1.8
+Version: 1.9
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-1.8/setup.py` & `pip2deb-1.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def readme():
     with open('README.rst', 'r') as f:
         content = f.read()
     return content
 
 setup(
     name="pip2deb",
-    version="1.8",
+    version="1.9",
     decription="A Simple Tool to Pack Python Project into a Debian Package, For Debian/Ubuntu and Termux",
     long_description=readme(),
     url='https://github.com/pacspedd/pip2deb',
     author="PacSpedd",
     author_email="pacspedd@outlook.com",
     license='MIT',
     classifiers=[
@@ -19,8 +19,8 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.8'
     ],
     packages=find_packages(),
     scripts=['pip2deb']
-)
+)
```

