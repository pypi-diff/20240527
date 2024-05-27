# Comparing `tmp/torch_onnx-0.0.1.tar.gz` & `tmp/torch_onnx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_onnx-0.0.1.tar", last modified: Sun May 26 19:03:21 2024, max compression
+gzip compressed data, was "torch_onnx-0.0.2.tar", last modified: Mon May 27 00:25:17 2024, max compression
```

## Comparing `torch_onnx-0.0.1.tar` & `torch_onnx-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:03:21.938076 torch_onnx-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-26 19:03:18.000000 torch_onnx-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-26 19:03:21.938076 torch_onnx-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-26 19:03:18.000000 torch_onnx-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-26 19:03:18.000000 torch_onnx-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 19:03:21.938076 torch_onnx-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:03:21.934076 torch_onnx-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:03:21.934076 torch_onnx-0.0.1/src/torch_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-26 19:03:18.000000 torch_onnx-0.0.1/src/torch_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-26 19:03:18.000000 torch_onnx-0.0.1/src/torch_onnx/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-26 19:03:18.000000 torch_onnx-0.0.1/src/torch_onnx/_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:03:21.938076 torch_onnx-0.0.1/src/torch_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-26 19:03:21.000000 torch_onnx-0.0.1/src/torch_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-26 19:03:21.000000 torch_onnx-0.0.1/src/torch_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 19:03:21.000000 torch_onnx-0.0.1/src/torch_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 19:03:21.000000 torch_onnx-0.0.1/src/torch_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 19:03:21.000000 torch_onnx-0.0.1/src/torch_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:25:17.473744 torch_onnx-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 00:25:01.000000 torch_onnx-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-27 00:25:17.473744 torch_onnx-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-27 00:25:01.000000 torch_onnx-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-27 00:25:01.000000 torch_onnx-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 00:25:17.473744 torch_onnx-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:25:17.469744 torch_onnx-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:25:17.473744 torch_onnx-0.0.2/src/torch_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 00:25:01.000000 torch_onnx-0.0.2/src/torch_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-27 00:25:01.000000 torch_onnx-0.0.2/src/torch_onnx/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-27 00:25:01.000000 torch_onnx-0.0.2/src/torch_onnx/_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:25:17.473744 torch_onnx-0.0.2/src/torch_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-27 00:25:17.000000 torch_onnx-0.0.2/src/torch_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-27 00:25:17.000000 torch_onnx-0.0.2/src/torch_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 00:25:17.000000 torch_onnx-0.0.2/src/torch_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 00:25:17.000000 torch_onnx-0.0.2/src/torch_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 00:25:17.000000 torch_onnx-0.0.2/src/torch_onnx.egg-info/top_level.txt
```

### Comparing `torch_onnx-0.0.1/LICENSE` & `torch_onnx-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_onnx-0.0.1/PKG-INFO` & `torch_onnx-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-onnx
-Version: 0.0.1
+Version: 0.0.2
 Summary: Experimental tools for converting PyTorch models to ONNX
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
 Project-URL: Repository, https://github.com/justinchuby/torch-onnx
 Keywords: onnx,pytorch,converter,convertion,exporter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `torch_onnx-0.0.1/README.md` & `torch_onnx-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `torch_onnx-0.0.1/pyproject.toml` & `torch_onnx-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "torch-onnx"
-version = "0.0.1"
+version = "0.0.2"
 description = "Experimental tools for converting PyTorch models to ONNX"
 authors = [{ name = "Justin Chu", email = "justinchu@microsoft.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 keywords = ["onnx", "pytorch", "converter", "convertion", "exporter"]
 classifiers = [
```

### Comparing `torch_onnx-0.0.1/src/torch_onnx/_core.py` & `torch_onnx-0.0.2/src/torch_onnx/_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -115,42 +115,67 @@
     elif isinstance(meta_val, (float, torch.SymFloat)):
         value.dtype = ir.DataType.FLOAT
         value.shape = ir.Shape([])
     else:
         pass
 
 
-def _get_node_namespace(node: torch.fx.Node) -> tuple[str, str]:
+def _get_qualified_module_name(cls: Any) -> str:
+    module = cls.__module__
+    if module is None or module == str.__class__.__module__:
+        return cls.__name__
+    return module + "." + cls.__name__
+
+
+def _get_node_namespace(node: torch.fx.Node) -> tuple[str, list[str], list[str]]:
     """Get the namespace and scope of the node.
 
+    Example::
+
+        {
+            'L__self__': ('', <class 'torchvision.models.resnet.ResNet'>),
+            'L__self___avgpool': ('avgpool', <class 'torch.nn.modules.pooling.AdaptiveAvgPool2d'>)
+        }
+
+    Will yield
+
+    namespace: ": torchvision.models.resnet.ResNet/avgpool: torch.nn.modules.pooling.AdaptiveAvgPool2d"
+    class_hierarchy: ["torchvision.models.resnet.ResNet", "torch.nn.modules.pooling.AdaptiveAvgPool2d"]
+    name_scopes: ["", "avgpool"]
+
     Args:
         node: The node to get the namespace and scope of.
 
     Returns:
-        A tuple of the namespace and the leave module name.
+        (namespace, class_hierarchy, name_scope)
     """
     nn_module_stack = node.meta.get("nn_module_stack")
+    print(nn_module_stack)
     if nn_module_stack is None:
         logging.warning("nn_module_stack not found for node %s", node.name)
-        return "", ""
-    scopes = []
-    module_name = ""
+        return "", [], []
+    namespaces = []
+    class_hierarchy = []
+    name_scopes = []
     for name, nn_module in nn_module_stack.values():
-        scopes.append(name)
-        module_name = repr(nn_module)
+        name_scopes.append(name)
+        nn_module_name = _get_qualified_module_name(nn_module)
+        class_hierarchy.append(nn_module_name)
+        namespaces.append(f"{name}: {_get_qualified_module_name(nn_module)}")
 
-    return "/".join(scopes), module_name
+    return "/".join(namespaces), class_hierarchy, name_scopes
 
 
 def _set_namespace(node: torch.fx.Node, ir_node: ir.Node):
     nn_module_stack = node.meta.get("nn_module_stack")
     node.meta["nn_module_stack"] = nn_module_stack
-    namespace, module_name = _get_node_namespace(node)
+    namespace, class_hierarchy, name_scopes = _get_node_namespace(node)
     ir_node.metadata_props["namespace"] = namespace
-    ir_node.metadata_props["module_name"] = module_name
+    ir_node.metadata_props["class_hierarchy"] = repr(class_hierarchy)
+    ir_node.metadata_props["name_scopes"] = repr(name_scopes)
 
 
 def _add_nodes(
     exported_program: torch.export.ExportedProgram, graph: ir.Graph
 ) -> dict[str, ir.Value]:
     values: dict[str, ir.Value] = {}
     for node in exported_program.graph.nodes:
```

### Comparing `torch_onnx-0.0.1/src/torch_onnx/_patch.py` & `torch_onnx-0.0.2/src/torch_onnx/_patch.py`

 * *Files identical despite different names*

### Comparing `torch_onnx-0.0.1/src/torch_onnx.egg-info/PKG-INFO` & `torch_onnx-0.0.2/src/torch_onnx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-onnx
-Version: 0.0.1
+Version: 0.0.2
 Summary: Experimental tools for converting PyTorch models to ONNX
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
 Project-URL: Repository, https://github.com/justinchuby/torch-onnx
 Keywords: onnx,pytorch,converter,convertion,exporter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

