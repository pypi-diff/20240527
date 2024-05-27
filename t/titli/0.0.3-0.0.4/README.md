# Comparing `tmp/titli-0.0.3.tar.gz` & `tmp/titli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titli-0.0.3.tar", last modified: Mon May 13 04:05:32 2024, max compression
+gzip compressed data, was "titli-0.0.4.tar", last modified: Mon May 27 11:10:21 2024, max compression
```

## Comparing `titli-0.0.3.tar` & `titli-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:32.617271 titli-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-13 04:05:26.000000 titli-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-13 04:05:32.617271 titli-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-13 04:05:26.000000 titli-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 04:05:32.617271 titli-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-13 04:05:26.000000 titli-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:32.613271 titli-0.0.3/titli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:26.000000 titli-0.0.3/titli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:32.617271 titli-0.0.3/titli/fe/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 04:05:26.000000 titli-0.0.3/titli/fe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23767 2024-05-13 04:05:26.000000 titli-0.0.3/titli/fe/after_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-13 04:05:26.000000 titli-0.0.3/titli/fe/base_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-13 04:05:26.000000 titli-0.0.3/titli/fe/corClust.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:32.617271 titli-0.0.3/titli/ids/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 04:05:26.000000 titli-0.0.3/titli/ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 04:05:26.000000 titli-0.0.3/titli/ids/base_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    17521 2024-05-13 04:05:26.000000 titli-0.0.3/titli/ids/kitsune.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-13 04:05:26.000000 titli-0.0.3/titli/ids/pytorch_kitsune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-13 04:05:26.000000 titli-0.0.3/titli/ids/torch_kitnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:32.617271 titli-0.0.3/titli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 04:05:26.000000 titli-0.0.3/titli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-13 04:05:26.000000 titli-0.0.3/titli/utils/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:32.617271 titli-0.0.3/titli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-13 04:05:32.000000 titli-0.0.3/titli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-13 04:05:32.000000 titli-0.0.3/titli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 04:05:32.000000 titli-0.0.3/titli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 04:05:32.000000 titli-0.0.3/titli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 04:05:32.000000 titli-0.0.3/titli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 04:05:32.000000 titli-0.0.3/titli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:10:21.585720 titli-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-27 11:10:15.000000 titli-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-27 11:10:21.585720 titli-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-27 11:10:15.000000 titli-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:10:21.585720 titli-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-27 11:10:15.000000 titli-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:10:21.581720 titli-0.0.4/titli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:10:15.000000 titli-0.0.4/titli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:10:21.585720 titli-0.0.4/titli/fe/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 11:10:15.000000 titli-0.0.4/titli/fe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23767 2024-05-27 11:10:15.000000 titli-0.0.4/titli/fe/after_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-27 11:10:15.000000 titli-0.0.4/titli/fe/base_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-27 11:10:15.000000 titli-0.0.4/titli/fe/corClust.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:10:21.585720 titli-0.0.4/titli/ids/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-27 11:10:15.000000 titli-0.0.4/titli/ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-27 11:10:15.000000 titli-0.0.4/titli/ids/base_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17521 2024-05-27 11:10:15.000000 titli-0.0.4/titli/ids/kitsune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-27 11:10:15.000000 titli-0.0.4/titli/ids/pytorch_kitsune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-27 11:10:15.000000 titli-0.0.4/titli/ids/torch_kitnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:10:21.585720 titli-0.0.4/titli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 11:10:15.000000 titli-0.0.4/titli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 11:10:15.000000 titli-0.0.4/titli/utils/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:10:21.585720 titli-0.0.4/titli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-27 11:10:21.000000 titli-0.0.4/titli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-27 11:10:21.000000 titli-0.0.4/titli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:10:21.000000 titli-0.0.4/titli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:10:21.000000 titli-0.0.4/titli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-27 11:10:21.000000 titli-0.0.4/titli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 11:10:21.000000 titli-0.0.4/titli.egg-info/top_level.txt
```

### Comparing `titli-0.0.3/LICENSE` & `titli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `titli-0.0.3/PKG-INFO` & `titli-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titli
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for collection of IDS and tools for evaluating them
 Home-page: https://github.com/spg-iitd/raids
 Author: Subrat Kumar Swain
 Author-email: mailofswainsubrat@gmail.com
 License: MIT
 Keywords: ids adversarial network nids
 Classifier: Programming Language :: Python :: 3
```

### Comparing `titli-0.0.3/README.md` & `titli-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `titli-0.0.3/setup.py` & `titli-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='titli',
-    version='0.0.3',
+    version='0.0.4',
     description='A library for collection of IDS and tools for evaluating them',
     long_description=open("README.md").read(),
     long_description_content_type = "text/markdown",
     url='https://github.com/spg-iitd/raids',
     packages=find_packages(),
     license='MIT',
     author="Subrat Kumar Swain",
```

### Comparing `titli-0.0.3/titli/fe/after_image.py` & `titli-0.0.4/titli/fe/after_image.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.3/titli/fe/base_feature_extractor.py` & `titli-0.0.4/titli/fe/base_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.3/titli/fe/corClust.py` & `titli-0.0.4/titli/fe/corClust.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.3/titli/ids/base_ids.py` & `titli-0.0.4/titli/ids/base_ids.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.3/titli/ids/kitsune.py` & `titli-0.0.4/titli/ids/kitsune.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.3/titli/ids/pytorch_kitsune.py` & `titli-0.0.4/titli/ids/pytorch_kitsune.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.3/titli/ids/torch_kitnet.py` & `titli-0.0.4/titli/ids/torch_kitnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,18 +88,18 @@
             self.norm_params = pickle.load(f)
 
     def forward(self, x):
         x = x.view(-1, self.input_dim)
 
         x_clusters = []
         for c in self.clusters:
-            norm_max = torch.tensor(self.norm_params[f"norm_max_{c[0]}"])
-            norm_min = torch.tensor(self.norm_params[f"norm_min_{c[0]}"])
+            norm_max = torch.tensor(self.norm_params[f"norm_max_{c[0]}"]).to(x.device)
+            norm_min = torch.tensor(self.norm_params[f"norm_min_{c[0]}"]).to(x.device)
 
-            x_cluster = torch.index_select(x, 1, torch.tensor(c))
+            x_cluster = torch.index_select(x, 1, torch.tensor(c).to(x.device))
             x_cluster = (x_cluster - norm_min) / (norm_max - norm_min + 0.0000000000000001)
             x_cluster = x_cluster.float()
 
             x_clusters.append(x_cluster)
 
         tail_losses = []
         for tail, c in zip(self.tails, x_clusters):
@@ -110,14 +110,15 @@
                 loss.data = torch.tensor(1e-2)
 
             tail_losses.append(loss)
 
         tails = torch.stack(tail_losses)
 
         # nomalize the tails
-        norm_max = torch.tensor(self.norm_params["norm_max_output"])
-        norm_min = torch.tensor(self.norm_params["norm_min_output"])
+        norm_max = torch.tensor(self.norm_params["norm_max_output"]).to(x.device)
+        norm_min = torch.tensor(self.norm_params["norm_min_output"]).to(x.device)
         tails = (tails - norm_min) / (norm_max - norm_min + 0.0000000000000001)
         tails = tails.float()
         x = self.head(tails)
 
         return x, tails
+
```

### Comparing `titli-0.0.3/titli.egg-info/PKG-INFO` & `titli-0.0.4/titli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titli
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for collection of IDS and tools for evaluating them
 Home-page: https://github.com/spg-iitd/raids
 Author: Subrat Kumar Swain
 Author-email: mailofswainsubrat@gmail.com
 License: MIT
 Keywords: ids adversarial network nids
 Classifier: Programming Language :: Python :: 3
```

