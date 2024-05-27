# Comparing `tmp/lightorch-0.0.1.tar.gz` & `tmp/lightorch-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightorch-0.0.1.tar", last modified: Mon May 27 16:22:53 2024, max compression
+gzip compressed data, was "lightorch-5.0.6.tar", last modified: Mon May 27 16:00:51 2024, max compression
```

## Comparing `lightorch-0.0.1.tar` & `lightorch-5.0.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:22:53.639920 lightorch-0.0.1/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1085 2024-05-27 15:34:53.000000 lightorch-0.0.1/LICENSE
--rw-r--r--   0 jenci     (1000) jenci     (1000)     2878 2024-05-27 16:22:53.639920 lightorch-0.0.1/PKG-INFO
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1421 2024-05-27 16:08:34.000000 lightorch-0.0.1/README.md
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:22:53.631920 lightorch-0.0.1/lightorch/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      208 2024-05-27 16:20:03.000000 lightorch-0.0.1/lightorch/__init__.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       76 2024-05-27 16:20:04.000000 lightorch-0.0.1/lightorch/_version.py
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:22:53.635920 lightorch-0.0.1/lightorch/default/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       71 2024-05-27 16:13:39.000000 lightorch-0.0.1/lightorch/default/__init__.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:13:38.000000 lightorch-0.0.1/lightorch/default/diffusion.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:13:37.000000 lightorch-0.0.1/lightorch/default/transformer.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     2912 2024-05-27 16:13:36.000000 lightorch-0.0.1/lightorch/default/vae.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)    16310 2024-05-27 16:06:54.000000 lightorch-0.0.1/lightorch/deprecated.py
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:22:53.635920 lightorch-0.0.1/lightorch/htuning/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       22 2024-05-27 15:42:31.000000 lightorch-0.0.1/lightorch/htuning/__init__.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     2800 2024-05-27 16:13:35.000000 lightorch-0.0.1/lightorch/htuning/optuna.py
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:22:53.635920 lightorch-0.0.1/lightorch/nn/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      161 2024-05-27 15:34:53.000000 lightorch-0.0.1/lightorch/nn/__init__.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      453 2024-05-27 15:54:13.000000 lightorch-0.0.1/lightorch/nn/complex.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     4360 2024-05-27 15:54:17.000000 lightorch-0.0.1/lightorch/nn/criterions.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1334 2024-05-27 15:54:21.000000 lightorch-0.0.1/lightorch/nn/dnn.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     4825 2024-05-27 16:14:05.000000 lightorch-0.0.1/lightorch/nn/fourier.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     4579 2024-05-27 15:54:40.000000 lightorch-0.0.1/lightorch/nn/functional.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      806 2024-05-27 15:54:41.000000 lightorch-0.0.1/lightorch/nn/kan.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      627 2024-05-27 16:13:34.000000 lightorch-0.0.1/lightorch/nn/monte_carlo.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      801 2024-05-27 16:13:34.000000 lightorch-0.0.1/lightorch/nn/normalization.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     3070 2024-05-27 15:54:53.000000 lightorch-0.0.1/lightorch/nn/partial.py
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:22:53.639920 lightorch-0.0.1/lightorch/nn/transformer/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       95 2024-05-27 15:54:11.000000 lightorch-0.0.1/lightorch/nn/transformer/__init__.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     8667 2024-05-27 15:55:05.000000 lightorch-0.0.1/lightorch/nn/transformer/attention.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     2243 2024-05-27 15:55:05.000000 lightorch-0.0.1/lightorch/nn/transformer/embedding.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     5858 2024-05-27 15:55:05.000000 lightorch-0.0.1/lightorch/nn/transformer/ffn.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     4414 2024-05-27 15:55:05.000000 lightorch-0.0.1/lightorch/nn/transformer/positional.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1180 2024-05-27 16:14:29.000000 lightorch-0.0.1/lightorch/nn/transformer/transformer.py
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:22:53.639920 lightorch-0.0.1/lightorch/training/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       53 2024-05-27 16:13:39.000000 lightorch-0.0.1/lightorch/training/__init__.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     4481 2024-05-27 16:13:33.000000 lightorch-0.0.1/lightorch/training/adversarial.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      524 2024-05-27 16:13:32.000000 lightorch-0.0.1/lightorch/training/cli.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     4615 2024-05-27 16:13:31.000000 lightorch-0.0.1/lightorch/training/supervised.py
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:22:53.639920 lightorch-0.0.1/lightorch.egg-info/
--rw-r--r--   0 jenci     (1000) jenci     (1000)     2878 2024-05-27 16:22:53.000000 lightorch-0.0.1/lightorch.egg-info/PKG-INFO
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1032 2024-05-27 16:22:53.000000 lightorch-0.0.1/lightorch.egg-info/SOURCES.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        1 2024-05-27 16:22:53.000000 lightorch-0.0.1/lightorch.egg-info/dependency_links.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       40 2024-05-27 16:22:53.000000 lightorch-0.0.1/lightorch.egg-info/requires.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       10 2024-05-27 16:22:53.000000 lightorch-0.0.1/lightorch.egg-info/top_level.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       38 2024-05-27 16:22:53.639920 lightorch-0.0.1/setup.cfg
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1870 2024-05-27 16:21:07.000000 lightorch-0.0.1/setup.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:00:51.522052 lightorch-5.0.6/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1085 2024-05-27 15:34:53.000000 lightorch-5.0.6/LICENSE
+-rw-r--r--   0 jenci     (1000) jenci     (1000)     2878 2024-05-27 16:00:51.522052 lightorch-5.0.6/PKG-INFO
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1421 2024-05-27 15:34:53.000000 lightorch-5.0.6/README.md
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:00:51.518052 lightorch-5.0.6/lightorch/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      207 2024-05-27 15:40:27.000000 lightorch-5.0.6/lightorch/__init__.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       76 2024-05-27 15:40:30.000000 lightorch-5.0.6/lightorch/_version.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:00:51.518052 lightorch-5.0.6/lightorch/default/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       71 2024-05-27 15:41:43.000000 lightorch-5.0.6/lightorch/default/__init__.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        0 2024-05-27 15:42:20.000000 lightorch-5.0.6/lightorch/default/diffusion.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        0 2024-05-27 15:42:20.000000 lightorch-5.0.6/lightorch/default/transformer.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     2912 2024-05-27 15:55:05.000000 lightorch-5.0.6/lightorch/default/vae.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)    16310 2024-05-27 15:40:36.000000 lightorch-5.0.6/lightorch/deprecated.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:00:51.518052 lightorch-5.0.6/lightorch/htuning/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       22 2024-05-27 15:42:31.000000 lightorch-5.0.6/lightorch/htuning/__init__.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     2800 2024-05-27 15:42:30.000000 lightorch-5.0.6/lightorch/htuning/optuna.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:00:51.522052 lightorch-5.0.6/lightorch/nn/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      161 2024-05-27 15:34:53.000000 lightorch-5.0.6/lightorch/nn/__init__.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      453 2024-05-27 15:54:13.000000 lightorch-5.0.6/lightorch/nn/complex.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     4360 2024-05-27 15:54:17.000000 lightorch-5.0.6/lightorch/nn/criterions.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1334 2024-05-27 15:54:21.000000 lightorch-5.0.6/lightorch/nn/dnn.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     4825 2024-05-27 15:54:23.000000 lightorch-5.0.6/lightorch/nn/fourier.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     4579 2024-05-27 15:54:40.000000 lightorch-5.0.6/lightorch/nn/functional.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      806 2024-05-27 15:54:41.000000 lightorch-5.0.6/lightorch/nn/kan.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      627 2024-05-27 15:43:58.000000 lightorch-5.0.6/lightorch/nn/monte_carlo.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      801 2024-05-27 15:43:59.000000 lightorch-5.0.6/lightorch/nn/normalization.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     3070 2024-05-27 15:54:53.000000 lightorch-5.0.6/lightorch/nn/partial.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:00:51.522052 lightorch-5.0.6/lightorch/nn/transformer/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       95 2024-05-27 15:54:11.000000 lightorch-5.0.6/lightorch/nn/transformer/__init__.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     8667 2024-05-27 15:55:05.000000 lightorch-5.0.6/lightorch/nn/transformer/attention.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     2243 2024-05-27 15:55:05.000000 lightorch-5.0.6/lightorch/nn/transformer/embedding.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     5858 2024-05-27 15:55:05.000000 lightorch-5.0.6/lightorch/nn/transformer/ffn.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     4414 2024-05-27 15:55:05.000000 lightorch-5.0.6/lightorch/nn/transformer/positional.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1105 2024-05-27 15:55:05.000000 lightorch-5.0.6/lightorch/nn/transformer/transformer.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:00:51.522052 lightorch-5.0.6/lightorch/training/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       53 2024-05-27 15:40:15.000000 lightorch-5.0.6/lightorch/training/__init__.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     4481 2024-05-27 15:40:19.000000 lightorch-5.0.6/lightorch/training/adversarial.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      524 2024-05-27 15:44:04.000000 lightorch-5.0.6/lightorch/training/cli.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     4615 2024-05-27 15:44:06.000000 lightorch-5.0.6/lightorch/training/supervised.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-05-27 16:00:51.522052 lightorch-5.0.6/lightorch.egg-info/
+-rw-r--r--   0 jenci     (1000) jenci     (1000)     2878 2024-05-27 16:00:51.000000 lightorch-5.0.6/lightorch.egg-info/PKG-INFO
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1032 2024-05-27 16:00:51.000000 lightorch-5.0.6/lightorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        1 2024-05-27 16:00:51.000000 lightorch-5.0.6/lightorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       40 2024-05-27 16:00:51.000000 lightorch-5.0.6/lightorch.egg-info/requires.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       10 2024-05-27 16:00:51.000000 lightorch-5.0.6/lightorch.egg-info/top_level.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       38 2024-05-27 16:00:51.522052 lightorch-5.0.6/setup.cfg
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1870 2024-05-27 16:00:15.000000 lightorch-5.0.6/setup.py
```

### Comparing `lightorch-0.0.1/LICENSE` & `lightorch-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/PKG-INFO` & `lightorch-5.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightorch
-Version: 0.0.1
+Version: 5.0.6
 Summary: Pytorch & Lightning based framework for research and ml-pipeline automation.
 Home-page: https://github.com/Jorgedavyd/lightorch
 Author: Jorge David Enciso Martínez
 Author-email: jorged.encyso@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `lightorch-0.0.1/README.md` & `lightorch-5.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/default/vae.py` & `lightorch-5.0.6/lightorch/default/vae.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/deprecated.py` & `lightorch-5.0.6/lightorch/deprecated.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/htuning/optuna.py` & `lightorch-5.0.6/lightorch/htuning/optuna.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/criterions.py` & `lightorch-5.0.6/lightorch/nn/criterions.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/dnn.py` & `lightorch-5.0.6/lightorch/nn/dnn.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/fourier.py` & `lightorch-5.0.6/lightorch/nn/fourier.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/functional.py` & `lightorch-5.0.6/lightorch/nn/functional.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/kan.py` & `lightorch-5.0.6/lightorch/nn/kan.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/monte_carlo.py` & `lightorch-5.0.6/lightorch/nn/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/normalization.py` & `lightorch-5.0.6/lightorch/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/partial.py` & `lightorch-5.0.6/lightorch/nn/partial.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/transformer/attention.py` & `lightorch-5.0.6/lightorch/nn/transformer/attention.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/transformer/embedding.py` & `lightorch-5.0.6/lightorch/nn/transformer/embedding.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/transformer/ffn.py` & `lightorch-5.0.6/lightorch/nn/transformer/ffn.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/transformer/positional.py` & `lightorch-5.0.6/lightorch/nn/transformer/positional.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/nn/transformer/transformer.py` & `lightorch-5.0.6/lightorch/nn/transformer/transformer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,42 @@
+"""INCLUDE ARCH FOR GENERAL"""
+
 from torch import nn, Tensor
 from typing import Optional, List
 
+
 class GeneralTransformer(nn.Module):
-    def __init__(self, *, encoder: Optional[nn.Module], decoder: Optional[nn.Module], n_layers: int) -> None:
+    def __init__(
+        self,
+        *,
+        encoder: Optional[nn.Module],
+        decoder: Optional[nn.Module],
+        n_layers: int
+    ) -> None:
         super().__init__()
         if encoder is not None:
 
-            self.encoders = nn.Sequential(
-                *[
-                    encoder for _ in range(n_layers)
-                ]
-            )
+            self.encoders = nn.Sequential(*[encoder for _ in range(n_layers)])
         else:
             self.encoders = False
 
         if decoder is not None:
-            self.decoders = nn.Sequential(
-                *[
-                    decoder for _ in range(n_layers)
-                ]
-            )
+            self.decoders = nn.Sequential(*[decoder for _ in range(n_layers)])
         else:
             self.decoders = False
+
     def encoder_forward(self, x: Tensor) -> Tensor:
         hist: List[nn.Module] = []
         for module in self.encoders:
             x = module(x)
             hist.append(x)
         return hist
+
     def forward(self, x: Tensor) -> Tensor:
         if self.encoders:
             hist = self.encoder_forward(x)
         # Continue
-            
-        
+
 
 class CrossTransformer(nn.Module):
     def __init__(self, encoder: nn.Module, decoder: nn.Module, n_layers: int) -> None:
-        pass
+        pass
```

### Comparing `lightorch-0.0.1/lightorch/training/adversarial.py` & `lightorch-5.0.6/lightorch/training/adversarial.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/training/cli.py` & `lightorch-5.0.6/lightorch/training/cli.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch/training/supervised.py` & `lightorch-5.0.6/lightorch/training/supervised.py`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/lightorch.egg-info/PKG-INFO` & `lightorch-5.0.6/lightorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightorch
-Version: 0.0.1
+Version: 5.0.6
 Summary: Pytorch & Lightning based framework for research and ml-pipeline automation.
 Home-page: https://github.com/Jorgedavyd/lightorch
 Author: Jorge David Enciso Martínez
 Author-email: jorged.encyso@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `lightorch-0.0.1/lightorch.egg-info/SOURCES.txt` & `lightorch-5.0.6/lightorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightorch-0.0.1/setup.py` & `lightorch-5.0.6/setup.py`

 * *Files identical despite different names*

