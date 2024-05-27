# Comparing `tmp/biobb_dna-4.1.0.tar.gz` & `tmp/biobb_dna-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_dna-4.1.0.tar", last modified: Fri Sep  8 07:41:07 2023, max compression
+gzip compressed data, was "biobb_dna-4.2.0.tar", last modified: Mon May 27 11:11:52 2024, max compression
```

## Comparing `biobb_dna-4.1.0.tar` & `biobb_dna-4.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 07:41:07.875619 biobb_dna-4.1.0/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:33:51.000000 biobb_dna-4.1.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     6057 2023-09-08 07:41:07.875451 biobb_dna-4.1.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5188 2023-09-08 07:37:33.000000 biobb_dna-4.1.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 07:41:07.870544 biobb_dna-4.1.0/biobb_dna/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      157 2023-09-08 07:37:18.000000 biobb_dna-4.1.0/biobb_dna/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 07:41:07.871830 biobb_dna-4.1.0/biobb_dna/backbone/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       74 2022-05-26 11:33:51.000000 biobb_dna-4.1.0/biobb_dna/backbone/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12720 2023-04-12 15:08:16.000000 biobb_dna-4.1.0/biobb_dna/backbone/bipopulations.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13445 2023-04-12 15:08:33.000000 biobb_dna-4.1.0/biobb_dna/backbone/canonicalag.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11634 2023-04-12 15:08:43.000000 biobb_dna-4.1.0/biobb_dna/backbone/puckering.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 07:41:07.872680 biobb_dna-4.1.0/biobb_dna/curvesplus/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       74 2022-05-26 11:33:51.000000 biobb_dna-4.1.0/biobb_dna/curvesplus/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10804 2023-04-12 15:09:45.000000 biobb_dna-4.1.0/biobb_dna/curvesplus/biobb_canal.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11639 2023-04-12 15:10:52.000000 biobb_dna-4.1.0/biobb_dna/curvesplus/biobb_canion.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13251 2023-04-13 13:28:52.000000 biobb_dna-4.1.0/biobb_dna/curvesplus/biobb_curves.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 07:41:07.873219 biobb_dna-4.1.0/biobb_dna/dna/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573       76 2022-05-26 11:33:51.000000 biobb_dna-4.1.0/biobb_dna/dna/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10973 2023-04-12 15:12:33.000000 biobb_dna-4.1.0/biobb_dna/dna/dna_averages.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13415 2023-04-12 15:13:22.000000 biobb_dna-4.1.0/biobb_dna/dna/dna_bimodality.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11440 2023-04-12 15:13:31.000000 biobb_dna-4.1.0/biobb_dna/dna/dna_timeseries.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 07:41:07.873808 biobb_dna-4.1.0/biobb_dna/interbp_correlations/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573      100 2022-05-26 11:33:51.000000 biobb_dna-4.1.0/biobb_dna/interbp_correlations/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15558 2023-04-12 15:13:59.000000 biobb_dna-4.1.0/biobb_dna/interbp_correlations/interbpcorr.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15215 2023-04-12 15:15:07.000000 biobb_dna-4.1.0/biobb_dna/interbp_correlations/interhpcorr.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10022 2023-04-12 15:17:30.000000 biobb_dna-4.1.0/biobb_dna/interbp_correlations/interseqcorr.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 07:41:07.874312 biobb_dna-4.1.0/biobb_dna/intrabp_correlations/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573      100 2022-05-26 11:33:51.000000 biobb_dna-4.1.0/biobb_dna/intrabp_correlations/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15851 2023-04-12 15:17:50.000000 biobb_dna-4.1.0/biobb_dna/intrabp_correlations/intrabpcorr.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15755 2023-04-12 15:18:20.000000 biobb_dna-4.1.0/biobb_dna/intrabp_correlations/intrahpcorr.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9919 2023-04-12 15:18:33.000000 biobb_dna-4.1.0/biobb_dna/intrabp_correlations/intraseqcorr.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 07:41:07.874680 biobb_dna-4.1.0/biobb_dna/stiffness/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573       73 2022-05-26 11:33:51.000000 biobb_dna-4.1.0/biobb_dna/stiffness/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10178 2023-04-12 15:30:30.000000 biobb_dna-4.1.0/biobb_dna/stiffness/average_stiffness.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12639 2023-04-12 15:30:58.000000 biobb_dna-4.1.0/biobb_dna/stiffness/basepair_stiffness.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 07:41:07.874803 biobb_dna-4.1.0/biobb_dna/test/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:33:51.000000 biobb_dna-4.1.0/biobb_dna/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 07:41:07.875263 biobb_dna-4.1.0/biobb_dna/utils/
--rw-r--r--   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:33:52.000000 biobb_dna-4.1.0/biobb_dna/utils/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573      900 2022-05-26 11:33:52.000000 biobb_dna-4.1.0/biobb_dna/utils/constants.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1363 2023-03-06 08:33:07.000000 biobb_dna-4.1.0/biobb_dna/utils/loader.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573      341 2022-05-26 11:33:52.000000 biobb_dna-4.1.0/biobb_dna/utils/transform.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 07:41:07.871280 biobb_dna-4.1.0/biobb_dna.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     6057 2023-09-08 07:41:07.000000 biobb_dna-4.1.0/biobb_dna.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1262 2023-09-08 07:41:07.000000 biobb_dna-4.1.0/biobb_dna.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-09-08 07:41:07.000000 biobb_dna-4.1.0/biobb_dna.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      981 2023-09-08 07:41:07.000000 biobb_dna-4.1.0/biobb_dna.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       55 2023-09-08 07:41:07.000000 biobb_dna-4.1.0/biobb_dna.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       10 2023-09-08 07:41:07.000000 biobb_dna-4.1.0/biobb_dna.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-09-08 07:41:07.875669 biobb_dna-4.1.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2541 2023-09-08 07:36:54.000000 biobb_dna-4.1.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-27 11:11:52.482724 biobb_dna-4.2.0/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:33:51.000000 biobb_dna-4.2.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6696 2024-05-27 11:11:52.482483 biobb_dna-4.2.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5727 2024-05-27 11:10:18.000000 biobb_dna-4.2.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-27 11:11:52.477558 biobb_dna-4.2.0/biobb_dna/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      157 2024-05-27 11:10:04.000000 biobb_dna-4.2.0/biobb_dna/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-27 11:11:52.479155 biobb_dna-4.2.0/biobb_dna/backbone/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       74 2022-05-26 11:33:51.000000 biobb_dna-4.2.0/biobb_dna/backbone/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12789 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/backbone/bipopulations.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13528 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/backbone/canonicalag.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11723 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/backbone/puckering.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-27 11:11:52.479727 biobb_dna-4.2.0/biobb_dna/curvesplus/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       74 2022-05-26 11:33:51.000000 biobb_dna-4.2.0/biobb_dna/curvesplus/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10880 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/curvesplus/biobb_canal.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11700 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/curvesplus/biobb_canion.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13345 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/curvesplus/biobb_curves.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-27 11:11:52.480263 biobb_dna-4.2.0/biobb_dna/dna/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       76 2022-05-26 11:33:51.000000 biobb_dna-4.2.0/biobb_dna/dna/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11053 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/dna/dna_averages.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13495 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/dna/dna_bimodality.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11610 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/dna/dna_timeseries.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-27 11:11:52.480779 biobb_dna-4.2.0/biobb_dna/interbp_correlations/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      100 2022-05-26 11:33:51.000000 biobb_dna-4.2.0/biobb_dna/interbp_correlations/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15650 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/interbp_correlations/interbpcorr.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15300 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/interbp_correlations/interhpcorr.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10130 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/interbp_correlations/interseqcorr.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-27 11:11:52.481267 biobb_dna-4.2.0/biobb_dna/intrabp_correlations/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      100 2022-05-26 11:33:51.000000 biobb_dna-4.2.0/biobb_dna/intrabp_correlations/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15943 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/intrabp_correlations/intrabpcorr.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15840 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/intrabp_correlations/intrahpcorr.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10033 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/intrabp_correlations/intraseqcorr.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-27 11:11:52.481641 biobb_dna-4.2.0/biobb_dna/stiffness/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       73 2022-05-26 11:33:51.000000 biobb_dna-4.2.0/biobb_dna/stiffness/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10519 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/stiffness/average_stiffness.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12746 2024-05-24 09:00:12.000000 biobb_dna-4.2.0/biobb_dna/stiffness/basepair_stiffness.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-27 11:11:52.481768 biobb_dna-4.2.0/biobb_dna/test/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:33:51.000000 biobb_dna-4.2.0/biobb_dna/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-27 11:11:52.482216 biobb_dna-4.2.0/biobb_dna/utils/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:33:52.000000 biobb_dna-4.2.0/biobb_dna/utils/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      900 2022-05-26 11:33:52.000000 biobb_dna-4.2.0/biobb_dna/utils/constants.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1363 2023-03-06 08:33:07.000000 biobb_dna-4.2.0/biobb_dna/utils/loader.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      341 2022-05-26 11:33:52.000000 biobb_dna-4.2.0/biobb_dna/utils/transform.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-27 11:11:52.478600 biobb_dna-4.2.0/biobb_dna.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6696 2024-05-27 11:11:52.000000 biobb_dna-4.2.0/biobb_dna.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1262 2024-05-27 11:11:52.000000 biobb_dna-4.2.0/biobb_dna.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2024-05-27 11:11:52.000000 biobb_dna-4.2.0/biobb_dna.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      981 2024-05-27 11:11:52.000000 biobb_dna-4.2.0/biobb_dna.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       55 2024-05-27 11:11:52.000000 biobb_dna-4.2.0/biobb_dna.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       10 2024-05-27 11:11:52.000000 biobb_dna-4.2.0/biobb_dna.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2024-05-27 11:11:52.482773 biobb_dna-4.2.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2541 2024-05-27 11:09:53.000000 biobb_dna-4.2.0/setup.py
```

### Comparing `biobb_dna-4.1.0/LICENSE` & `biobb_dna-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_dna-4.1.0/PKG-INFO` & `biobb_dna-4.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,13 @@
-Metadata-Version: 2.1
-Name: biobb_dna
-Version: 4.1.0
-Summary: Biobb_dna is a package composed of different analyses for nucleic acid trajectories.
-Home-page: https://github.com/bioexcel/biobb_dna
-Author: Biobb developers
-Author-email: lucia.fabio@irbbarcelona.com
-Project-URL: Documentation, http://biobb_dna.readthedocs.io/en/latest/
-Project-URL: Bioexcel, https://bioexcel.eu/
-Keywords: Bioinformatics Workflows BioExcel Compatibility
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_dna?label=Version)](https://GitHub.com/bioexcel/biobb_dna/tags/)
 [![](https://img.shields.io/pypi/v/biobb-dna.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-dna/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_dna?label=Conda)](https://anaconda.org/bioconda/biobb_dna)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_dna?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_dna)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_dna?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_dna:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_dna:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_dna)
 [![](https://img.shields.io/pypi/pyversions/biobb-dna.svg?label=Python%20Versions)](https://pypi.org/project/biobb-dna/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_dna)
 
 [![](https://readthedocs.org/projects/biobb-dna/badge/?version=latest&label=Docs)](https://biobb-dna.readthedocs.io/en/latest/?badge=latest)
@@ -39,84 +18,91 @@
 
 [![](https://docs.bioexcel.eu/biobb_dna/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_dna/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_dna/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_dna/coverage/)
 [![](https://docs.bioexcel.eu/biobb_dna/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_dna/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_dna?label=Last%20Commit)](https://github.com/bioexcel/biobb_dna/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_dna.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_dna/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_dna
 
 ## Introduction
 Biobb_dna is a package composed of different analyses for 
 nucleic acid trajectories and helical parameters.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_dna.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-dna.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_dna>=4.1.0"
+        pip install "biobb_dna>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-dna.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_dna>=4.1.0"
+        conda install -c bioconda "biobb_dna>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-dna.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-dna.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_dna:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_dna:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_dna:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_dna:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_dna.sif https://depot.galaxyproject.org/singularity/biobb_dna:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_dna.sif https://depot.galaxyproject.org/singularity/biobb_dna:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_dna.sif <command>
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-dna.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
-![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
+![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_dna-4.1.0/biobb_dna/backbone/bipopulations.py` & `biobb_dna-4.2.0/biobb_dna/backbone/bipopulations.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from biobb_common.configuration import settings
 
 
 class BIPopulations(BiobbObject):
     """
     | biobb_dna BIPopulations
     | Calculate BI/BII populations from epsilon and zeta parameters.
+    | Calculate BI/BII populations from epsilon and zeta parameters.
 
     Args:
         input_epsilC_path (str): Path to .ser file for helical parameter 'epsilC'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/backbone/canal_output_epsilC.ser>`_. Accepted formats: ser (edam:format_2330).
         input_epsilW_path (str): Path to .ser file for helical parameter 'epsilW'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/backbone/canal_output_epsilW.ser>`_. Accepted formats: ser (edam:format_2330).
         input_zetaC_path (str): Path to .ser file for helical parameter 'zetaC'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/backbone/canal_output_zetaC.ser>`_. Accepted formats: ser (edam:format_2330).
         input_zetaW_path (str): Path to .ser file for helical parameter 'zetaW'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/backbone/canal_output_zetaW.ser>`_. Accepted formats: ser (edam:format_2330).
         output_csv_path (str): Path to .csv file where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/backbone/bipop_ref.csv>`_. Accepted formats: csv (edam:format_3752).
```

### Comparing `biobb_dna-4.1.0/biobb_dna/backbone/canonicalag.py` & `biobb_dna-4.2.0/biobb_dna/backbone/canonicalag.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from biobb_common.configuration import settings
 
 
 class CanonicalAG(BiobbObject):
     """
     | biobb_dna CanonicalAG
     | Calculate Canonical Alpha/Gamma populations from alpha and gamma parameters.
+    | Calculate Canonical Alpha/Gamma populations from alpha and gamma parameters.
 
     Args:
         input_alphaC_path (str): Path to .ser file for helical parameter 'alphaC'. File type: input. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/backbone/canal_output_alphaC.ser>`_. Accepted formats: ser (edam:format_2330).
         input_alphaW_path (str): Path to .ser file for helical parameter 'alphaW'. File type: input. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/backbone/canal_output_alphaW.ser>`_. Accepted formats: ser (edam:format_2330).
         input_gammaC_path (str): Path to .ser file for helical parameter 'gammaC'. File type: input. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/backbone/canal_output_gammaC.ser>`_. Accepted formats: ser (edam:format_2330).
         input_gammaW_path (str): Path to .ser file for helical parameter 'gammaW'. File type: input. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/backbone/canal_output_gammaW.ser>`_. Accepted formats: ser (edam:format_2330).
         output_csv_path (str): Path to .csv file where output is saved. File type: output. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/backbone/canonag_ref.csv>`_. Accepted formats: csv (edam:format_3752).
```

### Comparing `biobb_dna-4.1.0/biobb_dna/backbone/puckering.py` & `biobb_dna-4.2.0/biobb_dna/backbone/puckering.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from biobb_common.configuration import settings
 
 
 class Puckering(BiobbObject):
     """
     | biobb_dna Puckering
     | Calculate Puckering from phase parameters.
+    | Calculate North/East/West/South distribution of sugar puckering backbone torsions.
 
     Args:
         input_phaseC_path (str): Path to .ser file for helical parameter 'phaseC'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/backbone/canal_output_phaseC.ser>`_. Accepted formats: ser (edam:format_2330).
         input_phaseW_path (str): Path to .ser file for helical parameter 'phaseW'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/backbone/canal_output_phaseW.ser>`_. Accepted formats: ser (edam:format_2330).
         output_csv_path (str): Path to .csv file where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/backbone/puckering_ref.csv>`_. Accepted formats: csv (edam:format_3752).
         output_jpg_path (str): Path to .jpg file where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/backbone/puckering_ref.jpg>`_. Accepted formats: jpg (edam:format_3579).
         properties (dict):
```

### Comparing `biobb_dna-4.1.0/biobb_dna/curvesplus/biobb_canal.py` & `biobb_dna-4.2.0/biobb_dna/curvesplus/biobb_canal.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Canal(BiobbObject):
     """
     | biobb_dna Canal
     | Wrapper for the Canal executable that is part of the Curves+ software suite.
+    | The Canal program is used to analyze the curvature of DNA structures.
 
     Args:
         input_cda_file (str): Input cda file, from Cur+ output. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/curvesplus/curves_output.cda>`_. Accepted formats: cda (edam:format_2330).
         input_lis_file (str) (Optional): Input lis file, from Cur+ output. File type: input. Accepted formats: lis (edam:format_2330).
         output_zip_path (str): zip filename for output files. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/curvesplus/canal_output.zip>`_. Accepted formats: zip (edam:format_3987).
         properties (dic):
             * **bases** (*str*) - (None) sequence of bases to be searched for in the I/P data (default is blank, meaning no specified sequence).
```

### Comparing `biobb_dna-4.1.0/biobb_dna/curvesplus/biobb_canion.py` & `biobb_dna-4.2.0/biobb_dna/curvesplus/biobb_canion.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Canion(BiobbObject):
     """
     | biobb_dna Canion
     | Wrapper for the Canion executable  that is part of the Curves+ software suite.
+    | Analyzes the trajectory of ions around a DNA molecule.
 
     Args:
         input_cdi_path (str): Trajectory input file. File type: input. `Sample file <https://mmb.irbbarcelona.org/biobb-dev/biobb-api/public/samples/THGA_K.cdi>`_. Accepted formats: cdi (edam:format_2330).
         input_afr_path (str): Helical axis frames corresponding to the input conformation to be analyzed. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/curvesplus/THGA.afr>`_. Accepted formats: afr (edam:format_2330).
         input_avg_struc_path (str): Average DNA conformation. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/curvesplus/THGA_avg.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_zip_path (str) (Optional): Filename for .zip files containing Canion output files. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/curvesplus/canion_output.zip>`_. Accepted formats: zip (edam:format_3987).
         properties (dict):
```

### Comparing `biobb_dna-4.1.0/biobb_dna/curvesplus/biobb_curves.py` & `biobb_dna-4.2.0/biobb_dna/curvesplus/biobb_curves.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Curves(BiobbObject):
     """
     | biobb_dna Curves
     | Wrapper for the Cur+ executable  that is part of the Curves+ software suite.
+    | The Cur+ program is used to analyze the structure of nucleic acids and their complexes.
 
     Args:
         input_struc_path (str): Trajectory or PDB input file. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/curvesplus/structure.stripped.trj>`_. Accepted formats: trj (edam:format_3910), pdb (edam:format_1476), netcdf (edam:format_3650), nc (edam:format_3650).
         input_top_path (str) (Optional): Topology file, needed along with .trj file (optional). File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/curvesplus/structure.stripped.top>`_. Accepted formats: top (edam:format_3881).
         output_cda_path (str): Filename for Curves+ output .cda file. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/curvesplus/curves_trj_output.cda>`_. Accepted formats: cda (edam:format_2330).
         output_lis_path (str): Filename for Curves+ output .lis file. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/curvesplus/curves_trj_output.lis>`_. Accepted formats: lis (edam:format_2330).
         output_zip_path (str) (Optional): Filename for .zip files containing Curves+ output that is not .cda or .lis files. File type: output. Accepted formats: zip (edam:format_3987).
```

### Comparing `biobb_dna-4.1.0/biobb_dna/dna/dna_averages.py` & `biobb_dna-4.2.0/biobb_dna/dna/dna_averages.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from biobb_common.configuration import settings
 
 
 class HelParAverages(BiobbObject):
     """
     | biobb_dna HelParAverages
     | Load .ser file for a given helical parameter and read each column corresponding to a base calculating average over each one.
+    | Calculate average values for each base pair and save them in a .csv file.
 
     Args:
         input_ser_path (str): Path to .ser file for helical parameter. File is expected to be a table, with the first column being an index and the rest the helical parameter values for each base/basepair. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/dna/canal_output_shift.ser>`_. Accepted formats: ser (edam:format_2330).
         output_csv_path (str): Path to .csv file where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/dna/shift_avg.csv>`_. Accepted formats: csv (edam:format_3752).
         output_jpg_path (str): Path to .jpg file where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/dna/shift_avg.jpg>`_. Accepted formats: jpg (edam:format_3579).
         properties (dict):
             * **sequence** (*str*) - (None) Nucleic acid sequence corresponding to the input .ser file. Length of sequence is expected to be the same as the total number of columns in the .ser file, minus the index column (even if later on a subset of columns is selected with the *seqpos* option).
```

### Comparing `biobb_dna-4.1.0/biobb_dna/dna/dna_bimodality.py` & `biobb_dna-4.2.0/biobb_dna/dna/dna_bimodality.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from biobb_dna.utils.loader import load_data
 
 
 class HelParBimodality(BiobbObject):
     """
     | biobb_dna HelParBimodality
     | Determine binormality/bimodality from a helical parameter series dataset.
+    | Determine binormality/bimodality from a helical parameter series dataset.
 
     Args:
         input_csv_file (str): Path to .csv file with helical parameter series. If `input_zip_file` is passed, this should be just the filename of the .csv file inside .zip.  File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/dna/series_shift_AT.csv>`_. Accepted formats: csv (edam:format_3752).
         input_zip_file (str) (Optional): .zip file containing the `input_csv_file` .csv file. File type: input. Accepted formats: zip (edam:format_3987).
         output_csv_path (str): Path to .csv file where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/dna/AT_shift_bimod.csv>`_. Accepted formats: csv (edam:format_3752).
         output_jpg_path (str): Path to .jpg file where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/dna/AT_shift_bimod.jpg>`_. Accepted formats: jpg (edam:format_3579).
         properties (dict):
```

### Comparing `biobb_dna-4.1.0/biobb_dna/dna/dna_timeseries.py` & `biobb_dna-4.2.0/biobb_dna/dna/dna_timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from biobb_common.tools.file_utils import launchlogger
 
 
 class HelParTimeSeries(BiobbObject):
     """
     | biobb_dna HelParTimeSeries
     | Created time series and histogram plots for each base pair from a helical parameter series file.
+    | The helical parameter series file is expected to be a table, with the first column being an index and the rest the helical parameter values for each base/basepair.
 
     Args:
         input_ser_path (str): Path to .ser file for helical parameter. File is expected to be a table, with the first column being an index and the rest the helical parameter values for each base/basepair. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/dna/canal_output_shift.ser>`_. Accepted formats: ser (edam:format_2330).
         output_zip_path (str): Path to output .zip files where data is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/dna/timeseries_output.zip>`_. Accepted formats: zip (edam:format_3987).
         properties (dict):
             * **sequence** (*str*) - (None) Nucleic acid sequence corresponding to the input .ser file. Length of sequence is expected to be the same as the total number of columns in the .ser file, minus the index column (even if later on a subset of columns is selected with the *usecols* option).
             * **bins** (*int*) - (None) Bins for histogram. Parameter has same options as matplotlib.pyplot.hist.
```

### Comparing `biobb_dna-4.1.0/biobb_dna/interbp_correlations/interbpcorr.py` & `biobb_dna-4.2.0/biobb_dna/interbp_correlations/interbpcorr.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from biobb_dna.utils import constants
 
 
 class InterBasePairCorrelation(BiobbObject):
     """
     | biobb_dna InterBasePairCorrelation
     | Calculate correlation between all base pairs of a single sequence and for a single helical parameter.
+    | Calculate correlation between neighboring base pairs and pairs of helical parameters.
 
     Args:
         input_filename_shift (str): Path to .ser file with data for helical parameter 'shift'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/canal_output_shift.ser>`_. Accepted formats: ser (edam:format_2330).
         input_filename_slide (str): Path to .ser file with data for helical parameter 'slide'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/canal_output_slide.ser>`_. Accepted formats: ser (edam:format_2330).
         input_filename_rise (str): Path to .ser file with data for helical parameter 'rise'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/canal_output_rise.ser>`_. Accepted formats: ser (edam:format_2330).
         input_filename_tilt (str): Path to .ser file with data for helical parameter 'tilt'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/canal_output_tilt.ser>`_. Accepted formats: ser (edam:format_2330).
         input_filename_roll (str): Path to .ser file with data for helical parameter 'roll'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/canal_output_roll.ser>`_. Accepted formats: ser (edam:format_2330).
```

### Comparing `biobb_dna-4.1.0/biobb_dna/interbp_correlations/interhpcorr.py` & `biobb_dna-4.2.0/biobb_dna/interbp_correlations/interhpcorr.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from biobb_dna.utils.loader import load_data
 
 
 class InterHelParCorrelation(BiobbObject):
     """
     | biobb_dna InterHelParCorrelation
     | Calculate correlation between helical parameters for a single inter-base pair.
+    | Calculate correlation between helical parameters for a single inter-base pair.
 
     Args:
         input_filename_shift (str): Path to .csv file with data for helical parameter 'shift'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/stiffness/series_shift_AA.csv>`_. Accepted formats: csv (edam:format_3752).
         input_filename_slide (str): Path to .csv file with data for helical parameter 'slide'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/stiffness/series_slide_AA.csv>`_. Accepted formats: csv (edam:format_3752).
         input_filename_rise (str): Path to .csv file with data for helical parameter 'rise'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/stiffness/series_rise_AA.csv>`_. Accepted formats: csv (edam:format_3752).
         input_filename_tilt (str): Path to .csv file with data for helical parameter 'tilt'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/stiffness/series_tilt_AA.csv>`_. Accepted formats: csv (edam:format_3752).
         input_filename_roll (str): Path to .csv file with data for helical parameter 'roll'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/stiffness/series_roll_AA.csv>`_. Accepted formats: csv (edam:format_3752).
```

### Comparing `biobb_dna-4.1.0/biobb_dna/interbp_correlations/interseqcorr.py` & `biobb_dna-4.2.0/biobb_dna/interbp_correlations/interseqcorr.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from biobb_dna.utils import constants
 
 
 class InterSequenceCorrelation(BiobbObject):
     """
     | biobb_dna InterSequenceCorrelation
     | Calculate correlation between all base pairs of a single sequence and for a single helical parameter.
+    | Calculate correlation between all base pairs of a single sequence and for a single helical parameter.
 
     Args:
         input_ser_path (str): Path to .ser file with data for single helical parameter. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/canal_output_roll.ser>`_. Accepted formats: ser (edam:format_2330).
         output_csv_path (str): Path to directory where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/correlation/inter_seqcorr_roll.csv>`_. Accepted formats: csv (edam:format_3752).
         output_jpg_path (str): Path to .jpg file where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/correlation/inter_seqcorr_roll.jpg>`_. Accepted formats: jpg (edam:format_3579).
         properties (dict):
             * **sequence** (*str*) - (None) Nucleic acid sequence for the input .ser file. Length of sequence is expected to be the same as the total number of columns in the .ser file, minus the index column (even if later on a subset of columns is selected with the *seqpos* option).
```

### Comparing `biobb_dna-4.1.0/biobb_dna/intrabp_correlations/intrabpcorr.py` & `biobb_dna-4.2.0/biobb_dna/intrabp_correlations/intrabpcorr.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from biobb_dna.utils import constants
 
 
 class IntraBasePairCorrelation(BiobbObject):
     """
     | biobb_dna IntraBasePairCorrelation
     | Calculate correlation between all intra-base pairs of a single sequence and for a single helical parameter.
+    | Calculate correlation between neighboring base pairs and pairs of helical parameters.
 
     Args:
         input_filename_shear (str): Path to .ser file with data for helical parameter 'shear'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/canal_output_shear.ser>`_. Accepted formats: ser (edam:format_2330).
         input_filename_stretch (str): Path to .ser file with data for helical parameter 'stretch'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/canal_output_stretch.ser>`_. Accepted formats: ser (edam:format_2330).
         input_filename_stagger (str): Path to .ser file with data for helical parameter 'stagger'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/canal_output_stagger.ser>`_. Accepted formats: ser (edam:format_2330).
         input_filename_buckle (str): Path to .ser file with data for helical parameter 'buckle'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/canal_output_buckle.ser>`_. Accepted formats: ser (edam:format_2330).
         input_filename_propel (str): Path to .ser file with data for helical parameter 'propel'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/canal_output_propel.ser>`_. Accepted formats: ser (edam:format_2330).
```

### Comparing `biobb_dna-4.1.0/biobb_dna/intrabp_correlations/intrahpcorr.py` & `biobb_dna-4.2.0/biobb_dna/intrabp_correlations/intrahpcorr.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from biobb_dna.utils.loader import load_data
 
 
 class IntraHelParCorrelation(BiobbObject):
     """
     | biobb_dna IntraHelParCorrelation
     | Calculate correlation between helical parameters for a single intra-base pair.
+    | Calculate correlation between helical parameters for a single intra-base pair.
 
     Args:
         input_filename_shear (str): Path to .csv file with data for helical parameter 'shear'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/series_shear_A.csv>`_. Accepted formats: csv (edam:format_3752).
         input_filename_stretch (str): Path to .csv file with data for helical parameter 'stretch'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/series_stretch_A.csv>`_. Accepted formats: csv (edam:format_3752).
         input_filename_stagger (str): Path to .csv file with data for helical parameter 'stagger'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/series_stagger_A.csv>`_. Accepted formats: csv (edam:format_3752).
         input_filename_buckle (str): Path to .csv file with data for helical parameter 'buckle'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/series_buckle_A.csv>`_. Accepted formats: csv (edam:format_3752).
         input_filename_propel (str): Path to .csv file with data for helical parameter 'propeller'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/series_propel_A.csv>`_. Accepted formats: csv (edam:format_3752).
```

### Comparing `biobb_dna-4.1.0/biobb_dna/intrabp_correlations/intraseqcorr.py` & `biobb_dna-4.2.0/biobb_dna/intrabp_correlations/intraseqcorr.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from biobb_dna.utils import constants
 
 
 class IntraSequenceCorrelation(BiobbObject):
     """
     | biobb_dna IntraSequenceCorrelation
     | Calculate correlation between all intra-base pairs of a single sequence and for a single helical parameter.
+    | Calculate correlation between all intra-base pairs of a single sequence and for a single helical parameter.
 
     Args:
         input_ser_path (str): Path to .ser file with data for single helical parameter. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/correlation/canal_output_buckle.ser>`_. Accepted formats: ser (edam:format_2330).
         output_csv_path (str): Path to directory where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/correlation/intra_seqcorr_buckle.csv>`_. Accepted formats: csv (edam:format_3752).
         output_jpg_path (str): Path to .jpg file where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/correlation/intra_seqcorr_buckle.jpg>`_. Accepted formats: jpg (edam:format_3579).
         properties (dict):
             * **sequence** (*str*) - (None) Nucleic acid sequence for the input .ser file. Length of sequence is expected to be the same as the total number of columns in the .ser file, minus the index column (even if later on a subset of columns is selected with the *seqpos* option).
```

### Comparing `biobb_dna-4.1.0/biobb_dna/stiffness/average_stiffness.py` & `biobb_dna-4.2.0/biobb_dna/stiffness/average_stiffness.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from biobb_common.configuration import settings
 
 
 class AverageStiffness(BiobbObject):
     """
     | biobb_dna AverageStiffness
     | Calculate average stiffness constants for each base pair of a trajectory's series.
+    | Calculate the average stiffness constants for each base pair of a trajectory's series. The input is a .ser file with the helical parameter values for each base/basepair. The output is a .csv file with the average stiffness constants for each base pair and a .jpg file with a plot of the average stiffness constants for each base pair.
 
     Args:
         input_ser_path (str): Path to .ser file for helical parameter. File is expected to be a table, with the first column being an index and the rest the helical parameter values for each base/basepair. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/stiffness/canal_output_roll.ser>`_. Accepted formats: ser (edam:format_2330).
         output_csv_path (str): Path to .csv file where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/stiffness/stiffavg_roll.csv>`_. Accepted formats: csv (edam:format_3752).
         output_jpg_path (str): Path to .jpg file where output is saved. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/reference/stiffness/stiffavg_roll.jpg>`_. Accepted formats: jpg (edam:format_3579).
         properties (dict):
             * **KT** (*float*) - (0.592186827) Value of Boltzmann temperature factor.
```

### Comparing `biobb_dna-4.1.0/biobb_dna/stiffness/basepair_stiffness.py` & `biobb_dna-4.2.0/biobb_dna/stiffness/basepair_stiffness.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from biobb_dna.utils.loader import load_data
 
 
 class BPStiffness(BiobbObject):
     """
     | biobb_dna BPStiffness
     | Calculate stiffness constants matrix between all six helical parameters for a single base pair step.
+    | Calculate stiffness constants matrix between all six helical parameters for a single base pair step.
 
     Args:
         input_filename_shift (str): Path to csv file with data for helical parameter 'shift'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/stiffness/series_shift_AA.csv>`_. Accepted formats: csv (edam:format_3752)
         input_filename_slide (str): Path to csv file with data for helical parameter 'slide'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/stiffness/series_slide_AA.csv>`_. Accepted formats: csv (edam:format_3752)
         input_filename_rise (str): Path to csv file with data for helical parameter 'rise'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/stiffness/series_rise_AA.csv>`_. Accepted formats: csv (edam:format_3752)
         input_filename_tilt (str): Path to csv file with data for helical parameter 'tilt'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/stiffness/series_tilt_AA.csv>`_. Accepted formats: csv (edam:format_3752)
         input_filename_roll (str): Path to csv file with data for helical parameter 'roll'. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_dna/master/biobb_dna/test/data/stiffness/series_roll_AA.csv>`_. Accepted formats: csv (edam:format_3752)
```

### Comparing `biobb_dna-4.1.0/biobb_dna/utils/constants.py` & `biobb_dna-4.2.0/biobb_dna/utils/constants.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-4.1.0/biobb_dna/utils/loader.py` & `biobb_dna-4.2.0/biobb_dna/utils/loader.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-4.1.0/biobb_dna.egg-info/PKG-INFO` & `biobb_dna-4.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
-Name: biobb-dna
-Version: 4.1.0
+Name: biobb_dna
+Version: 4.2.0
 Summary: Biobb_dna is a package composed of different analyses for nucleic acid trajectories.
 Home-page: https://github.com/bioexcel/biobb_dna
 Author: Biobb developers
 Author-email: lucia.fabio@irbbarcelona.com
-Project-URL: Documentation, http://biobb_dna.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-dna.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.2.0
+Requires-Dist: pandas>=1.3.0
+Requires-Dist: scikit-learn==0.24.2
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_dna?label=Version)](https://GitHub.com/bioexcel/biobb_dna/tags/)
 [![](https://img.shields.io/pypi/v/biobb-dna.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-dna/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_dna?label=Conda)](https://anaconda.org/bioconda/biobb_dna)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_dna?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_dna)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_dna?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_dna:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_dna:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_dna)
 [![](https://img.shields.io/pypi/pyversions/biobb-dna.svg?label=Python%20Versions)](https://pypi.org/project/biobb-dna/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_dna)
 
 [![](https://readthedocs.org/projects/biobb-dna/badge/?version=latest&label=Docs)](https://biobb-dna.readthedocs.io/en/latest/?badge=latest)
@@ -39,84 +42,91 @@
 
 [![](https://docs.bioexcel.eu/biobb_dna/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_dna/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_dna/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_dna/coverage/)
 [![](https://docs.bioexcel.eu/biobb_dna/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_dna/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_dna?label=Last%20Commit)](https://github.com/bioexcel/biobb_dna/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_dna.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_dna/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_dna
 
 ## Introduction
 Biobb_dna is a package composed of different analyses for 
 nucleic acid trajectories and helical parameters.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_dna.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-dna.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_dna>=4.1.0"
+        pip install "biobb_dna>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-dna.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_dna>=4.1.0"
+        conda install -c bioconda "biobb_dna>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-dna.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-dna.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_dna:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_dna:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_dna:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_dna:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_dna.sif https://depot.galaxyproject.org/singularity/biobb_dna:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_dna.sif https://depot.galaxyproject.org/singularity/biobb_dna:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_dna.sif <command>
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-dna.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_dna-4.1.0/biobb_dna.egg-info/SOURCES.txt` & `biobb_dna-4.2.0/biobb_dna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_dna-4.1.0/biobb_dna.egg-info/entry_points.txt` & `biobb_dna-4.2.0/biobb_dna.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_dna-4.1.0/setup.py` & `biobb_dna-4.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_dna",
-    version="4.1.0",
+    version="4.2.0",
     author="Biobb developers",
     author_email="lucia.fabio@irbbarcelona.com",
     description="Biobb_dna is a package composed of different analyses for nucleic acid trajectories.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_dna",
     project_urls={
-        "Documentation": "http://biobb_dna.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-dna.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['adapters', 'docs', 'test']),
     install_requires=[
-        'biobb_common==4.1.0',
+        'biobb_common==4.2.0',
         'pandas>=1.3.0',
         'scikit-learn==0.24.2'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "biobb_curves = biobb_dna.curvesplus.biobb_curves:main",
             "biobb_canal = biobb_dna.curvesplus.biobb_canal:main",
```

