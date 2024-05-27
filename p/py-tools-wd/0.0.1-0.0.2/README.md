# Comparing `tmp/py_tools_wd-0.0.1.tar.gz` & `tmp/py-tools-wd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_tools_wd-0.0.1.tar", last modified: Mon May 27 05:54:38 2024, max compression
+gzip compressed data, was "py-tools-wd-0.0.2.tar", last modified: Mon May 27 07:58:25 2024, max compression
```

## Comparing `py_tools_wd-0.0.1.tar` & `py-tools-wd-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 05:54:38.575811 py_tools_wd-0.0.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-27 03:17:32.000000 py_tools_wd-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      880 2024-05-27 05:54:38.575811 py_tools_wd-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       27 2024-05-27 03:17:32.000000 py_tools_wd-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 05:54:38.575811 py_tools_wd-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3005 2024-05-27 05:54:21.000000 py_tools_wd-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 05:54:38.571811 py_tools_wd-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 05:54:38.575811 py_tools_wd-0.0.1/src/py_tools_wd/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 04:48:25.000000 py_tools_wd-0.0.1/src/py_tools_wd/__init__.py
--rw-r--r--   0 root         (0) root         (0)      333 2024-05-27 05:54:21.000000 py_tools_wd-0.0.1/src/py_tools_wd/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 05:54:38.575811 py_tools_wd-0.0.1/src/py_tools_wd.egg-info/
--rw-r--r--   0 root         (0) root         (0)      880 2024-05-27 05:54:38.000000 py_tools_wd-0.0.1/src/py_tools_wd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-27 05:54:38.000000 py_tools_wd-0.0.1/src/py_tools_wd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 05:54:38.000000 py_tools_wd-0.0.1/src/py_tools_wd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 05:54:38.000000 py_tools_wd-0.0.1/src/py_tools_wd.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-27 05:54:38.000000 py_tools_wd-0.0.1/src/py_tools_wd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 07:58:25.478941 py-tools-wd-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-27 03:17:32.000000 py-tools-wd-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      880 2024-05-27 07:58:25.478941 py-tools-wd-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       27 2024-05-27 03:17:32.000000 py-tools-wd-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 07:58:25.478941 py-tools-wd-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3028 2024-05-27 07:00:35.000000 py-tools-wd-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 07:58:25.474941 py-tools-wd-0.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 07:58:25.474941 py-tools-wd-0.0.2/src/py_tools_wd/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:38:56.000000 py-tools-wd-0.0.2/src/py_tools_wd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      333 2024-05-27 07:01:50.000000 py-tools-wd-0.0.2/src/py_tools_wd/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 07:58:25.474941 py-tools-wd-0.0.2/src/py_tools_wd/image/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:38:56.000000 py-tools-wd-0.0.2/src/py_tools_wd/image/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3627 2024-05-27 06:45:12.000000 py-tools-wd-0.0.2/src/py_tools_wd/image/image_converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 07:58:25.474941 py-tools-wd-0.0.2/src/py_tools_wd/mq/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:38:56.000000 py-tools-wd-0.0.2/src/py_tools_wd/mq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-05-27 07:33:37.000000 py-tools-wd-0.0.2/src/py_tools_wd/mq/channel.py
+-rw-r--r--   0 root         (0) root         (0)     3985 2024-05-27 07:46:10.000000 py-tools-wd-0.0.2/src/py_tools_wd/mq/kafka.py
+-rw-r--r--   0 root         (0) root         (0)    11196 2024-05-27 07:58:15.000000 py-tools-wd-0.0.2/src/py_tools_wd/mq/rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 07:58:25.474941 py-tools-wd-0.0.2/src/py_tools_wd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      880 2024-05-27 07:58:25.000000 py-tools-wd-0.0.2/src/py_tools_wd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      474 2024-05-27 07:58:25.000000 py-tools-wd-0.0.2/src/py_tools_wd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 07:58:25.000000 py-tools-wd-0.0.2/src/py_tools_wd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 05:54:38.000000 py-tools-wd-0.0.2/src/py_tools_wd.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-27 07:58:25.000000 py-tools-wd-0.0.2/src/py_tools_wd.egg-info/top_level.txt
```

### Comparing `py_tools_wd-0.0.1/LICENSE` & `py-tools-wd-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_tools_wd-0.0.1/PKG-INFO` & `py-tools-wd-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_tools_wd
-Version: 0.0.1
+Name: py-tools-wd
+Version: 0.0.2
 Summary: wd py tools
 Home-page: https://github.com/pgcomb/wd_tools_py
 Author: Wang Dongxu
 Author-email: wangdongxudyx@163.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `py_tools_wd-0.0.1/setup.py` & `py-tools-wd-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 import os
 import sys
 from codecs import open
 
 from setuptools import setup
 
-
 CURRENT_PYTHON = sys.version_info[:2]
 REQUIRED_PYTHON = (3, 8)
 
 if CURRENT_PYTHON < REQUIRED_PYTHON:
     sys.stderr.write(
         """
 ==========================
@@ -23,15 +22,14 @@
 pin to an older version of Requests (<2.32.0).
 """.format(
             *(REQUIRED_PYTHON + CURRENT_PYTHON)
         )
     )
     sys.exit(1)
 
-
 # 'setup.py publish' shortcut.
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist bdist_wheel")
     os.system("twine upload dist/*")
     sys.exit()
 
 requires = [
@@ -54,15 +52,15 @@
     version=about["__version__"],
     description=about["__description__"],
     long_description=readme,
     long_description_content_type="text/markdown",
     author=about["__author__"],
     author_email=about["__author_email__"],
     url=about["__url__"],
-    packages=["py_tools_wd"],
+    packages=["py_tools_wd/image", "py_tools_wd/mq"],
     package_data={"": ["LICENSE", "NOTICE"]},
     package_dir={"": "src"},
     include_package_data=True,
     python_requires=">=3.8",
     install_requires=requires,
     license=about["__license__"],
     zip_safe=False,
@@ -93,8 +91,8 @@
         # "socks": ["PySocks>=1.5.6, !=1.5.7"],
         # "use_chardet_on_py3": ["chardet>=3.0.2,<6"],
     },
     project_urls={
         # "Documentation": "https://requests.readthedocs.io",
         # "Source": "https://github.com/psf/requests",
     },
-)
+)
```

### Comparing `py_tools_wd-0.0.1/src/py_tools_wd.egg-info/PKG-INFO` & `py-tools-wd-0.0.2/src/py_tools_wd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tools-wd
-Version: 0.0.1
+Version: 0.0.2
 Summary: wd py tools
 Home-page: https://github.com/pgcomb/wd_tools_py
 Author: Wang Dongxu
 Author-email: wangdongxudyx@163.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

