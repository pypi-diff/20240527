# Comparing `tmp/ms1searchpy-2.8.3-py3-none-any.whl.zip` & `tmp/ms1searchpy-2.8.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 8559168 bytes, number of entries: 18
+Zip file size: 8565293 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-16 13:01 ms1searchpy/__init__.py
 -rw-r--r--  2.0 unx     4236 b- defN 24-Apr-24 10:36 ms1searchpy/combine.py
 -rw-r--r--  2.0 unx     2746 b- defN 23-Mar-16 13:01 ms1searchpy/combine_proteins.py
 -rw-r--r--  2.0 unx    24852 b- defN 24-May-21 13:28 ms1searchpy/directms1quant.py
--rw-r--r--  2.0 unx    16454 b- defN 24-May-24 10:37 ms1searchpy/directms1quantmulti.py
+-rw-r--r--  2.0 unx    27663 b- defN 24-May-27 12:17 ms1searchpy/directms1quantDIA.py
+-rw-r--r--  2.0 unx    16465 b- defN 24-May-27 12:17 ms1searchpy/directms1quantmulti.py
 -rw-r--r--  2.0 unx     7218 b- defN 24-May-14 13:38 ms1searchpy/group_specific.py
 -rw-r--r--  2.0 unx    84411 b- defN 24-May-16 15:08 ms1searchpy/main.py
 -rw-r--r--  2.0 unx     7413 b- defN 23-Mar-16 13:01 ms1searchpy/ms1todiffacto.py
 -rw-r--r--  2.0 unx     5074 b- defN 24-Mar-14 15:01 ms1searchpy/search.py
 -rw-r--r--  2.0 unx    14862 b- defN 24-Jan-26 14:14 ms1searchpy/utils.py
 -rw-r--r--  2.0 unx    15305 b- defN 24-Mar-14 15:25 ms1searchpy/utils_figures.py
 -rw-r--r--  2.0 unx  9177032 b- defN 24-Jan-15 09:44 ms1searchpy/models/CSD_model_LCMSMS.hdf5
--rwxr-xr-x  2.0 unx      551 b- defN 24-May-24 10:39 ms1searchpy-2.8.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     8733 b- defN 24-May-24 10:39 ms1searchpy-2.8.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 10:39 ms1searchpy-2.8.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      492 b- defN 24-May-24 10:39 ms1searchpy-2.8.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-May-24 10:39 ms1searchpy-2.8.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1518 b- defN 24-May-24 10:39 ms1searchpy-2.8.3.dist-info/RECORD
-18 files, 9371001 bytes uncompressed, 8556684 bytes compressed:  8.7%
+-rwxr-xr-x  2.0 unx      551 b- defN 24-May-27 13:17 ms1searchpy-2.8.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8733 b- defN 24-May-27 13:17 ms1searchpy-2.8.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-27 13:17 ms1searchpy-2.8.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx      492 b- defN 24-May-27 13:17 ms1searchpy-2.8.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-27 13:17 ms1searchpy-2.8.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1608 b- defN 24-May-27 13:17 ms1searchpy-2.8.4.dist-info/RECORD
+19 files, 9398765 bytes uncompressed, 8562669 bytes compressed:  8.9%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: ms1searchpy/combine_proteins.py
 Comment: 
 
 Filename: ms1searchpy/directms1quant.py
 Comment: 
 
+Filename: ms1searchpy/directms1quantDIA.py
+Comment: 
+
 Filename: ms1searchpy/directms1quantmulti.py
 Comment: 
 
 Filename: ms1searchpy/group_specific.py
 Comment: 
 
 Filename: ms1searchpy/main.py
@@ -30,26 +33,26 @@
 
 Filename: ms1searchpy/utils_figures.py
 Comment: 
 
 Filename: ms1searchpy/models/CSD_model_LCMSMS.hdf5
 Comment: 
 
-Filename: ms1searchpy-2.8.3.dist-info/LICENSE
+Filename: ms1searchpy-2.8.4.dist-info/LICENSE
 Comment: 
 
-Filename: ms1searchpy-2.8.3.dist-info/METADATA
+Filename: ms1searchpy-2.8.4.dist-info/METADATA
 Comment: 
 
-Filename: ms1searchpy-2.8.3.dist-info/WHEEL
+Filename: ms1searchpy-2.8.4.dist-info/WHEEL
 Comment: 
 
-Filename: ms1searchpy-2.8.3.dist-info/entry_points.txt
+Filename: ms1searchpy-2.8.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ms1searchpy-2.8.3.dist-info/top_level.txt
+Filename: ms1searchpy-2.8.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ms1searchpy-2.8.3.dist-info/RECORD
+Filename: ms1searchpy-2.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ms1searchpy/directms1quantmulti.py

```diff
@@ -50,15 +50,15 @@
 
 def process_files(args):
 
     infolder = args['pdir']
     ms1folder = args['pdir']
     path_to_fasta = args['d']
 
-    df1 = pd.read_table(args['samples'], dtype={'group': str, 'condition': str})
+    df1 = pd.read_table(args['samples'], dtype={'group': str, 'condition': str, 'vs': str})
     df1['sample'] = df1['group']
     if 'condition' not in df1.columns:
         df1['condition'] = ''
         
     if 'replicate' not in df1.columns:
         df1['replicate'] = 1
```

## Comparing `ms1searchpy-2.8.3.dist-info/LICENSE` & `ms1searchpy-2.8.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ms1searchpy-2.8.3.dist-info/METADATA` & `ms1searchpy-2.8.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms1searchpy
-Version: 2.8.3
+Version: 2.8.4
 Summary: A proteomics search engine for LC-MS1 spectra.
 Author: Mark Ivanov
 Author-email: pyteomics@googlegroups.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Education
```

## Comparing `ms1searchpy-2.8.3.dist-info/RECORD` & `ms1searchpy-2.8.4.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 ms1searchpy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ms1searchpy/combine.py,sha256=7S61Ftnv4NJUmfnV6vjVp2uHwslkDcQQJVPzWYVm1nk,4236
 ms1searchpy/combine_proteins.py,sha256=LFJuwkb8UBy-1T-kAT3H4zxkqQ6VTso6SOLP7s8o0Ow,2746
 ms1searchpy/directms1quant.py,sha256=OuInuVdPCIsRbvRSCM1mnNqh0jQwvQhhcd6Bo0AbnnM,24852
-ms1searchpy/directms1quantmulti.py,sha256=x6iFcoUt2bI-8x1Z6vLpBpxz6lUBli01bcSoB3jfkhw,16454
+ms1searchpy/directms1quantDIA.py,sha256=Nsc-761aWMIFYlqOIlruQ3arQp3FU_WYI4clsKDmZ9s,27663
+ms1searchpy/directms1quantmulti.py,sha256=Sf7AI_pyM_jqDfzjgGJMyHyqcndqUbFFT_PJcL0OJ1c,16465
 ms1searchpy/group_specific.py,sha256=AqEN5xkrsEdXeVFdqHUkQa0tmip14zQQrK4pu0tFZi4,7218
 ms1searchpy/main.py,sha256=Gj3VqOO46Pu2CGVZiOu2fdj8KyppxEVD5bJBbUwY2Os,84411
 ms1searchpy/ms1todiffacto.py,sha256=xGxcIe8-C_vSLx5Qz5qwSKa4oULJ-8cgq4DtCTXKe3s,7413
 ms1searchpy/search.py,sha256=LzcFU_j7pilzoHo-4b_D0gkMXGwruWt4G5vluWPa-Qk,5074
 ms1searchpy/utils.py,sha256=D59l42xbMYMyL6GEuKOCOPsdexaMmo-1j3cKSNPN9lE,14862
 ms1searchpy/utils_figures.py,sha256=KfBAVLoq7U57HV-hct8CpiOL4BCHADAWIBFbH-jWB_M,15305
 ms1searchpy/models/CSD_model_LCMSMS.hdf5,sha256=7nAu3-YWKjsuQNCpgoRpTjInA-dPe7kZE1pTGKg-3OQ,9177032
-ms1searchpy-2.8.3.dist-info/LICENSE,sha256=WanbJHdVmtsm-QgIuB0GDMrtkwBHY6WmTzwvX6ZZtgs,551
-ms1searchpy-2.8.3.dist-info/METADATA,sha256=5XTJiMar_D4nb1TuvLMiZ5FBXx58-7eHM8K91GRqsoE,8733
-ms1searchpy-2.8.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ms1searchpy-2.8.3.dist-info/entry_points.txt,sha256=ACLj6QbnpM9wI-CQA2YFf_ZmWEFqN9GZpbuxO6ZEeHE,492
-ms1searchpy-2.8.3.dist-info/top_level.txt,sha256=pyjbWV_odwavqf6q4mSj2P0L0zLqKEDftX53QvxeJlc,12
-ms1searchpy-2.8.3.dist-info/RECORD,,
+ms1searchpy-2.8.4.dist-info/LICENSE,sha256=WanbJHdVmtsm-QgIuB0GDMrtkwBHY6WmTzwvX6ZZtgs,551
+ms1searchpy-2.8.4.dist-info/METADATA,sha256=Yp86CdWaC56pg3AuIWv4dSstYT3i7a5JqrrzYdTjjZY,8733
+ms1searchpy-2.8.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ms1searchpy-2.8.4.dist-info/entry_points.txt,sha256=ACLj6QbnpM9wI-CQA2YFf_ZmWEFqN9GZpbuxO6ZEeHE,492
+ms1searchpy-2.8.4.dist-info/top_level.txt,sha256=pyjbWV_odwavqf6q4mSj2P0L0zLqKEDftX53QvxeJlc,12
+ms1searchpy-2.8.4.dist-info/RECORD,,
```

