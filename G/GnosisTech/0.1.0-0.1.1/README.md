# Comparing `tmp/GnosisTech-0.1.0.tar.gz` & `tmp/gnosistech-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\GnosisTech-0.1.0.tar", last modified: Fri May 24 08:20:12 2024, max compression
+gzip compressed data, was "dist\gnosistech-0.1.1.tar", last modified: Mon May 27 03:18:05 2024, max compression
```

## Comparing `GnosisTech-0.1.0.tar` & `gnosistech-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 08:20:12.485072 GnosisTech-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-05-24 08:20:12.455089 GnosisTech-0.1.0/GnosisTech.egg-info/
--rw-rw-rw-   0        0        0      472 2024-05-24 08:20:12.000000 GnosisTech-0.1.0/GnosisTech.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-05-24 08:20:12.000000 GnosisTech-0.1.0/GnosisTech.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 08:20:12.000000 GnosisTech-0.1.0/GnosisTech.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-24 08:20:12.000000 GnosisTech-0.1.0/GnosisTech.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      472 2024-05-24 08:20:12.484073 GnosisTech-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 GnosisTech-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 08:20:12.467083 GnosisTech-0.1.0/_backtest_source/
--rw-rw-rw-   0        0        0        0 2024-05-23 03:58:58.000000 GnosisTech-0.1.0/_backtest_source/__init__.py
--rw-rw-rw-   0        0        0    30092 2024-05-23 03:58:58.000000 GnosisTech-0.1.0/_backtest_source/_plotting.py
--rw-rw-rw-   0        0        0     6924 2024-05-23 03:58:58.000000 GnosisTech-0.1.0/_backtest_source/_stats.py
--rw-rw-rw-   0        0        0     5915 2024-05-23 03:58:58.000000 GnosisTech-0.1.0/_backtest_source/_util.py
--rw-rw-rw-   0        0        0    16793 2024-05-23 03:58:58.000000 GnosisTech-0.1.0/_backtest_source/lib.py
--rw-rw-rw-   0        0        0    72566 2024-05-23 03:58:58.000000 GnosisTech-0.1.0/_backtest_source/source.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:20:12.474079 GnosisTech-0.1.0/backtest/
--rw-rw-rw-   0        0        0        0 2024-05-23 03:58:58.000000 GnosisTech-0.1.0/backtest/__init__.py
--rw-rw-rw-   0        0        0      969 2024-05-23 03:58:58.000000 GnosisTech-0.1.0/backtest/event_base.py
--rw-rw-rw-   0        0        0     4188 2024-05-23 03:58:58.000000 GnosisTech-0.1.0/backtest/vectorized.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:20:12.482074 GnosisTech-0.1.0/plot/
--rw-rw-rw-   0        0        0        0 2024-05-23 03:58:58.000000 GnosisTech-0.1.0/plot/__init__.py
--rw-rw-rw-   0        0        0     9363 2024-05-23 09:33:20.000000 GnosisTech-0.1.0/plot/plot.py
--rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 GnosisTech-0.1.0/plot/ultils.py
--rw-rw-rw-   0        0        0       42 2024-05-24 08:20:12.486073 GnosisTech-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      523 2024-05-24 08:20:01.000000 GnosisTech-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:18:05.261097 gnosistech-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-27 03:18:05.259099 gnosistech-0.1.1/GnosisTech.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-05-27 03:18:05.000000 gnosistech-0.1.1/GnosisTech.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2024-05-27 03:18:05.000000 gnosistech-0.1.1/GnosisTech.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 03:18:05.000000 gnosistech-0.1.1/GnosisTech.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 03:18:05.000000 gnosistech-0.1.1/GnosisTech.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      416 2024-05-27 03:18:05.260098 gnosistech-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 03:18:05.262097 gnosistech-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      523 2024-05-27 03:13:21.000000 gnosistech-0.1.1/setup.py
```

### Comparing `GnosisTech-0.1.0/README.md` & `gnosistech-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `GnosisTech-0.1.0/setup.py` & `gnosistech-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='GnosisTech',
-    version='0.1.0',
+    version='0.1.1',
     author='Phung Ngoc An',
     author_email='phungankh2@gmail.com',
     description='PyQuantTrader là một thư viện Python hỗ trợ những vấn đề về quant trading.',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

