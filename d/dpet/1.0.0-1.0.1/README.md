# Comparing `tmp/dpet-1.0.0.tar.gz` & `tmp/dpet-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpet-1.0.0.tar", last modified: Mon May 27 12:58:15 2024, max compression
+gzip compressed data, was "dpet-1.0.1.tar", last modified: Mon May 27 12:57:40 2024, max compression
```

## Comparing `dpet-1.0.0.tar` & `dpet-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 12:58:15.944338 dpet-1.0.0/
--rw-rw-rw-   0        0        0      574 2024-05-27 12:58:15.944338 dpet-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-24 14:02:53.000000 dpet-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 12:58:15.921191 dpet-1.0.0/dpet/
--rw-rw-rw-   0        0        0        0 2024-04-16 14:40:30.000000 dpet-1.0.0/dpet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:58:15.937299 dpet-1.0.0/dpet/data/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:02:18.000000 dpet-1.0.0/dpet/data/__init__.py
--rw-rw-rw-   0        0        0      916 2024-04-22 08:46:28.000000 dpet-1.0.0/dpet/data/api_client.py
--rw-rw-rw-   0        0        0     3654 2024-05-24 10:46:19.000000 dpet-1.0.0/dpet/data/comparison.py
--rw-rw-rw-   0        0        0     7248 2024-05-23 08:35:26.000000 dpet-1.0.0/dpet/data/coord.py
--rw-rw-rw-   0        0        0      457 2024-04-22 08:46:28.000000 dpet-1.0.0/dpet/data/extract_tar_gz.py
--rw-rw-rw-   0        0        0     2001 2024-04-16 14:34:09.000000 dpet-1.0.0/dpet/data/topology.py
--rw-rw-rw-   0        0        0    16400 2024-05-23 08:35:26.000000 dpet-1.0.0/dpet/dimensionality_reduction.py
--rw-rw-rw-   0        0        0    17032 2024-05-27 10:51:19.000000 dpet-1.0.0/dpet/ensemble.py
--rw-rw-rw-   0        0        0    26679 2024-05-27 10:46:08.000000 dpet-1.0.0/dpet/ensemble_analysis.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:58:15.942340 dpet-1.0.0/dpet/featurization/
--rw-rw-rw-   0        0        0        0 2024-05-03 14:12:27.000000 dpet-1.0.0/dpet/featurization/__init__.py
--rw-rw-rw-   0        0        0    14279 2024-05-23 08:35:26.000000 dpet-1.0.0/dpet/featurization/angles.py
--rw-rw-rw-   0        0        0     6540 2024-05-23 08:35:26.000000 dpet-1.0.0/dpet/featurization/distances.py
--rw-rw-rw-   0        0        0     1977 2024-05-23 10:07:54.000000 dpet-1.0.0/dpet/featurization/ensemble_level.py
--rw-rw-rw-   0        0        0     1847 2024-05-23 08:35:26.000000 dpet-1.0.0/dpet/featurization/glob.py
--rw-rw-rw-   0        0        0     1979 2024-05-23 08:35:26.000000 dpet-1.0.0/dpet/featurization/utils.py
--rw-rw-rw-   0        0        0    80809 2024-05-24 10:46:19.000000 dpet-1.0.0/dpet/visualization.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:58:15.943338 dpet-1.0.0/dpet.egg-info/
--rw-rw-rw-   0        0        0      574 2024-05-27 12:58:15.000000 dpet-1.0.0/dpet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2024-05-27 12:58:15.000000 dpet-1.0.0/dpet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 12:58:15.000000 dpet-1.0.0/dpet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-05-27 12:58:15.000000 dpet-1.0.0/dpet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-27 12:58:15.000000 dpet-1.0.0/dpet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-24 13:49:45.000000 dpet-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      645 2024-05-27 12:58:15.946355 dpet-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 12:57:40.513807 dpet-1.0.1/
+-rw-rw-rw-   0        0        0      574 2024-05-27 12:57:40.512809 dpet-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:02:53.000000 dpet-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 12:57:40.477288 dpet-1.0.1/dpet/
+-rw-rw-rw-   0        0        0        0 2024-04-16 14:40:30.000000 dpet-1.0.1/dpet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:57:40.505849 dpet-1.0.1/dpet/data/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:02:18.000000 dpet-1.0.1/dpet/data/__init__.py
+-rw-rw-rw-   0        0        0      916 2024-04-22 08:46:28.000000 dpet-1.0.1/dpet/data/api_client.py
+-rw-rw-rw-   0        0        0     3654 2024-05-24 10:46:19.000000 dpet-1.0.1/dpet/data/comparison.py
+-rw-rw-rw-   0        0        0     7248 2024-05-23 08:35:26.000000 dpet-1.0.1/dpet/data/coord.py
+-rw-rw-rw-   0        0        0      457 2024-04-22 08:46:28.000000 dpet-1.0.1/dpet/data/extract_tar_gz.py
+-rw-rw-rw-   0        0        0     2001 2024-04-16 14:34:09.000000 dpet-1.0.1/dpet/data/topology.py
+-rw-rw-rw-   0        0        0    16400 2024-05-23 08:35:26.000000 dpet-1.0.1/dpet/dimensionality_reduction.py
+-rw-rw-rw-   0        0        0    17032 2024-05-27 10:51:19.000000 dpet-1.0.1/dpet/ensemble.py
+-rw-rw-rw-   0        0        0    26679 2024-05-27 10:46:08.000000 dpet-1.0.1/dpet/ensemble_analysis.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:57:40.510809 dpet-1.0.1/dpet/featurization/
+-rw-rw-rw-   0        0        0        0 2024-05-03 14:12:27.000000 dpet-1.0.1/dpet/featurization/__init__.py
+-rw-rw-rw-   0        0        0    14279 2024-05-23 08:35:26.000000 dpet-1.0.1/dpet/featurization/angles.py
+-rw-rw-rw-   0        0        0     6540 2024-05-23 08:35:26.000000 dpet-1.0.1/dpet/featurization/distances.py
+-rw-rw-rw-   0        0        0     1977 2024-05-23 10:07:54.000000 dpet-1.0.1/dpet/featurization/ensemble_level.py
+-rw-rw-rw-   0        0        0     1847 2024-05-23 08:35:26.000000 dpet-1.0.1/dpet/featurization/glob.py
+-rw-rw-rw-   0        0        0     1979 2024-05-23 08:35:26.000000 dpet-1.0.1/dpet/featurization/utils.py
+-rw-rw-rw-   0        0        0    80809 2024-05-24 10:46:19.000000 dpet-1.0.1/dpet/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:57:40.511812 dpet-1.0.1/dpet.egg-info/
+-rw-rw-rw-   0        0        0      574 2024-05-27 12:57:40.000000 dpet-1.0.1/dpet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2024-05-27 12:57:40.000000 dpet-1.0.1/dpet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 12:57:40.000000 dpet-1.0.1/dpet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-27 12:57:40.000000 dpet-1.0.1/dpet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-27 12:57:40.000000 dpet-1.0.1/dpet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-24 13:49:45.000000 dpet-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      645 2024-05-27 12:57:40.514808 dpet-1.0.1/setup.cfg
```

### Comparing `dpet-1.0.0/PKG-INFO` & `dpet-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpet
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for analysing disordered protein ensembles based on MDTraj
 Home-page: https://github.com/hamidrgh/EnsembleTools
 Author: Nikola Ivanovic
 Author-email: nikola.iv.99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `dpet-1.0.0/dpet/data/api_client.py` & `dpet-1.0.1/dpet/data/api_client.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet/data/comparison.py` & `dpet-1.0.1/dpet/data/comparison.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet/data/coord.py` & `dpet-1.0.1/dpet/data/coord.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet/data/topology.py` & `dpet-1.0.1/dpet/data/topology.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet/dimensionality_reduction.py` & `dpet-1.0.1/dpet/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet/ensemble.py` & `dpet-1.0.1/dpet/ensemble.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet/ensemble_analysis.py` & `dpet-1.0.1/dpet/ensemble_analysis.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet/featurization/angles.py` & `dpet-1.0.1/dpet/featurization/angles.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet/featurization/distances.py` & `dpet-1.0.1/dpet/featurization/distances.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet/featurization/ensemble_level.py` & `dpet-1.0.1/dpet/featurization/ensemble_level.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet/featurization/glob.py` & `dpet-1.0.1/dpet/featurization/glob.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet/featurization/utils.py` & `dpet-1.0.1/dpet/featurization/utils.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet/visualization.py` & `dpet-1.0.1/dpet/visualization.py`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/dpet.egg-info/PKG-INFO` & `dpet-1.0.1/dpet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpet
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for analysing disordered protein ensembles based on MDTraj
 Home-page: https://github.com/hamidrgh/EnsembleTools
 Author: Nikola Ivanovic
 Author-email: nikola.iv.99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `dpet-1.0.0/dpet.egg-info/SOURCES.txt` & `dpet-1.0.1/dpet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dpet-1.0.0/setup.cfg` & `dpet-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 7065 740d 0a76 6572 7369 6f6e   = dpet..version
-00000020: 203d 2031 2e30 2e30 0d0a 6175 7468 6f72   = 1.0.0..author
+00000020: 203d 2031 2e30 2e31 0d0a 6175 7468 6f72   = 1.0.1..author
 00000030: 203d 204e 696b 6f6c 6120 4976 616e 6f76   = Nikola Ivanov
 00000040: 6963 0d0a 6175 7468 6f72 5f65 6d61 696c  ic..author_email
 00000050: 203d 206e 696b 6f6c 612e 6976 2e39 3940   = nikola.iv.99@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2041 2050 7974 686f  iption = A Pytho
 00000080: 6e20 7061 636b 6167 6520 666f 7220 616e  n package for an
 00000090: 616c 7973 696e 6720 6469 736f 7264 6572  alysing disorder
```

