# Comparing `tmp/pyVMO-0.0.1.tar.gz` & `tmp/pyvmo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyVMO-0.0.1.tar", last modified: Fri Mar 22 19:29:04 2024, max compression
+gzip compressed data, was "pyvmo-0.0.4.tar", last modified: Mon May 27 21:32:31 2024, max compression
```

## Comparing `pyVMO-0.0.1.tar` & `pyvmo-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-03-22 19:29:04.000000 pyVMO-0.0.1/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2024-03-22 15:49:37.000000 pyVMO-0.0.1/LICENSE
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-03-22 16:01:38.000000 pyVMO-0.0.1/MANIFEST.in
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      477 2024-03-22 19:29:04.000000 pyVMO-0.0.1/PKG-INFO
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       56 2024-03-22 15:49:37.000000 pyVMO-0.0.1/README.md
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-03-22 19:29:04.000000 pyVMO-0.0.1/pyVMO.egg-info/
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      477 2024-03-22 19:29:04.000000 pyVMO-0.0.1/pyVMO.egg-info/PKG-INFO
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      315 2024-03-22 19:29:04.000000 pyVMO-0.0.1/pyVMO.egg-info/SOURCES.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2024-03-22 19:29:04.000000 pyVMO-0.0.1/pyVMO.egg-info/dependency_links.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       66 2024-03-22 19:29:04.000000 pyVMO-0.0.1/pyVMO.egg-info/requires.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        6 2024-03-22 19:29:04.000000 pyVMO-0.0.1/pyVMO.egg-info/top_level.txt
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-03-22 19:29:04.000000 pyVMO-0.0.1/pyvmo/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       26 2024-03-22 16:10:21.000000 pyVMO-0.0.1/pyvmo/__init__.py
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-03-22 19:29:04.000000 pyVMO-0.0.1/pyvmo/distance/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       91 2024-03-22 16:10:47.000000 pyVMO-0.0.1/pyvmo/distance/__init__.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     9662 2024-03-22 16:35:35.000000 pyVMO-0.0.1/pyvmo/distance/ibs.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     6497 2024-03-22 17:26:09.000000 pyVMO-0.0.1/pyvmo/format.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     6944 2024-03-22 16:53:34.000000 pyVMO-0.0.1/pyvmo/operation.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      500 2024-03-22 19:17:05.000000 pyVMO-0.0.1/pyvmo/versions.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     3189 2024-03-22 16:53:31.000000 pyVMO-0.0.1/pyvmo/vmo.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2024-03-22 19:29:04.000000 pyVMO-0.0.1/setup.cfg
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      809 2024-03-22 16:47:25.000000 pyVMO-0.0.1/setup.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-27 21:32:31.000000 pyvmo-0.0.4/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2024-05-21 19:42:01.000000 pyvmo-0.0.4/LICENSE
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-21 19:42:01.000000 pyvmo-0.0.4/MANIFEST.in
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2742 2024-05-27 21:32:31.000000 pyvmo-0.0.4/PKG-INFO
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2320 2024-05-27 21:30:06.000000 pyvmo-0.0.4/README.md
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2742 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/PKG-INFO
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      360 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       41 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/entry_points.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       66 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/requires.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        6 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/top_level.txt
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyvmo/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)       26 2024-05-21 19:42:01.000000 pyvmo-0.0.4/pyvmo/__init__.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     5665 2024-05-21 21:34:47.000000 pyvmo-0.0.4/pyvmo/cli.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyvmo/distance/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)       91 2024-05-21 19:42:01.000000 pyvmo-0.0.4/pyvmo/distance/__init__.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     9662 2024-05-21 19:42:01.000000 pyvmo-0.0.4/pyvmo/distance/ibs.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     7257 2024-05-27 21:25:34.000000 pyvmo-0.0.4/pyvmo/format.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     7007 2024-05-21 19:42:01.000000 pyvmo-0.0.4/pyvmo/operation.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      917 2024-05-27 21:03:17.000000 pyvmo-0.0.4/pyvmo/versions.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     3372 2024-05-21 19:42:01.000000 pyvmo-0.0.4/pyvmo/vmo.py
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2024-05-27 21:32:31.000000 pyvmo-0.0.4/setup.cfg
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      803 2024-05-21 21:06:24.000000 pyvmo-0.0.4/setup.py
```

### Comparing `pyVMO-0.0.1/LICENSE` & `pyvmo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyVMO-0.0.1/pyvmo/distance/ibs.py` & `pyvmo-0.0.4/pyvmo/distance/ibs.py`

 * *Files identical despite different names*

### Comparing `pyVMO-0.0.1/pyvmo/format.py` & `pyvmo-0.0.4/pyvmo/format.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from cyvcf2 import VCF
 from toolbiox.lib.common.os import mkdir, have_file
 from toolbiox.lib.common.util import pickle_dump
+from toolbiox.lib.common.sqlite_command import pickle_load_obj, pickle_dump_obj
 from pyvmo.operation import get_mis_ref_alt_num_parallel
 import allel
 import gc
 import h5py
 import numpy as np
 import pandas as pd
 import time
+import pickle
 
 
 def vcf_to_vmo(input_vcf_file, output_vmo, chunk_size=10000, force_update=False):
     mkdir(output_vmo.vmo_dir, False if force_update else True)
     log_file = "%s/store.log" % output_vmo.vmo_dir
 
     # Store vcf to hdf5
@@ -58,15 +60,15 @@
                         del memmap
                         gc.collect()
                         # dataset.read_direct(memmap, np.s_[row_slice, col_slice], np.s_[row_slice, col_slice])
                         block_parsed_num += 1
                         parsed_ratio = block_parsed_num/total_chunks*100
                         if parsed_ratio - last_printed_ratio >= 1:
                             logger_handle.write("%s: parsed %d blocks (%.2f%%)\n" % (time.strftime(
-                                "%Y-%m-%d %H:%M:%S", time.localtime()), block_parsed_num, block_parsed_num*chunk_size*chunk_size/len(rows)/len(columns)*100))
+                                "%Y-%m-%d %H:%M:%S", time.localtime()), block_parsed_num, parsed_ratio))
                             logger_handle.flush()
                             last_printed_ratio = parsed_ratio
 
     # Store memmap size
     if not have_file(output_vmo.memmap_size_file_path) or force_update:
         with h5py.File(output_vmo.info_store, 'r') as f:
             dataset = f['calldata/GT']
@@ -81,20 +83,37 @@
         with open(log_file, 'a') as logger_handle:
             vcf_reader = VCF(input_vcf_file)
             total_num = vcf_reader.num_records
             num = 0
             variants_list = []
             for variant in vcf_reader():
                 # variant
-                variants_list.append({
+                # variant_dict = {
+                #     'CHROM': variant.CHROM,
+                #     'POS': variant.POS,
+                #     'ID': variant.ID,
+                #     'REF': variant.REF,
+                #     'ALT': variant.ALT,
+                #     'QUAL': variant.QUAL,
+                #     'FILTER': variant.FILTERS,
+                #     'INFO': dict(variant.INFO)
+                # }                
+
+                variant_dict = {
                     'CHROM': variant.CHROM,
                     'POS': variant.POS,
+                    'ID': variant.ID,
                     'REF': variant.REF,
-                    'ALT': ','.join([str(a) for a in variant.ALT]),
-                })
+                    'ALT': pickle_dump_obj(variant.ALT),
+                    'QUAL': pickle_dump_obj(variant.QUAL),
+                    'FILTER': pickle_dump_obj(variant.FILTERS),
+                    'INFO': pickle_dump_obj(dict(variant.INFO))
+                }                
+
+                variants_list.append(variant_dict)                
 
                 num += 1
                 if num % 100000 == 0:
                     logger_handle.write("%s: read %d/%d variants (%.2f%%)\n" % (time.strftime(
                         "%Y-%m-%d %H:%M:%S", time.localtime()), num, total_num, num/total_num*100))
                     logger_handle.flush()
 
@@ -129,21 +148,21 @@
 
     with open(bimbam_file, 'w') as bimbam_handle:
 
         for i in range(m.shape[0]):
             chr_id = var_df.iloc[i]['CHROM']
             pos = int(var_df.iloc[i]['POS'])
             ref = var_df.iloc[i]['REF']
-            alt = var_df.iloc[i]['ALT']
+            alt = pickle_load_obj(var_df.iloc[i]['ALT'])[0]
 
             minor_allele = alt if ref_num[i] > alt_num[i] else ref
             major_allele = ref if ref_num[i] > alt_num[i] else alt
             major_allele_is_ref = ref_num[i] > alt_num[i]
 
-            var_id = "%s_%d_%s/%s" % (chr_id, pos, minor_allele, major_allele)
+            var_id = "%s_%d_%s/%s" % (chr_id, pos, ref, alt)
 
             bimbam_col_list = [var_id, minor_allele, major_allele] +  list(np.sum(m[i], axis=1) if major_allele_is_ref else  np.sum(np.abs(m[i] - 1),axis=1))
 
             bimbam_handle.write(",".join([str(i) for i in bimbam_col_list]) + "\n")
 
 
 if __name__ == "__main__":
```

### Comparing `pyVMO-0.0.1/pyvmo/operation.py` & `pyvmo-0.0.4/pyvmo/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from joblib import Parallel, delayed
-from toolbiox.lib.common.os import have_file
+from toolbiox.lib.common.os import have_file, mkdir
 from toolbiox.lib.common.util import pickle_dump
 import gc
 import h5py
 import numpy as np
 import pandas as pd
 import time
 
 # build submatrix
 
 
 def extract_sub_vmo(vmo, sub_vmo_dir, var_idx_list=None, spl_idx_list=None, chunk_size=10000, force_update=False):
+    mkdir(sub_vmo_dir, False if force_update else True)
 
     variants_info_store = "%s/variants_info_store.h5" % sub_vmo_dir
     samples_info_store = "%s/samples_info_store.h5" % sub_vmo_dir
     memmap_file_path = "%s/memmap.dat" % sub_vmo_dir
     memmap_size_file_path = "%s/memmap_size.pkl" % sub_vmo_dir
 
     log_file = "%s/store.log" % sub_vmo_dir
```

### Comparing `pyVMO-0.0.1/pyvmo/vmo.py` & `pyvmo-0.0.4/pyvmo/vmo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyvmo.format import vcf_to_vmo
+from pyvmo.format import vcf_to_vmo, vmo_to_bimbam
 from pyvmo.operation import extract_sub_vmo, get_valid_variant_index
 from toolbiox.lib.common.os import mkdir
 from toolbiox.lib.common.util import pickle_load
 import numpy as np
 import pandas as pd
 
 
@@ -49,14 +49,17 @@
     # site filter
     def site_filter(self, maf_thr=0.05, mis_thr=0.5, chunk_size=1000, n_jobs=8):
         m = self.get_matrix()
         valid_variant_bool_index = get_valid_variant_index(
             m, maf_thr=maf_thr, mis_thr=mis_thr, chunk_size=chunk_size, n_jobs=n_jobs)
         return np.where(valid_variant_bool_index)[0]
 
+    # convert to bimbam
+    def to_bimbam(self, bimbam_file, chunk_size=1000, n_jobs=8):
+        vmo_to_bimbam(self, bimbam_file, chunk_size=chunk_size, n_jobs=n_jobs)
 
 if __name__ == '__main__':
     vcf_file = "my_vcf_file"
     vmo_dir = "my_vmo_dir"
     sample_id_list = ["sample1", "sample2", "sample3"]
 
     # Store raw vcf to vmo, vcf to hdf5 about 5h (64618398, 1757, 2) and matrix to memmap about 45min
```

### Comparing `pyVMO-0.0.1/setup.py` & `pyvmo-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     author_email="xuyuxing@mail.kib.ac.cn",
     description="A test python toolkit for variant site analysis",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url="https://github.com/SouthernCD/pyVMO",
     include_package_data = True,
 
-    # entry_points={
-    #     "console_scripts": ["PyVMO = pyvmo.cli:main"]
-    # },    
+    entry_points={
+        "console_scripts": ["PyVMO = pyvmo.cli:main"]
+    },    
 
     packages=setuptools.find_packages(),
 
     install_requires=[
         "toolbiox>=0.0.44",
         "scikit-allel>=1.3.7",
         "cyvcf2>=0.30.28",
```

