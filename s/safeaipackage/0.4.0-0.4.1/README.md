# Comparing `tmp/safeaipackage-0.4.0.tar.gz` & `tmp/safeaipackage-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeaipackage-0.4.0.tar", last modified: Fri Mar  1 07:55:02 2024, max compression
+gzip compressed data, was "safeaipackage-0.4.1.tar", last modified: Mon May 27 07:57:34 2024, max compression
```

## Comparing `safeaipackage-0.4.0.tar` & `safeaipackage-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-01 07:55:02.418814 safeaipackage-0.4.0/
--rw-rw-rw-   0        0        0     1086 2024-01-17 11:00:29.000000 safeaipackage-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     4617 2024-03-01 07:55:02.417818 safeaipackage-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     4081 2024-02-20 21:41:24.000000 safeaipackage-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-01 07:55:02.410744 safeaipackage-0.4.0/safeaipackage/
--rw-rw-rw-   0        0        0        0 2024-01-16 09:13:27.000000 safeaipackage-0.4.0/safeaipackage/__init__.py
--rw-rw-rw-   0        0        0     4114 2024-02-28 16:55:34.000000 safeaipackage-0.4.0/safeaipackage/check_accuracy.py
--rw-rw-rw-   0        0        0     3165 2024-02-28 16:49:02.000000 safeaipackage-0.4.0/safeaipackage/check_explainability.py
--rw-rw-rw-   0        0        0     3181 2024-02-28 16:49:00.000000 safeaipackage-0.4.0/safeaipackage/check_fairness.py
--rw-rw-rw-   0        0        0     3042 2024-02-28 16:49:31.000000 safeaipackage-0.4.0/safeaipackage/check_privacy.py
--rw-rw-rw-   0        0        0     8219 2024-03-01 07:52:43.000000 safeaipackage-0.4.0/safeaipackage/check_robustness.py
-drwxrwxrwx   0        0        0        0 2024-03-01 07:55:02.415824 safeaipackage-0.4.0/safeaipackage/utils/
--rw-rw-rw-   0        0        0        0 2024-02-04 00:43:52.000000 safeaipackage-0.4.0/safeaipackage/utils/__init__.py
--rw-rw-rw-   0        0        0     3801 2024-02-28 16:43:10.000000 safeaipackage-0.4.0/safeaipackage/utils/util.py
-drwxrwxrwx   0        0        0        0 2024-03-01 07:55:02.416821 safeaipackage-0.4.0/safeaipackage.egg-info/
--rw-rw-rw-   0        0        0     4617 2024-03-01 07:55:02.000000 safeaipackage-0.4.0/safeaipackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2024-03-01 07:55:02.000000 safeaipackage-0.4.0/safeaipackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-01 07:55:02.000000 safeaipackage-0.4.0/safeaipackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-01 07:55:02.000000 safeaipackage-0.4.0/safeaipackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-01 07:55:02.418814 safeaipackage-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1051 2024-03-01 07:54:11.000000 safeaipackage-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:57:34.701906 safeaipackage-0.4.1/
+-rw-rw-rw-   0        0        0     1086 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     4907 2024-05-27 07:57:34.701906 safeaipackage-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4371 2024-05-26 14:20:44.000000 safeaipackage-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 07:57:34.694779 safeaipackage-0.4.1/safeaipackage/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/__init__.py
+-rw-rw-rw-   0        0        0     4114 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/check_accuracy.py
+-rw-rw-rw-   0        0        0     3165 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/check_explainability.py
+-rw-rw-rw-   0        0        0     3181 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/check_fairness.py
+-rw-rw-rw-   0        0        0     3042 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/check_privacy.py
+-rw-rw-rw-   0        0        0     8219 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/check_robustness.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:57:34.699909 safeaipackage-0.4.1/safeaipackage/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/utils/__init__.py
+-rw-rw-rw-   0        0        0     3801 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/utils/util.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:57:34.700907 safeaipackage-0.4.1/safeaipackage.egg-info/
+-rw-rw-rw-   0        0        0     4907 2024-05-27 07:57:34.000000 safeaipackage-0.4.1/safeaipackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2024-05-27 07:57:34.000000 safeaipackage-0.4.1/safeaipackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 07:57:34.000000 safeaipackage-0.4.1/safeaipackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-27 07:57:34.000000 safeaipackage-0.4.1/safeaipackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 07:57:34.702907 safeaipackage-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2024-05-27 07:28:19.000000 safeaipackage-0.4.1/setup.py
```

### Comparing `safeaipackage-0.4.0/LICENSE` & `safeaipackage-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `safeaipackage-0.4.0/PKG-INFO` & `safeaipackage-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safeaipackage
-Version: 0.4.0
+Version: 0.4.1
 Summary: SAFE AI package to measure risks of AI models
 Author: Golnoosh Babaei
 Author-email: <golnoosh.babaei93@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -63,10 +63,11 @@
 
 
 # Citations
 
 The proposed measures in this package came primarily out of research by 
 [Paolo Giudici](https://www.linkedin.com/in/paolo-giudici-60028a/), [Emanuela Raffinetti](https://www.linkedin.com/in/emanuela-raffinetti-a3980215/), 
 and [Golnoosh Babaei](https://www.linkedin.com/in/golnoosh-babaei-990077187/) in the [Statistical laboratory](https://sites.google.com/unipv.it/statslab-pavia/home?authuser=0) 
-at the University of Pavia. If you use safe_ai package in your research we would appreciate a citation to the appropriate paper(s):
-* For the RGA measure introduced in "check_accuracy" module, you can read/cite [this paper](https://link.springer.com/article/10.1007/s11135-023-01613-y)
-
+at the University of Pavia. 
+This package is based on the following papers. If you use safeaipackage in your research we would appreciate a citation to our papers:
+* [Giudici, P., & Raffinetti, E. (2024). RGA: a unified measure of predictive accuracy. Advances in Data Analysis and Classification, 1-27.](https://link.springer.com/article/10.1007/s11634-023-00574-2)
+* [Raffinetti, E. (2023). A rank graduation accuracy measure to mitigate artificial intelligence risks. Quality & Quantity, 57(Suppl 2), 131-150.](https://link.springer.com/article/10.1007/s11135-023-01613-y)
```

### Comparing `safeaipackage-0.4.0/README.md` & `safeaipackage-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -48,10 +48,11 @@
 
 
 # Citations
 
 The proposed measures in this package came primarily out of research by 
 [Paolo Giudici](https://www.linkedin.com/in/paolo-giudici-60028a/), [Emanuela Raffinetti](https://www.linkedin.com/in/emanuela-raffinetti-a3980215/), 
 and [Golnoosh Babaei](https://www.linkedin.com/in/golnoosh-babaei-990077187/) in the [Statistical laboratory](https://sites.google.com/unipv.it/statslab-pavia/home?authuser=0) 
-at the University of Pavia. If you use safe_ai package in your research we would appreciate a citation to the appropriate paper(s):
-* For the RGA measure introduced in "check_accuracy" module, you can read/cite [this paper](https://link.springer.com/article/10.1007/s11135-023-01613-y)
-
+at the University of Pavia. 
+This package is based on the following papers. If you use safeaipackage in your research we would appreciate a citation to our papers:
+* [Giudici, P., & Raffinetti, E. (2024). RGA: a unified measure of predictive accuracy. Advances in Data Analysis and Classification, 1-27.](https://link.springer.com/article/10.1007/s11634-023-00574-2)
+* [Raffinetti, E. (2023). A rank graduation accuracy measure to mitigate artificial intelligence risks. Quality & Quantity, 57(Suppl 2), 131-150.](https://link.springer.com/article/10.1007/s11135-023-01613-y)
```

### Comparing `safeaipackage-0.4.0/safeaipackage/check_accuracy.py` & `safeaipackage-0.4.1/safeaipackage/check_accuracy.py`

 * *Files identical despite different names*

### Comparing `safeaipackage-0.4.0/safeaipackage/check_explainability.py` & `safeaipackage-0.4.1/safeaipackage/check_explainability.py`

 * *Files identical despite different names*

### Comparing `safeaipackage-0.4.0/safeaipackage/check_fairness.py` & `safeaipackage-0.4.1/safeaipackage/check_fairness.py`

 * *Files identical despite different names*

### Comparing `safeaipackage-0.4.0/safeaipackage/check_privacy.py` & `safeaipackage-0.4.1/safeaipackage/check_privacy.py`

 * *Files identical despite different names*

### Comparing `safeaipackage-0.4.0/safeaipackage/check_robustness.py` & `safeaipackage-0.4.1/safeaipackage/check_robustness.py`

 * *Files identical despite different names*

### Comparing `safeaipackage-0.4.0/safeaipackage/utils/util.py` & `safeaipackage-0.4.1/safeaipackage/utils/util.py`

 * *Files identical despite different names*

### Comparing `safeaipackage-0.4.0/safeaipackage.egg-info/PKG-INFO` & `safeaipackage-0.4.1/safeaipackage.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safeaipackage
-Version: 0.4.0
+Version: 0.4.1
 Summary: SAFE AI package to measure risks of AI models
 Author: Golnoosh Babaei
 Author-email: <golnoosh.babaei93@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -63,10 +63,11 @@
 
 
 # Citations
 
 The proposed measures in this package came primarily out of research by 
 [Paolo Giudici](https://www.linkedin.com/in/paolo-giudici-60028a/), [Emanuela Raffinetti](https://www.linkedin.com/in/emanuela-raffinetti-a3980215/), 
 and [Golnoosh Babaei](https://www.linkedin.com/in/golnoosh-babaei-990077187/) in the [Statistical laboratory](https://sites.google.com/unipv.it/statslab-pavia/home?authuser=0) 
-at the University of Pavia. If you use safe_ai package in your research we would appreciate a citation to the appropriate paper(s):
-* For the RGA measure introduced in "check_accuracy" module, you can read/cite [this paper](https://link.springer.com/article/10.1007/s11135-023-01613-y)
-
+at the University of Pavia. 
+This package is based on the following papers. If you use safeaipackage in your research we would appreciate a citation to our papers:
+* [Giudici, P., & Raffinetti, E. (2024). RGA: a unified measure of predictive accuracy. Advances in Data Analysis and Classification, 1-27.](https://link.springer.com/article/10.1007/s11634-023-00574-2)
+* [Raffinetti, E. (2023). A rank graduation accuracy measure to mitigate artificial intelligence risks. Quality & Quantity, 57(Suppl 2), 131-150.](https://link.springer.com/article/10.1007/s11135-023-01613-y)
```

### Comparing `safeaipackage-0.4.0/setup.py` & `safeaipackage-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 
 # Open README.md with UTF-8 encoding
 with open(this_directory / "README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '0.4.0'
+VERSION = '0.4.1'
 DESCRIPTION = 'SAFE AI package to measure risks of AI models'
 
 # Setting up
 setup(
     name="safeaipackage",
     version=VERSION,
     author="Golnoosh Babaei",
```

