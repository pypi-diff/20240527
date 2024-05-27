# Comparing `tmp/mdgrad-0.1.tar.gz` & `tmp/mdgrad-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdgrad-0.1.tar", last modified: Sun May 26 16:46:35 2024, max compression
+gzip compressed data, was "mdgrad-0.2.tar", last modified: Mon May 27 21:40:01 2024, max compression
```

## Comparing `mdgrad-0.1.tar` & `mdgrad-0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-26 16:46:35.908918 mdgrad-0.1/
--rw-r--r--   0 neddamj    (501) staff       (20)     1070 2024-05-23 16:47:17.000000 mdgrad-0.1/LICENSE
--rw-r--r--   0 neddamj    (501) staff       (20)     1933 2024-05-26 16:46:35.908524 mdgrad-0.1/PKG-INFO
--rw-r--r--   0 neddamj    (501) staff       (20)     1288 2024-05-26 16:44:42.000000 mdgrad-0.1/README.md
-drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-26 16:46:35.904243 mdgrad-0.1/mdgrad/
--rw-r--r--   0 neddamj    (501) staff       (20)       27 2024-05-26 16:43:33.000000 mdgrad-0.1/mdgrad/__init__.py
-drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-26 16:46:35.907256 mdgrad-0.1/mdgrad/nn/
--rw-r--r--   0 neddamj    (501) staff       (20)       70 2024-05-24 19:34:32.000000 mdgrad-0.1/mdgrad/nn/__init__.py
--rw-r--r--   0 neddamj    (501) staff       (20)      643 2024-05-26 16:43:14.000000 mdgrad-0.1/mdgrad/nn/activations.py
--rw-r--r--   0 neddamj    (501) staff       (20)     1914 2024-05-26 16:43:14.000000 mdgrad-0.1/mdgrad/nn/layers.py
--rw-r--r--   0 neddamj    (501) staff       (20)      781 2024-05-26 16:43:19.000000 mdgrad-0.1/mdgrad/nn/losses.py
--rw-r--r--   0 neddamj    (501) staff       (20)      633 2024-05-26 16:43:23.000000 mdgrad-0.1/mdgrad/nn/optim.py
--rw-r--r--   0 neddamj    (501) staff       (20)    10002 2024-05-26 16:16:39.000000 mdgrad-0.1/mdgrad/tensor.py
-drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-26 16:46:35.907955 mdgrad-0.1/mdgrad.egg-info/
--rw-r--r--   0 neddamj    (501) staff       (20)     1933 2024-05-26 16:46:35.000000 mdgrad-0.1/mdgrad.egg-info/PKG-INFO
--rw-r--r--   0 neddamj    (501) staff       (20)      317 2024-05-26 16:46:35.000000 mdgrad-0.1/mdgrad.egg-info/SOURCES.txt
--rw-r--r--   0 neddamj    (501) staff       (20)        1 2024-05-26 16:46:35.000000 mdgrad-0.1/mdgrad.egg-info/dependency_links.txt
--rw-r--r--   0 neddamj    (501) staff       (20)        6 2024-05-26 16:46:35.000000 mdgrad-0.1/mdgrad.egg-info/requires.txt
--rw-r--r--   0 neddamj    (501) staff       (20)        7 2024-05-26 16:46:35.000000 mdgrad-0.1/mdgrad.egg-info/top_level.txt
--rw-r--r--   0 neddamj    (501) staff       (20)       38 2024-05-26 16:46:35.908996 mdgrad-0.1/setup.cfg
--rw-r--r--   0 neddamj    (501) staff       (20)     2200 2024-05-26 16:45:42.000000 mdgrad-0.1/setup.py
+drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-27 21:40:01.529102 mdgrad-0.2/
+-rw-r--r--   0 neddamj    (501) staff       (20)     1070 2024-05-23 16:47:17.000000 mdgrad-0.2/LICENSE
+-rw-r--r--   0 neddamj    (501) staff       (20)     1962 2024-05-27 21:40:01.528843 mdgrad-0.2/PKG-INFO
+-rw-r--r--   0 neddamj    (501) staff       (20)     1288 2024-05-26 16:44:42.000000 mdgrad-0.2/README.md
+drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-27 21:40:01.524723 mdgrad-0.2/mdgrad/
+-rw-r--r--   0 neddamj    (501) staff       (20)       27 2024-05-27 21:31:43.000000 mdgrad-0.2/mdgrad/__init__.py
+drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-27 21:40:01.528162 mdgrad-0.2/mdgrad/nn/
+-rw-r--r--   0 neddamj    (501) staff       (20)       70 2024-05-27 21:22:14.000000 mdgrad-0.2/mdgrad/nn/__init__.py
+-rw-r--r--   0 neddamj    (501) staff       (20)      643 2024-05-26 16:43:14.000000 mdgrad-0.2/mdgrad/nn/activations.py
+-rw-r--r--   0 neddamj    (501) staff       (20)     1952 2024-05-26 18:31:40.000000 mdgrad-0.2/mdgrad/nn/layers.py
+-rw-r--r--   0 neddamj    (501) staff       (20)     1636 2024-05-27 21:03:19.000000 mdgrad-0.2/mdgrad/nn/losses.py
+-rw-r--r--   0 neddamj    (501) staff       (20)      573 2024-05-27 21:31:27.000000 mdgrad-0.2/mdgrad/optim.py
+-rw-r--r--   0 neddamj    (501) staff       (20)    10168 2024-05-27 21:19:31.000000 mdgrad-0.2/mdgrad/tensor.py
+drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-27 21:40:01.528463 mdgrad-0.2/mdgrad.egg-info/
+-rw-r--r--   0 neddamj    (501) staff       (20)     1962 2024-05-27 21:40:01.000000 mdgrad-0.2/mdgrad.egg-info/PKG-INFO
+-rw-r--r--   0 neddamj    (501) staff       (20)      314 2024-05-27 21:40:01.000000 mdgrad-0.2/mdgrad.egg-info/SOURCES.txt
+-rw-r--r--   0 neddamj    (501) staff       (20)        1 2024-05-27 21:40:01.000000 mdgrad-0.2/mdgrad.egg-info/dependency_links.txt
+-rw-r--r--   0 neddamj    (501) staff       (20)        6 2024-05-27 21:40:01.000000 mdgrad-0.2/mdgrad.egg-info/requires.txt
+-rw-r--r--   0 neddamj    (501) staff       (20)        7 2024-05-27 21:40:01.000000 mdgrad-0.2/mdgrad.egg-info/top_level.txt
+-rw-r--r--   0 neddamj    (501) staff       (20)       38 2024-05-27 21:40:01.529153 mdgrad-0.2/setup.cfg
+-rw-r--r--   0 neddamj    (501) staff       (20)     2229 2024-05-27 21:39:34.000000 mdgrad-0.2/setup.py
```

### Comparing `mdgrad-0.1/LICENSE` & `mdgrad-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdgrad-0.1/PKG-INFO` & `mdgrad-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdgrad
-Version: 0.1
+Version: 0.2
 Summary: Tensor-based autdiff engine and neural network API
 Author: Jordan Madden
 Author-email: <jordanmadden285@gmail.com>
 Keywords: python,tensors,neural networks,automatic differentiation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -45,15 +45,15 @@
 e = d ** 2
 f = e.sum()
 print(f.data) 
 f.backward()
 print(a.grad) 
 ```
 
-An example showing how to define and run a neural network. See demo.ipynb for more details on training.
+An example showing how to define and run a neural network. See demo.ipynb and/or regression_demo.ipynb for more details on training.
 
 ```python
 
 import mdgrad
 import mdgrad.nn as nn
 
 # Define the model and loss function
```

### Comparing `mdgrad-0.1/README.md` & `mdgrad-0.2/README.md`

 * *Files identical despite different names*

### Comparing `mdgrad-0.1/mdgrad/nn/activations.py` & `mdgrad-0.2/mdgrad/nn/activations.py`

 * *Files identical despite different names*

### Comparing `mdgrad-0.1/mdgrad/nn/layers.py` & `mdgrad-0.2/mdgrad/nn/layers.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             if isinstance(value, Module):
                 params.extend(value.parameters())
         return list(set(params))
     
 class Linear(Module):
     def __init__(self, in_features, out_features, bias=True):
         self.bias = bias
-        self.w = Tensor.randn(in_features, out_features)
+        self.w = Tensor.randn(in_features, out_features) / np.sqrt(in_features + out_features)
         self.b = Tensor.zeros((1, out_features)) if self.bias else None
 
     def forward(self, x):
         x = x if isinstance(x, Tensor) else Tensor(x)
         
         out = x @ self.w + self.b if self.bias else x @ self.w
         # Add previous tensors to computation graph
```

### Comparing `mdgrad-0.1/mdgrad/tensor.py` & `mdgrad-0.2/mdgrad/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,28 +76,25 @@
 
         def _backward():
             self.grad += (self.data > 0) * out.grad
         out._backward = _backward
 
         return out
     
-    def transpose(self,):
-        out = Tensor(np.transpose(self.data), (self,))
+    def transpose(self, axes=None):
+        out = Tensor(np.transpose(self.data, axes=axes), (self,))
         
         def _backward():
-            self.grad += np.transpose(out.grad)
+            self.grad += np.transpose(out.grad, axes=axes)
         out._backward = _backward
         
         return out
     
     def log(self):
-        print(self.data)
-        val = Tensor(np.log(self.data) + 1e-9, (self,))
-        print(val)
-        out = val
+        out = Tensor(np.log(self.data + 1e-9), (self,))
 
         def _backward():
             self.grad += (1/self.data) * out.grad
         out._backward = _backward
 
         return out
     
@@ -308,14 +305,18 @@
     out = x.sum(axis=axis, keepdims=keepdims) 
     return out * math.prod(out.shape) / math.prod(x.shape)
 
 def exp(x):
     x = x if isinstance(x, Tensor) else Tensor(x)
     return x.exp()
 
+def log(x):
+    x = x if isinstance(x, Tensor) else Tensor(x)
+    return x.log()
+
 def sin(x):
     x = x if isinstance(x, Tensor) else Tensor(x)
     return x.sin()
 
 def cos(x):
     x = x if isinstance(x, Tensor) else Tensor(x)
     return x.cos()
@@ -332,14 +333,18 @@
     x = x if isinstance(x, Tensor) else Tensor(x)
     return Tensor(np.argmax(x.data, axis=axis))
 
 def argmin(x, axis=None):
     x = x if isinstance(x, Tensor) else Tensor(x)
     return Tensor(np.argmin(x.data, axis=axis))
 
+def transpose(x, axes=None):
+    x = x if isinstance(x, Tensor) else Tensor(x)
+    return x.transpose(axes=axes)
+
 def ones(shape):
     return Tensor.ones(shape=shape)
 
 def zeros(shape):
     return Tensor.zeros(shape=shape)
 
 def eye(N, M=None):
```

### Comparing `mdgrad-0.1/mdgrad.egg-info/PKG-INFO` & `mdgrad-0.2/mdgrad.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdgrad
-Version: 0.1
+Version: 0.2
 Summary: Tensor-based autdiff engine and neural network API
 Author: Jordan Madden
 Author-email: <jordanmadden285@gmail.com>
 Keywords: python,tensors,neural networks,automatic differentiation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -45,15 +45,15 @@
 e = d ** 2
 f = e.sum()
 print(f.data) 
 f.backward()
 print(a.grad) 
 ```
 
-An example showing how to define and run a neural network. See demo.ipynb for more details on training.
+An example showing how to define and run a neural network. See demo.ipynb and/or regression_demo.ipynb for more details on training.
 
 ```python
 
 import mdgrad
 import mdgrad.nn as nn
 
 # Define the model and loss function
```

### Comparing `mdgrad-0.1/setup.py` & `mdgrad-0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.1'
+VERSION = '0.2'
 DESCRIPTION = 'Tensor-based autdiff engine and neural network API'
 LONG_DESCRIPTION = """
 # mdgrad
 
 A small autograd engine that implements backpropagation (reverse-mode autodiff). Heavily inspired by karpathy's [micrograd](https://github.com/karpathy/micrograd/tree/master), and extended to support operations on tensors instead of scalars. Includes a small neural network api for building and training neural networks.
 
 Hopefully useful as an educational resource.
@@ -32,15 +32,15 @@
 e = d ** 2
 f = e.sum()
 print(f.data) 
 f.backward()
 print(a.grad) 
 ```
 
-An example showing how to define and run a neural network. See demo.ipynb for more details on training.
+An example showing how to define and run a neural network. See demo.ipynb and/or regression_demo.ipynb for more details on training.
 
 ```python
 
 import mdgrad
 import mdgrad.nn as nn
 
 # Define the model and loss function
```

