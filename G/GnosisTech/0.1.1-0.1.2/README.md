# Comparing `tmp/gnosistech-0.1.1.tar.gz` & `tmp/gnosistech-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gnosistech-0.1.1.tar", last modified: Mon May 27 03:18:05 2024, max compression
+gzip compressed data, was "dist\gnosistech-0.1.2.tar", last modified: Mon May 27 06:41:57 2024, max compression
```

## Comparing `gnosistech-0.1.1.tar` & `gnosistech-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 03:18:05.261097 gnosistech-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-05-27 03:18:05.259099 gnosistech-0.1.1/GnosisTech.egg-info/
--rw-rw-rw-   0        0        0      416 2024-05-27 03:18:05.000000 gnosistech-0.1.1/GnosisTech.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2024-05-27 03:18:05.000000 gnosistech-0.1.1/GnosisTech.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 03:18:05.000000 gnosistech-0.1.1/GnosisTech.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 03:18:05.000000 gnosistech-0.1.1/GnosisTech.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      416 2024-05-27 03:18:05.260098 gnosistech-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-27 03:18:05.262097 gnosistech-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      523 2024-05-27 03:13:21.000000 gnosistech-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:41:57.194354 gnosistech-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-05-27 06:41:57.191356 gnosistech-0.1.2/GnosisTech.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-05-27 06:41:57.000000 gnosistech-0.1.2/GnosisTech.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      678 2024-05-27 06:41:57.000000 gnosistech-0.1.2/GnosisTech.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 06:41:57.000000 gnosistech-0.1.2/GnosisTech.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-27 06:41:57.000000 gnosistech-0.1.2/GnosisTech.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      416 2024-05-27 06:41:57.192356 gnosistech-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 06:41:57.153379 gnosistech-0.1.2/pyquanttrade/
+-rw-rw-rw-   0        0        0        0 2024-05-27 06:31:36.000000 gnosistech-0.1.2/pyquanttrade/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:41:57.166370 gnosistech-0.1.2/pyquanttrade/_backtest_source/
+-rw-rw-rw-   0        0        0        0 2024-05-23 03:58:58.000000 gnosistech-0.1.2/pyquanttrade/_backtest_source/__init__.py
+-rw-rw-rw-   0        0        0    30092 2024-05-23 03:58:58.000000 gnosistech-0.1.2/pyquanttrade/_backtest_source/_plotting.py
+-rw-rw-rw-   0        0        0     6924 2024-05-23 03:58:58.000000 gnosistech-0.1.2/pyquanttrade/_backtest_source/_stats.py
+-rw-rw-rw-   0        0        0     5915 2024-05-23 03:58:58.000000 gnosistech-0.1.2/pyquanttrade/_backtest_source/_util.py
+-rw-rw-rw-   0        0        0    16793 2024-05-23 03:58:58.000000 gnosistech-0.1.2/pyquanttrade/_backtest_source/lib.py
+-rw-rw-rw-   0        0        0    72566 2024-05-23 03:58:58.000000 gnosistech-0.1.2/pyquanttrade/_backtest_source/source.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:41:57.178363 gnosistech-0.1.2/pyquanttrade/backtest/
+-rw-rw-rw-   0        0        0        0 2024-05-23 03:58:58.000000 gnosistech-0.1.2/pyquanttrade/backtest/__init__.py
+-rw-rw-rw-   0        0        0      969 2024-05-23 03:58:58.000000 gnosistech-0.1.2/pyquanttrade/backtest/event_base.py
+-rw-rw-rw-   0        0        0     4188 2024-05-23 03:58:58.000000 gnosistech-0.1.2/pyquanttrade/backtest/vectorized.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:41:57.182362 gnosistech-0.1.2/pyquanttrade/data/
+-rw-rw-rw-   0        0        0        0 2024-05-26 06:44:06.000000 gnosistech-0.1.2/pyquanttrade/data/__init__.py
+-rw-rw-rw-   0        0        0     4228 2024-05-23 03:58:58.000000 gnosistech-0.1.2/pyquanttrade/data/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:41:57.189356 gnosistech-0.1.2/pyquanttrade/plot/
+-rw-rw-rw-   0        0        0        0 2024-05-23 03:58:58.000000 gnosistech-0.1.2/pyquanttrade/plot/__init__.py
+-rw-rw-rw-   0        0        0     7421 2024-05-26 09:16:51.000000 gnosistech-0.1.2/pyquanttrade/plot/plot.py
+-rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-0.1.2/pyquanttrade/plot/ultils.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 06:41:57.194354 gnosistech-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      523 2024-05-27 06:35:41.000000 gnosistech-0.1.2/setup.py
```

### Comparing `gnosistech-0.1.1/LICENSE` & `gnosistech-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.1/README.md` & `gnosistech-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.1/setup.py` & `gnosistech-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='GnosisTech',
-    version='0.1.1',
+    version='0.1.2',
     author='Phung Ngoc An',
     author_email='phungankh2@gmail.com',
     description='PyQuantTrader là một thư viện Python hỗ trợ những vấn đề về quant trading.',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

