# Comparing `tmp/pyfemtet-0.4.2.tar.gz` & `tmp/pyfemtet-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfemtet-0.4.2.tar", max compression
+gzip compressed data, was "pyfemtet-0.4.3.tar", max compression
```

## Comparing `pyfemtet-0.4.2.tar` & `pyfemtet-0.4.3.tar`

### file list

```diff
@@ -1,37 +1,70 @@
--rw-r--r--   0        0        0     1485 2024-05-13 11:07:43.197936 pyfemtet-0.4.2/LICENSE
--rw-r--r--   0        0        0      483 2024-05-13 11:07:43.197936 pyfemtet-0.4.2/README.md
--rw-r--r--   0        0        0   170268 2024-05-13 11:07:43.293937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.femprj
--rw-r--r--   0        0        0   226626 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.prt
--rw-r--r--   0        0        0     3980 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.py
--rw-r--r--   0        0        0    83094 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.SLDPRT
--rw-r--r--   0        0        0   155307 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.femprj
--rw-r--r--   0        0        0     4182 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.py
--rw-r--r--   0        0        0   268761 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/gau_ex08_parametric.femprj
--rw-r--r--   0        0        0     1799 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/gau_ex08_parametric.py
--rw-r--r--   0        0        0   126336 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/her_ex40_parametric.femprj
--rw-r--r--   0        0        0     5144 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/her_ex40_parametric.py
--rw-r--r--   0        0        0     2148 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/wat_ex14_parallel_parametric.py
--rw-r--r--   0        0        0   172895 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/wat_ex14_parametric.femprj
--rw-r--r--   0        0        0     2052 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/wat_ex14_parametric.py
--rw-r--r--   0        0        0       21 2024-05-13 11:07:55.278068 pyfemtet-0.4.2/pyfemtet/__init__.py
--rw-r--r--   0        0        0     1386 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/core.py
--rw-r--r--   0        0        0    16177 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/dispatch_extensions.py
--rw-r--r--   0        0        0     2507 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/logger.py
--rw-r--r--   0        0        0      596 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/__init__.py
--rw-r--r--   0        0        0    20602 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/_femopt.py
--rw-r--r--   0        0        0    24361 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/_femopt_core.py
--rw-r--r--   0        0        0      480 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/__init__.py
--rw-r--r--   0        0        0     2079 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/_base.py
--rw-r--r--   0        0        0    24439 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet.py
--rw-r--r--   0        0        0       83 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_nx/__init__.py
--rw-r--r--   0        0        0     4192 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_nx/_interface.py
--rw-r--r--   0        0        0     2856 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_nx/update_model.py
--rw-r--r--   0        0        0     6515 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_sldworks.py
--rw-r--r--   0        0        0      191 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/opt/__init__.py
--rw-r--r--   0        0        0     7101 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/opt/_base.py
--rw-r--r--   0        0        0     9996 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/opt/_optuna.py
--rw-r--r--   0        0        0      193 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/visualization/__init__.py
--rw-r--r--   0        0        0     5306 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/visualization/_graphs.py
--rw-r--r--   0        0        0    42104 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/visualization/_monitor.py
--rw-r--r--   0        0        0     1360 2024-05-13 11:07:55.278068 pyfemtet-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 pyfemtet-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1485 2024-05-27 03:03:35.288106 pyfemtet-0.4.3/LICENSE
+-rw-r--r--   0        0        0      483 2024-05-27 03:03:35.288106 pyfemtet-0.4.3/README.md
+-rw-r--r--   0        0        0   170268 2024-05-27 03:03:35.420107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.femprj
+-rw-r--r--   0        0        0   226626 2024-05-27 03:03:35.420107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.prt
+-rw-r--r--   0        0        0     3980 2024-05-27 03:03:35.420107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.py
+-rw-r--r--   0        0        0    83094 2024-05-27 03:03:35.420107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.SLDPRT
+-rw-r--r--   0        0        0   155307 2024-05-27 03:03:35.420107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.femprj
+-rw-r--r--   0        0        0     4182 2024-05-27 03:03:35.420107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.py
+-rw-r--r--   0        0        0     5144 2024-05-27 03:03:35.420107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/_her_ex40_parametric.py
+-rw-r--r--   0        0        0   268761 2024-05-27 03:03:35.420107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/gau_ex08_parametric.femprj
+-rw-r--r--   0        0        0     1799 2024-05-27 03:03:35.420107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/gau_ex08_parametric.py
+-rw-r--r--   0        0        0   126336 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/her_ex40_parametric.femprj
+-rw-r--r--   0        0        0     5144 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/her_ex40_parametric.py
+-rw-r--r--   0        0        0     2148 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/wat_ex14_parallel_parametric.py
+-rw-r--r--   0        0        0   172895 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/wat_ex14_parametric.femprj
+-rw-r--r--   0        0        0     2052 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/wat_ex14_parametric.py
+-rw-r--r--   0        0        0       21 2024-05-27 03:03:50.868228 pyfemtet-0.4.3/pyfemtet/__init__.py
+-rw-r--r--   0        0        0     1386 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/core.py
+-rw-r--r--   0        0        0    16177 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/dispatch_extensions.py
+-rw-r--r--   0        0        0     2507 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/logger.py
+-rw-r--r--   0        0        0      596 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/opt/__init__.py
+-rw-r--r--   0        0        0    20602 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/opt/_femopt.py
+-rw-r--r--   0        0        0    24361 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/opt/_femopt_core.py
+-rw-r--r--   0        0        0   149193 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/cad_ex01_NX.femprj
+-rw-r--r--   0        0        0   226626 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/cad_ex01_NX.prt
+-rw-r--r--   0        0        0     4519 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/cad_ex01_NX.py
+-rw-r--r--   0        0        0    97158 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/cad_ex01_SW.SLDPRT
+-rw-r--r--   0        0        0   126837 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/cad_ex01_SW.femprj
+-rw-r--r--   0        0        0     4586 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/cad_ex01_SW.py
+-rw-r--r--   0        0        0    72896 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/gal_ex58_parametric.femprj
+-rw-r--r--   0        0        0     2485 2024-05-27 03:03:35.424107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/gal_ex58_parametric.py
+-rw-r--r--   0        0        0   279251 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/gau_ex08_parametric.femprj
+-rw-r--r--   0        0        0     1956 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/gau_ex08_parametric.py
+-rw-r--r--   0        0        0   117221 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/her_ex40_parametric.femprj
+-rw-r--r--   0        0        0     4839 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/her_ex40_parametric.py
+-rw-r--r--   0        0        0   262283 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/paswat_ex1_parametric.femprj
+-rw-r--r--   0        0        0     2388 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/paswat_ex1_parametric.py
+-rw-r--r--   0        0        0     2499 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/paswat_ex1_parametric_parallel.py
+-rw-r--r--   0        0        0   179596 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/wat_ex14_parametric.femprj
+-rw-r--r--   0        0        0     2240 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample/wat_ex14_parametric.py
+-rw-r--r--   0        0        0   143533 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/cad_ex01_NX_jp.femprj
+-rw-r--r--   0        0        0     4797 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/cad_ex01_NX_jp.py
+-rw-r--r--   0        0        0   128026 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/cad_ex01_SW_jp.femprj
+-rw-r--r--   0        0        0     4864 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/cad_ex01_SW_jp.py
+-rw-r--r--   0        0        0    75668 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/gal_ex58_parametric_jp.femprj
+-rw-r--r--   0        0        0     2488 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/gal_ex58_parametric_jp.py
+-rw-r--r--   0        0        0   295600 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/gau_ex08_parametric_jp.femprj
+-rw-r--r--   0        0        0     2114 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/gau_ex08_parametric_jp.py
+-rw-r--r--   0        0        0   129783 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/her_ex40_parametric_jp.femprj
+-rw-r--r--   0        0        0     5272 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/her_ex40_parametric_jp.py
+-rw-r--r--   0        0        0   265368 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/paswat_ex1_parametric_jp.femprj
+-rw-r--r--   0        0        0     2516 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/paswat_ex1_parametric_jp.py
+-rw-r--r--   0        0        0     2632 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/paswat_ex1_parametric_parallel_jp.py
+-rw-r--r--   0        0        0   177944 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/wat_ex14_parametric_jp.femprj
+-rw-r--r--   0        0        0     2311 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/femprj_sample_jp/wat_ex14_parametric_jp.py
+-rw-r--r--   0        0        0      480 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/interface/__init__.py
+-rw-r--r--   0        0        0     2079 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/interface/_base.py
+-rw-r--r--   0        0        0    24754 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/interface/_femtet.py
+-rw-r--r--   0        0        0       83 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/interface/_femtet_with_nx/__init__.py
+-rw-r--r--   0        0        0     3931 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/interface/_femtet_with_nx/_interface.py
+-rw-r--r--   0        0        0     2856 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/interface/_femtet_with_nx/update_model.py
+-rw-r--r--   0        0        0     6254 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/interface/_femtet_with_sldworks.py
+-rw-r--r--   0        0        0      191 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/opt/__init__.py
+-rw-r--r--   0        0        0     7101 2024-05-27 03:03:35.428107 pyfemtet-0.4.3/pyfemtet/opt/opt/_base.py
+-rw-r--r--   0        0        0     9996 2024-05-27 03:03:35.432107 pyfemtet-0.4.3/pyfemtet/opt/opt/_optuna.py
+-rw-r--r--   0        0        0      193 2024-05-27 03:03:35.432107 pyfemtet-0.4.3/pyfemtet/opt/visualization/__init__.py
+-rw-r--r--   0        0        0     5306 2024-05-27 03:03:35.432107 pyfemtet-0.4.3/pyfemtet/opt/visualization/_graphs.py
+-rw-r--r--   0        0        0    42104 2024-05-27 03:03:35.432107 pyfemtet-0.4.3/pyfemtet/opt/visualization/_monitor.py
+-rw-r--r--   0        0        0     1360 2024-05-27 03:03:50.864228 pyfemtet-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 pyfemtet-0.4.3/PKG-INFO
```

### Comparing `pyfemtet-0.4.2/LICENSE` & `pyfemtet-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.femprj` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.femprj`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.prt` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.prt`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.py` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.SLDPRT` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.SLDPRT`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.femprj` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.femprj`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.py` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/gau_ex08_parametric.femprj` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/gau_ex08_parametric.femprj`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/gau_ex08_parametric.py` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/gau_ex08_parametric.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/her_ex40_parametric.femprj` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/her_ex40_parametric.femprj`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/her_ex40_parametric.py` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/_her_ex40_parametric.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/wat_ex14_parallel_parametric.py` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/wat_ex14_parallel_parametric.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/wat_ex14_parametric.femprj` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/wat_ex14_parametric.femprj`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/wat_ex14_parametric.py` & `pyfemtet-0.4.3/pyfemtet/FemtetPJTSample/wat_ex14_parametric.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/core.py` & `pyfemtet-0.4.3/pyfemtet/core.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/dispatch_extensions.py` & `pyfemtet-0.4.3/pyfemtet/dispatch_extensions.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/logger.py` & `pyfemtet-0.4.3/pyfemtet/logger.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/opt/__init__.py` & `pyfemtet-0.4.3/pyfemtet/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/opt/_femopt.py` & `pyfemtet-0.4.3/pyfemtet/opt/_femopt.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/opt/_femopt_core.py` & `pyfemtet-0.4.3/pyfemtet/opt/_femopt_core.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/opt/interface/_base.py` & `pyfemtet-0.4.3/pyfemtet/opt/interface/_base.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet.py` & `pyfemtet-0.4.3/pyfemtet/opt/interface/_femtet.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     def __init__(
             self,
             femprj_path=None,
             model_name=None,
             connect_method='auto',
             strictly_pid_specify=True,
             allow_without_project=False,
+            open_result_with_gui=True,
             **kwargs  # 継承されたクラスからの引数
     ):
 
         # win32com の初期化
         CoInitialize()
 
         # 引数の処理
@@ -70,14 +71,15 @@
             self.femprj_path = None
         else:
             self.femprj_path = os.path.abspath(femprj_path)
         self.model_name = model_name
         self.connect_method = connect_method
         self.allow_without_project = allow_without_project
         self.original_femprj_path = self.femprj_path
+        self.open_result_with_gui = open_result_with_gui
 
         # その他のメンバーの宣言や初期化
         self.Femtet = None
         self.femtet_pid = 0
         self.quit_when_destruct = False
         self.connected_method = 'unconnected'
         self.parameters = None
@@ -104,14 +106,15 @@
 
         # subprocess で restore するための情報保管
         # パスなどは connect_and_open_femtet での処理結果を反映し
         # メインで開いた解析モデルが確実に開かれるようにする
         super().__init__(
             femprj_path=self.femprj_path,
             model_name=self.model_name,
+            open_result_with_gui=self.open_result_with_gui,
             **kwargs
         )
 
     def __del__(self):
         if self.quit_when_destruct:
             try:
                 # 強制終了 TODO: 自動保存を回避する
@@ -555,21 +558,22 @@
         # 次に呼ばれるはずのユーザー定義コスト関数の記述を簡単にするため先に解析結果を開いておく
         self._call_femtet_api(
             self.Femtet.OpenCurrentResult,
             False,
             SolveError,  # 生きてるのに開けない場合
             error_message='解析結果のオープンに失敗しました',
             is_Gaudi_method=True,
-            args=(True,),
+            args=(self.open_result_with_gui,),
         )
 
     def update(self, parameters: 'pd.DataFrame') -> None:
         """See :func:`FEMInterface.update`"""
         self.parameters = parameters.copy()
         self.update_model(parameters)
+        # TODO: CAD 連携における座標を基にした境界条件の割当直しなどの処理をここに挟めるようにする
         self.solve()
 
     def quit(self, timeout=1, force=True):
         """Force to terminate connected Femtet."""
         util.close_femtet(self.Femtet.hWnd, timeout, force)
 
     def _setup_before_parallel(self, client):
```

### Comparing `pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_nx/_interface.py` & `pyfemtet-0.4.3/pyfemtet/opt/interface/_femtet_with_nx/_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,15 @@
     """
 
     _JOURNAL_PATH = os.path.abspath(os.path.join(here, 'update_model.py'))
 
     def __init__(
             self,
             prt_path,
-            femprj_path=None,
-            model_name=None,
-            connect_method='auto',
-            strictly_pid_specify=True,
+            **kwargs
     ):
 
         # check NX installation
         self.run_journal_path = os.path.join(os.environ.get('UGII_BASE_DIR'), 'NXBIN', 'run_journal.exe')
         if not os.path.isfile(self.run_journal_path):
             raise FileNotFoundError(
                 r'"%UGII_BASE_DIR%\NXBIN\run_journal.exe" が見つかりませんでした。環境変数 UGII_BASE_DIR 又は NX のインストール状態を確認してください。')
@@ -47,19 +44,16 @@
             self.prt_path = os.path.join(space, os.path.basename(prt_path))
         except ValueError:  # get_worker に失敗した場合
             self.prt_path = os.path.abspath(prt_path)
 
         # FemtetInterface の設定 (femprj_path, model_name の更新など)
         # + restore 情報の上書き
         super().__init__(
-            femprj_path=femprj_path,
-            model_name=model_name,
-            connect_method=connect_method,
-            strictly_pid_specify=strictly_pid_specify,
             prt_path=self.prt_path,
+            **kwargs
         )
 
     def check_param_value(self, name):
         """Override FemtetInterface.check_param_value().
 
         Do nothing because the parameter can be registered
         to not only .femprj but also .prt.
```

### Comparing `pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_nx/update_model.py` & `pyfemtet-0.4.3/pyfemtet/opt/interface/_femtet_with_nx/update_model.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_sldworks.py` & `pyfemtet-0.4.3/pyfemtet/opt/interface/_femtet_with_sldworks.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,36 +22,30 @@
     swSaveAsOptions_Silent = 1  # https://help.solidworks.com/2021/english/api/swconst/solidworks.interop.swconst~solidworks.interop.swconst.swsaveasoptions_e.html
     swSaveWithReferencesOptions_None = 0  # https://help-solidworks-com.translate.goog/2023/english/api/swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSaveWithReferencesOptions_e.html?_x_tr_sl=auto&_x_tr_tl=ja&_x_tr_hl=ja&_x_tr_pto=wapp
     swDocPART = 1  # https://help.solidworks.com/2023/english/api/swconst/SOLIDWORKS.Interop.swconst~SOLIDWORKS.Interop.swconst.swDocumentTypes_e.html
 
     def __init__(
             self,
             sldprt_path,
-            femprj_path=None,
-            model_name=None,
-            connect_method='auto',
-            strictly_pid_specify=True,
+            **kwargs
     ):
         # 引数の処理
         # dask サブプロセスのときは space 直下の sldprt_path を参照する
         try:
             worker = get_worker()
             space = worker.local_directory
             self.sldprt_path = os.path.join(space, os.path.basename(sldprt_path))
         except ValueError:  # get_worker に失敗した場合
             self.sldprt_path = os.path.abspath(sldprt_path)
 
         # FemtetInterface の設定 (femprj_path, model_name の更新など)
         # + restore 情報の上書き
         super().__init__(
-            femprj_path=femprj_path,
-            model_name=model_name,
-            connect_method=connect_method,
-            strictly_pid_specify=strictly_pid_specify,
             sldprt_path=self.sldprt_path,
+            **kwargs
         )
 
     def initialize_sldworks_connection(self):
         # SolidWorks を捕まえ、ファイルを開く
         self.swApp = DispatchEx('SLDWORKS.Application')
         self.swApp.Visible = True
```

### Comparing `pyfemtet-0.4.2/pyfemtet/opt/opt/_base.py` & `pyfemtet-0.4.3/pyfemtet/opt/opt/_base.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/opt/opt/_optuna.py` & `pyfemtet-0.4.3/pyfemtet/opt/opt/_optuna.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/opt/visualization/_graphs.py` & `pyfemtet-0.4.3/pyfemtet/opt/visualization/_graphs.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyfemtet/opt/visualization/_monitor.py` & `pyfemtet-0.4.3/pyfemtet/opt/visualization/_monitor.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.2/pyproject.toml` & `pyfemtet-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfemtet"
-version = "0.4.2"  # ignored by versioning plugin
+version = "0.4.3"  # ignored by versioning plugin
 description = "Design parameter optimization using Femtet."
 authors = ["kazuma.naito <kazuma.naito@murata.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/pyfemtet/pyfemtet"
 
 [tool.poetry.dependencies]
```

### Comparing `pyfemtet-0.4.2/PKG-INFO` & `pyfemtet-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfemtet
-Version: 0.4.2
+Version: 0.4.3
 Summary: Design parameter optimization using Femtet.
 Home-page: https://github.com/pyfemtet/pyfemtet
 License: BSD-3-Clause
 Author: kazuma.naito
 Author-email: kazuma.naito@murata.com
 Requires-Python: >=3.9.3,<3.13
 Classifier: License :: OSI Approved :: BSD License
```

