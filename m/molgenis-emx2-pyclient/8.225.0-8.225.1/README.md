# Comparing `tmp/molgenis_emx2_pyclient-8.225.0.tar.gz` & `tmp/molgenis_emx2_pyclient-8.225.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgenis_emx2_pyclient-8.225.0.tar", last modified: Fri Oct 20 10:19:40 2023, max compression
+gzip compressed data, was "molgenis_emx2_pyclient-8.225.1.tar", last modified: Fri Oct 20 14:01:30 2023, max compression
```

## Comparing `molgenis_emx2_pyclient-8.225.0.tar` & `molgenis_emx2_pyclient-8.225.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 10:19:40.207348 molgenis_emx2_pyclient-8.225.0/
--rw-r--r--   0 root         (0) root         (0)     7631 2023-10-20 10:07:01.000000 molgenis_emx2_pyclient-8.225.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1903 2023-10-20 10:19:40.207348 molgenis_emx2_pyclient-8.225.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1552 2023-10-20 10:07:01.000000 molgenis_emx2_pyclient-8.225.0/README.md
--rw-r--r--   0 root         (0) root         (0)      634 2023-10-20 10:07:01.000000 molgenis_emx2_pyclient-8.225.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       31 2023-10-20 10:07:01.000000 molgenis_emx2_pyclient-8.225.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-20 10:19:40.207348 molgenis_emx2_pyclient-8.225.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 10:19:40.203348 molgenis_emx2_pyclient-8.225.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 10:19:40.207348 molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient/
--rw-r--r--   0 root         (0) root         (0)       27 2023-10-20 10:07:01.000000 molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14796 2023-10-20 10:07:01.000000 molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient/client.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-10-20 10:07:01.000000 molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-10-20 10:07:01.000000 molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient/graphql_queries.py
--rw-r--r--   0 root         (0) root         (0)      840 2023-10-20 10:07:01.000000 molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 10:19:40.207348 molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1903 2023-10-20 10:19:40.000000 molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      509 2023-10-20 10:19:40.000000 molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-20 10:19:40.000000 molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-10-20 10:19:40.000000 molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-10-20 10:19:40.000000 molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-10-20 10:19:03.000000 molgenis_emx2_pyclient-8.225.0/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 14:01:30.385104 molgenis_emx2_pyclient-8.225.1/
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-10-20 13:49:24.000000 molgenis_emx2_pyclient-8.225.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-10-20 14:01:30.385104 molgenis_emx2_pyclient-8.225.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-10-20 13:49:24.000000 molgenis_emx2_pyclient-8.225.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      634 2023-10-20 13:49:24.000000 molgenis_emx2_pyclient-8.225.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       31 2023-10-20 13:49:24.000000 molgenis_emx2_pyclient-8.225.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-10-20 14:01:30.385104 molgenis_emx2_pyclient-8.225.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 14:01:30.377104 molgenis_emx2_pyclient-8.225.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 14:01:30.381104 molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-10-20 13:49:24.000000 molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14796 2023-10-20 13:49:24.000000 molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient/client.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-10-20 13:49:24.000000 molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-10-20 13:49:24.000000 molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient/graphql_queries.py
+-rw-r--r--   0 root         (0) root         (0)      840 2023-10-20 13:49:24.000000 molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 14:01:30.381104 molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-10-20 14:01:30.000000 molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      509 2023-10-20 14:01:30.000000 molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-20 14:01:30.000000 molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-10-20 14:01:30.000000 molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-10-20 14:01:30.000000 molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-10-20 14:00:54.000000 molgenis_emx2_pyclient-8.225.1/version.txt
```

### Comparing `molgenis_emx2_pyclient-8.225.0/LICENSE` & `molgenis_emx2_pyclient-8.225.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.225.0/PKG-INFO` & `molgenis_emx2_pyclient-8.225.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis_emx2_pyclient
-Version: 8.225.0
+Version: 8.225.1
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molgenis_emx2_pyclient-8.225.0/README.md` & `molgenis_emx2_pyclient-8.225.1/README.md`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.225.0/pyproject.toml` & `molgenis_emx2_pyclient-8.225.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient/client.py` & `molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient/client.py`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient/exceptions.py` & `molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient/graphql_queries.py` & `molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient/utils.py` & `molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient/utils.py`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.225.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO` & `molgenis_emx2_pyclient-8.225.1/src/molgenis_emx2_pyclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-pyclient
-Version: 8.225.0
+Version: 8.225.1
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

