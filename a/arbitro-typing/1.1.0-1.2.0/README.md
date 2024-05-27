# Comparing `tmp/arbitro_typing-1.1.0.tar.gz` & `tmp/arbitro_typing-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arbitro_typing-1.1.0.tar", max compression
+gzip compressed data, was "arbitro_typing-1.2.0.tar", max compression
```

## Comparing `arbitro_typing-1.1.0.tar` & `arbitro_typing-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-08 16:38:06.133912 arbitro_typing-1.1.0/arbitro_typing/__init__.py
--rw-r--r--   0        0        0      921 2024-05-08 16:41:57.827275 arbitro_typing-1.1.0/arbitro_typing/data_types.py
--rw-r--r--   0        0        0     1642 2024-05-08 16:42:41.112323 arbitro_typing-1.1.0/arbitro_typing/models/operations.py
--rw-r--r--   0        0        0     1097 2024-05-08 16:52:49.200238 arbitro_typing-1.1.0/LICENSE
--rw-r--r--   0        0        0      332 2024-05-08 17:23:18.889298 arbitro_typing-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      159 2024-05-08 17:22:18.452296 arbitro_typing-1.1.0/README.md
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 arbitro_typing-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-08 16:38:06.133912 arbitro_typing-1.2.0/arbitro_typing/__init__.py
+-rw-r--r--   0        0        0      979 2024-05-27 16:16:55.338502 arbitro_typing-1.2.0/arbitro_typing/data_types.py
+-rw-r--r--   0        0        0     5510 2024-05-27 16:16:26.249331 arbitro_typing-1.2.0/arbitro_typing/models/operations.py
+-rw-r--r--   0        0        0     1097 2024-05-08 16:52:49.200238 arbitro_typing-1.2.0/LICENSE
+-rw-r--r--   0        0        0      332 2024-05-27 16:28:43.361645 arbitro_typing-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      159 2024-05-08 17:22:18.452296 arbitro_typing-1.2.0/README.md
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 arbitro_typing-1.2.0/PKG-INFO
```

### Comparing `arbitro_typing-1.1.0/arbitro_typing/data_types.py` & `arbitro_typing-1.2.0/arbitro_typing/data_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,25 +7,25 @@
         for member in cls:
             if member == value:
                 return member
         return None
 
 class ReceivePay(ImplMissing):
     """
-    Representa un Activo (Receive) o un Pasivo (Pay).
+    Representa el tipo de pata de la operación, el cual puede ser Activo (Receive) o Pasivo (Pay).
     """
 
     RECEIVE = auto()
     PAY = auto()
 
 class Product(ImplMissing):
     """
     Representa los tipos de productos que procesa el sistema.
 
-    Los tipos soportados son: ICP=Swap Cámara, CCS=Cross Currency UF/CLP, BASIS=Basis USD/CLP.
+    Los tipos soportados son: ``ICP``=Swap Cámara, ``CCS``=Cross Currency UF/CLP, ``BASIS``=Basis USD/CLP.
     """
 
     ICP = auto()
     CCS = auto()
     BASIS = auto()
 
 class Bank(ImplMissing):
```

### Comparing `arbitro_typing-1.1.0/LICENSE` & `arbitro_typing-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arbitro_typing-1.1.0/PKG-INFO` & `arbitro_typing-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arbitro-typing
-Version: 1.1.0
+Version: 1.2.0
 Summary: 
 Author: Diego Villegas
 Author-email: dvillegas@creasys.cl
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

