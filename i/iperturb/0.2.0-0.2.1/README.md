# Comparing `tmp/iperturb-0.2.0.tar.gz` & `tmp/iperturb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iperturb-0.2.0.tar", last modified: Mon May 27 04:32:01 2024, max compression
+gzip compressed data, was "iperturb-0.2.1.tar", last modified: Mon May 27 06:58:46 2024, max compression
```

## Comparing `iperturb-0.2.0.tar` & `iperturb-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 chenyz    (1659) chenyz    (1659)        0 2024-05-27 04:32:01.837911 iperturb-0.2.0/
--rw-r--r--   0 chenyz    (1659) chenyz    (1659)     2235 2024-05-27 04:32:01.836911 iperturb-0.2.0/PKG-INFO
--rw-rw-r--   0 chenyz    (1659) chenyz    (1659)     1459 2024-05-27 03:22:33.000000 iperturb-0.2.0/README.md
-drwxrwxr-x   0 chenyz    (1659) chenyz    (1659)        0 2024-05-27 04:32:01.835911 iperturb-0.2.0/iPerturb/
--rw-rw-r--   0 chenyz    (1659) chenyz    (1659)      126 2024-05-27 03:59:12.000000 iperturb-0.2.0/iPerturb/__init__.py
--rw-rw-r--   0 chenyz    (1659) chenyz    (1659)    17820 2024-05-27 03:11:28.000000 iperturb-0.2.0/iPerturb/model.py
--rw-rw-r--   0 chenyz    (1659) chenyz    (1659)    12529 2024-05-24 08:42:56.000000 iperturb-0.2.0/iPerturb/preprocess.py
--rw-rw-r--   0 chenyz    (1659) chenyz    (1659)     8084 2024-05-24 08:05:54.000000 iperturb-0.2.0/iPerturb/utils.py
-drwxrwxr-x   0 chenyz    (1659) chenyz    (1659)        0 2024-05-27 04:32:01.836911 iperturb-0.2.0/iperturb.egg-info/
--rw-r--r--   0 chenyz    (1659) chenyz    (1659)     2235 2024-05-27 04:32:01.000000 iperturb-0.2.0/iperturb.egg-info/PKG-INFO
--rw-rw-r--   0 chenyz    (1659) chenyz    (1659)      257 2024-05-27 04:32:01.000000 iperturb-0.2.0/iperturb.egg-info/SOURCES.txt
--rw-rw-r--   0 chenyz    (1659) chenyz    (1659)        1 2024-05-27 04:32:01.000000 iperturb-0.2.0/iperturb.egg-info/dependency_links.txt
--rw-rw-r--   0 chenyz    (1659) chenyz    (1659)      161 2024-05-27 04:32:01.000000 iperturb-0.2.0/iperturb.egg-info/requires.txt
--rw-rw-r--   0 chenyz    (1659) chenyz    (1659)        9 2024-05-27 04:32:01.000000 iperturb-0.2.0/iperturb.egg-info/top_level.txt
--rw-rw-r--   0 chenyz    (1659) chenyz    (1659)       38 2024-05-27 04:32:01.837911 iperturb-0.2.0/setup.cfg
--rw-rw-r--   0 chenyz    (1659) chenyz    (1659)      978 2024-05-27 04:31:53.000000 iperturb-0.2.0/setup.py
+drwxrwxr-x   0 chenyz    (1659) chenyz    (1659)        0 2024-05-27 06:58:46.806445 iperturb-0.2.1/
+-rw-r--r--   0 chenyz    (1659) chenyz    (1659)     2146 2024-05-27 06:58:46.806445 iperturb-0.2.1/PKG-INFO
+-rw-rw-r--   0 chenyz    (1659) chenyz    (1659)     1459 2024-05-27 03:22:33.000000 iperturb-0.2.1/README.md
+drwxrwxr-x   0 chenyz    (1659) chenyz    (1659)        0 2024-05-27 06:58:46.805445 iperturb-0.2.1/iPerturb/
+-rw-rw-r--   0 chenyz    (1659) chenyz    (1659)      126 2024-05-27 03:59:12.000000 iperturb-0.2.1/iPerturb/__init__.py
+-rw-rw-r--   0 chenyz    (1659) chenyz    (1659)    17820 2024-05-27 03:11:28.000000 iperturb-0.2.1/iPerturb/model.py
+-rw-rw-r--   0 chenyz    (1659) chenyz    (1659)    12529 2024-05-24 08:42:56.000000 iperturb-0.2.1/iPerturb/preprocess.py
+-rw-rw-r--   0 chenyz    (1659) chenyz    (1659)     8108 2024-05-27 06:18:42.000000 iperturb-0.2.1/iPerturb/utils.py
+drwxrwxr-x   0 chenyz    (1659) chenyz    (1659)        0 2024-05-27 06:58:46.805445 iperturb-0.2.1/iperturb.egg-info/
+-rw-r--r--   0 chenyz    (1659) chenyz    (1659)     2146 2024-05-27 06:58:46.000000 iperturb-0.2.1/iperturb.egg-info/PKG-INFO
+-rw-rw-r--   0 chenyz    (1659) chenyz    (1659)      257 2024-05-27 06:58:46.000000 iperturb-0.2.1/iperturb.egg-info/SOURCES.txt
+-rw-rw-r--   0 chenyz    (1659) chenyz    (1659)        1 2024-05-27 06:58:46.000000 iperturb-0.2.1/iperturb.egg-info/dependency_links.txt
+-rw-rw-r--   0 chenyz    (1659) chenyz    (1659)      102 2024-05-27 06:58:46.000000 iperturb-0.2.1/iperturb.egg-info/requires.txt
+-rw-rw-r--   0 chenyz    (1659) chenyz    (1659)        9 2024-05-27 06:58:46.000000 iperturb-0.2.1/iperturb.egg-info/top_level.txt
+-rw-rw-r--   0 chenyz    (1659) chenyz    (1659)       38 2024-05-27 06:58:46.806445 iperturb-0.2.1/setup.cfg
+-rw-rw-r--   0 chenyz    (1659) chenyz    (1659)      978 2024-05-27 06:58:03.000000 iperturb-0.2.1/setup.py
```

### Comparing `iperturb-0.2.0/PKG-INFO` & `iperturb-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: iperturb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Atlas-level data integration in multi-condition single-cell genomics
 Home-page: https://github.com/BillyChen123/iPerturb
 Author: Billy Chen
 Author-email: cyz2022@stu.xjtu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: anndata>=0.7.4
 Requires-Dist: numpy>=1.18.5
 Requires-Dist: pandas>=1.1.1
-Requires-Dist: pyro>=3.16
-Requires-Dist: pyro_ppl>=1.6.0
+Requires-Dist: pyro_ppl
 Requires-Dist: scanpy>=1.6.0
-Requires-Dist: scib>=1.1.5
-Requires-Dist: scikit_learn>=1.5.0
-Requires-Dist: scipy>=1.5.4
-Requires-Dist: setuptools>=50.1.0
-Requires-Dist: torch>=1.8.0
+Requires-Dist: scikit_learn
+Requires-Dist: scipy
+Requires-Dist: setuptools
+Requires-Dist: torch
 
 # iperturb
 
 iPerutrb使用变分自动编码器实现了人群规模单细胞数据的多条件整合。
 
 ## 安装
```

### Comparing `iperturb-0.2.0/README.md` & `iperturb-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `iperturb-0.2.0/iPerturb/model.py` & `iperturb-0.2.1/iPerturb/model.py`

 * *Files identical despite different names*

### Comparing `iperturb-0.2.0/iPerturb/preprocess.py` & `iperturb-0.2.1/iPerturb/preprocess.py`

 * *Files identical despite different names*

### Comparing `iperturb-0.2.0/iPerturb/utils.py` & `iperturb-0.2.1/iPerturb/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # setup environment
 import os
 smoke_test = ('CI' in os.environ)  # for continuous integration tests
 
 import torch
 import scanpy as sc
-from scib import me
+# from scib import me
 import pandas as pd
 import numpy as np
 import anndata as ad
 import scanpy as sc
 from sklearn.neighbors import NearestNeighbors
 
 def process_batch_X(datasets):
@@ -41,25 +41,25 @@
     num_batch = len(batch_labels)
 
     x_list_mean = [x.mean(axis=0) for x in x_list]
     x_list_scale = [x.std(axis=0) for x in x_list]
 
     return num_genes, num_batch, x_list_mean, x_list_scale
 
-def Find_ari(datasets):
-    ########### 这个函数用于寻找模型的最优聚类 ########### 
-    ari_max = -1
-    index_i = 0
-    for i in range(0,30):
-        sc.tl.louvain(datasets,resolution=i*0.01,key_added='seurat_clusters')
-        ari = me.ari(datasets,'groundtruth','seurat_clusters')
-        if ari>ari_max:
-            ari_max = ari
-            index_i = i
-    return ari_max,index_i
+# def Find_ari(datasets):
+#     ########### 这个函数用于寻找模型的最优聚类 ########### 
+#     ari_max = -1
+#     index_i = 0
+#     for i in range(0,30):
+#         sc.tl.louvain(datasets,resolution=i*0.01,key_added='seurat_clusters')
+#         ari = me.ari(datasets,'groundtruth','seurat_clusters')
+#         if ari>ari_max:
+#             ari_max = ari
+#             index_i = i
+#     return ari_max,index_i
 
 
 def construct_anndata(data,columns_names,index_names,raw):
     ########### 这个函数构建新的anndata用来进行下游分析 ########### 
     DATA = pd.DataFrame(data=data, columns=columns_names,index=index_names)
     datasets = sc.AnnData(DATA)
     datasets.obs['sample_id'] = DATA.index  # 添加样本 ID 列
```

### Comparing `iperturb-0.2.0/iperturb.egg-info/PKG-INFO` & `iperturb-0.2.1/iperturb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: iperturb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Atlas-level data integration in multi-condition single-cell genomics
 Home-page: https://github.com/BillyChen123/iPerturb
 Author: Billy Chen
 Author-email: cyz2022@stu.xjtu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: anndata>=0.7.4
 Requires-Dist: numpy>=1.18.5
 Requires-Dist: pandas>=1.1.1
-Requires-Dist: pyro>=3.16
-Requires-Dist: pyro_ppl>=1.6.0
+Requires-Dist: pyro_ppl
 Requires-Dist: scanpy>=1.6.0
-Requires-Dist: scib>=1.1.5
-Requires-Dist: scikit_learn>=1.5.0
-Requires-Dist: scipy>=1.5.4
-Requires-Dist: setuptools>=50.1.0
-Requires-Dist: torch>=1.8.0
+Requires-Dist: scikit_learn
+Requires-Dist: scipy
+Requires-Dist: setuptools
+Requires-Dist: torch
 
 # iperturb
 
 iPerutrb使用变分自动编码器实现了人群规模单细胞数据的多条件整合。
 
 ## 安装
```

### Comparing `iperturb-0.2.0/setup.py` & `iperturb-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read().splitlines()
 
 setup(
     name="iperturb",  # 包的名字
-    version="0.2.0",  # 初始版本
+    version="0.2.1",  # 初始版本
     author="Billy Chen",
     author_email="cyz2022@stu.xjtu.edu.cn",
     description="Atlas-level data integration in multi-condition single-cell genomics",  # 简短描述
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BillyChen123/iPerturb",  # 项目的主页
     packages=find_packages(),  # 自动找到包
```

