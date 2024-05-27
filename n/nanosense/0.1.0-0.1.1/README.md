# Comparing `tmp/nanosense-0.1.0.tar.gz` & `tmp/nanosense-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanosense-0.1.0.tar", last modified: Sun May 26 06:25:51 2024, max compression
+gzip compressed data, was "nanosense-0.1.1.tar", last modified: Sun May 26 06:36:57 2024, max compression
```

## Comparing `nanosense-0.1.0.tar` & `nanosense-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.093517 nanosense-0.1.0/
--rw-r--r--   0 shankardutt   (501) staff       (20)     1053 2024-05-26 06:25:51.093301 nanosense-0.1.0/PKG-INFO
--rw-r--r--   0 shankardutt   (501) staff       (20)       11 2024-04-05 23:59:28.000000 nanosense-0.1.0/README.md
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.084785 nanosense-0.1.0/nanosense/
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.085938 nanosense-0.1.0/nanosense/Clustering and Data Reduction/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/Clustering and Data Reduction/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)   107280 2024-05-20 03:54:27.000000 nanosense-0.1.0/nanosense/Clustering and Data Reduction/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.086722 nanosense-0.1.0/nanosense/Combine Datasets/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/Combine Datasets/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)     5973 2024-05-08 03:18:56.000000 nanosense-0.1.0/nanosense/Combine Datasets/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.087210 nanosense-0.1.0/nanosense/Data Reduction/
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.088157 nanosense-0.1.0/nanosense/Data Reduction/Docs/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/Data Reduction/Docs/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/Data Reduction/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)   228038 2024-05-20 04:16:55.000000 nanosense-0.1.0/nanosense/Data Reduction/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.088414 nanosense-0.1.0/nanosense/Data Visualisation/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/Data Visualisation/__init__.py
--rwx------   0 shankardutt   (501) staff       (20)   101413 2024-05-19 00:30:33.000000 nanosense-0.1.0/nanosense/Data Visualisation/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.089172 nanosense-0.1.0/nanosense/Event Analysis/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/Event Analysis/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    32048 2024-05-19 00:26:20.000000 nanosense-0.1.0/nanosense/Event Analysis/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.089657 nanosense-0.1.0/nanosense/Frequency and multi-plots/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/Frequency and multi-plots/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    39035 2024-05-19 00:31:20.000000 nanosense-0.1.0/nanosense/Frequency and multi-plots/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.090355 nanosense-0.1.0/nanosense/ML Analysis/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/ML Analysis/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    60685 2024-05-07 07:33:17.000000 nanosense-0.1.0/nanosense/ML Analysis/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.091015 nanosense-0.1.0/nanosense/Nanopore Size Calc/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/Nanopore Size Calc/__init__.py
--rwx------   0 shankardutt   (501) staff       (20)     5069 2024-05-08 03:29:30.000000 nanosense-0.1.0/nanosense/Nanopore Size Calc/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.091408 nanosense-0.1.0/nanosense/Plotting and selecting/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/Plotting and selecting/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    28580 2024-05-07 07:27:05.000000 nanosense-0.1.0/nanosense/Plotting and selecting/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.091987 nanosense-0.1.0/nanosense/Resource Monitor/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/Resource Monitor/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    11105 2024-05-11 05:45:18.000000 nanosense-0.1.0/nanosense/Resource Monitor/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.092561 nanosense-0.1.0/nanosense/Spectrogram and PSD/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/Spectrogram and PSD/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    28223 2024-05-10 06:05:42.000000 nanosense-0.1.0/nanosense/Spectrogram and PSD/main.py
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.0/nanosense/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)     1101 2024-04-29 05:17:53.000000 nanosense-0.1.0/nanosense/crypt_activation.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    15927 2024-05-10 07:48:43.000000 nanosense-0.1.0/nanosense/nanosense.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:51.093038 nanosense-0.1.0/nanosense.egg-info/
--rw-r--r--   0 shankardutt   (501) staff       (20)     1053 2024-05-26 06:25:51.000000 nanosense-0.1.0/nanosense.egg-info/PKG-INFO
--rw-r--r--   0 shankardutt   (501) staff       (20)     1165 2024-05-26 06:25:51.000000 nanosense-0.1.0/nanosense.egg-info/SOURCES.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)        1 2024-05-26 06:25:51.000000 nanosense-0.1.0/nanosense.egg-info/dependency_links.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)      235 2024-05-26 06:25:51.000000 nanosense-0.1.0/nanosense.egg-info/requires.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)       10 2024-05-26 06:25:51.000000 nanosense-0.1.0/nanosense.egg-info/top_level.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)       38 2024-05-26 06:25:51.093573 nanosense-0.1.0/setup.cfg
--rw-r--r--   0 shankardutt   (501) staff       (20)     1166 2024-05-26 06:25:10.000000 nanosense-0.1.0/setup.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.415839 nanosense-0.1.1/
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1054 2024-05-26 06:36:57.415637 nanosense-0.1.1/PKG-INFO
+-rw-r--r--   0 shankardutt   (501) staff       (20)       11 2024-04-05 23:59:28.000000 nanosense-0.1.1/README.md
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.410716 nanosense-0.1.1/nanosense/
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.411970 nanosense-0.1.1/nanosense/Clustering and Data Reduction/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/Clustering and Data Reduction/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)   107280 2024-05-20 03:54:27.000000 nanosense-0.1.1/nanosense/Clustering and Data Reduction/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.412323 nanosense-0.1.1/nanosense/Combine Datasets/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/Combine Datasets/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)     5973 2024-05-08 03:18:56.000000 nanosense-0.1.1/nanosense/Combine Datasets/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.412594 nanosense-0.1.1/nanosense/Data Reduction/
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.412877 nanosense-0.1.1/nanosense/Data Reduction/Docs/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/Data Reduction/Docs/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/Data Reduction/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)   228038 2024-05-20 04:16:55.000000 nanosense-0.1.1/nanosense/Data Reduction/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.413128 nanosense-0.1.1/nanosense/Data Visualisation/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/Data Visualisation/__init__.py
+-rwx------   0 shankardutt   (501) staff       (20)   101413 2024-05-19 00:30:33.000000 nanosense-0.1.1/nanosense/Data Visualisation/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.413443 nanosense-0.1.1/nanosense/Event Analysis/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/Event Analysis/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    32048 2024-05-19 00:26:20.000000 nanosense-0.1.1/nanosense/Event Analysis/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.413757 nanosense-0.1.1/nanosense/Frequency and multi-plots/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/Frequency and multi-plots/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    39035 2024-05-19 00:31:20.000000 nanosense-0.1.1/nanosense/Frequency and multi-plots/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.414050 nanosense-0.1.1/nanosense/ML Analysis/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/ML Analysis/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    60685 2024-05-07 07:33:17.000000 nanosense-0.1.1/nanosense/ML Analysis/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.414332 nanosense-0.1.1/nanosense/Nanopore Size Calc/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/Nanopore Size Calc/__init__.py
+-rwx------   0 shankardutt   (501) staff       (20)     5069 2024-05-08 03:29:30.000000 nanosense-0.1.1/nanosense/Nanopore Size Calc/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.414586 nanosense-0.1.1/nanosense/Plotting and selecting/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/Plotting and selecting/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    28580 2024-05-07 07:27:05.000000 nanosense-0.1.1/nanosense/Plotting and selecting/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.414892 nanosense-0.1.1/nanosense/Resource Monitor/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/Resource Monitor/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    11105 2024-05-11 05:45:18.000000 nanosense-0.1.1/nanosense/Resource Monitor/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.415137 nanosense-0.1.1/nanosense/Spectrogram and PSD/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/Spectrogram and PSD/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    28223 2024-05-10 06:05:42.000000 nanosense-0.1.1/nanosense/Spectrogram and PSD/main.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.1/nanosense/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1101 2024-04-29 05:17:53.000000 nanosense-0.1.1/nanosense/crypt_activation.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    15927 2024-05-10 07:48:43.000000 nanosense-0.1.1/nanosense/nanosense.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:36:57.415369 nanosense-0.1.1/nanosense.egg-info/
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1054 2024-05-26 06:36:57.000000 nanosense-0.1.1/nanosense.egg-info/PKG-INFO
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1201 2024-05-26 06:36:57.000000 nanosense-0.1.1/nanosense.egg-info/SOURCES.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)        1 2024-05-26 06:36:57.000000 nanosense-0.1.1/nanosense.egg-info/dependency_links.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)       55 2024-05-26 06:36:57.000000 nanosense-0.1.1/nanosense.egg-info/entry_points.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)      235 2024-05-26 06:36:57.000000 nanosense-0.1.1/nanosense.egg-info/requires.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)       10 2024-05-26 06:36:57.000000 nanosense-0.1.1/nanosense.egg-info/top_level.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)       38 2024-05-26 06:36:57.415954 nanosense-0.1.1/setup.cfg
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1283 2024-05-26 06:36:02.000000 nanosense-0.1.1/setup.py
```

### Comparing `nanosense-0.1.0/PKG-INFO` & `nanosense-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nanosense
-Version: 0.1.0
+Version: 0.1.1
 Summary: A comprehensive package for nanosense data analysis and visualization.
 Home-page: https://github.com/shankardutt/nanosense
 Author: Shankar Dutt
 Author-email: shankar.dutt@anu.edu.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Requires-Dist: PySide6
 Requires-Dist: cryptography
 Requires-Dist: matplotlib
 Requires-Dist: neo
 Requires-Dist: numpy
 Requires-Dist: pyabf
 Requires-Dist: scipy
```

### Comparing `nanosense-0.1.0/nanosense/Clustering and Data Reduction/main.py` & `nanosense-0.1.1/nanosense/Clustering and Data Reduction/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense/Combine Datasets/main.py` & `nanosense-0.1.1/nanosense/Combine Datasets/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense/Data Reduction/main.py` & `nanosense-0.1.1/nanosense/Data Reduction/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense/Data Visualisation/main.py` & `nanosense-0.1.1/nanosense/Data Visualisation/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense/Event Analysis/main.py` & `nanosense-0.1.1/nanosense/Event Analysis/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense/Frequency and multi-plots/main.py` & `nanosense-0.1.1/nanosense/Frequency and multi-plots/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense/ML Analysis/main.py` & `nanosense-0.1.1/nanosense/ML Analysis/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense/Nanopore Size Calc/main.py` & `nanosense-0.1.1/nanosense/Nanopore Size Calc/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense/Plotting and selecting/main.py` & `nanosense-0.1.1/nanosense/Plotting and selecting/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense/Resource Monitor/main.py` & `nanosense-0.1.1/nanosense/Resource Monitor/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense/Spectrogram and PSD/main.py` & `nanosense-0.1.1/nanosense/Spectrogram and PSD/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense/crypt_activation.py` & `nanosense-0.1.1/nanosense/crypt_activation.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense/nanosense.py` & `nanosense-0.1.1/nanosense/nanosense.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.0/nanosense.egg-info/PKG-INFO` & `nanosense-0.1.1/nanosense.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nanosense
-Version: 0.1.0
+Version: 0.1.1
 Summary: A comprehensive package for nanosense data analysis and visualization.
 Home-page: https://github.com/shankardutt/nanosense
 Author: Shankar Dutt
 Author-email: shankar.dutt@anu.edu.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Requires-Dist: PySide6
 Requires-Dist: cryptography
 Requires-Dist: matplotlib
 Requires-Dist: neo
 Requires-Dist: numpy
 Requires-Dist: pyabf
 Requires-Dist: scipy
```

### Comparing `nanosense-0.1.0/nanosense.egg-info/SOURCES.txt` & `nanosense-0.1.1/nanosense.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.py
 nanosense/__init__.py
 nanosense/crypt_activation.py
 nanosense/nanosense.py
 nanosense.egg-info/PKG-INFO
 nanosense.egg-info/SOURCES.txt
 nanosense.egg-info/dependency_links.txt
+nanosense.egg-info/entry_points.txt
 nanosense.egg-info/requires.txt
 nanosense.egg-info/top_level.txt
 nanosense/Clustering and Data Reduction/__init__.py
 nanosense/Clustering and Data Reduction/main.py
 nanosense/Combine Datasets/__init__.py
 nanosense/Combine Datasets/main.py
 nanosense/Data Reduction/__init__.py
```

### Comparing `nanosense-0.1.0/setup.py` & `nanosense-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nanosense',
-    version='0.1.0',
+    version='0.1.1',
     description='A comprehensive package for nanosense data analysis and visualization.',
     author='Shankar Dutt',
     author_email='shankar.dutt@anu.edu.au',
     url='https://github.com/shankardutt/nanosense',
     packages=find_packages(include=['nanosense', 'nanosense.*']),
     include_package_data=True,
     install_requires=[
@@ -39,9 +39,14 @@
         'pynvml',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.10',
+    entry_points={
+        'console_scripts': [
+            'nanosense=nanosense.nanosense:main',
+        ],
+    },
 )
```

