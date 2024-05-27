# Comparing `tmp/torch_onnx-0.0.2.tar.gz` & `tmp/torch_onnx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_onnx-0.0.2.tar", last modified: Mon May 27 00:25:17 2024, max compression
+gzip compressed data, was "torch_onnx-0.0.3.tar", last modified: Mon May 27 01:49:50 2024, max compression
```

## Comparing `torch_onnx-0.0.2.tar` & `torch_onnx-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:25:17.473744 torch_onnx-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 00:25:01.000000 torch_onnx-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-27 00:25:17.473744 torch_onnx-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-27 00:25:01.000000 torch_onnx-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-27 00:25:01.000000 torch_onnx-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 00:25:17.473744 torch_onnx-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:25:17.469744 torch_onnx-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:25:17.473744 torch_onnx-0.0.2/src/torch_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 00:25:01.000000 torch_onnx-0.0.2/src/torch_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-27 00:25:01.000000 torch_onnx-0.0.2/src/torch_onnx/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-27 00:25:01.000000 torch_onnx-0.0.2/src/torch_onnx/_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:25:17.473744 torch_onnx-0.0.2/src/torch_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-27 00:25:17.000000 torch_onnx-0.0.2/src/torch_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-27 00:25:17.000000 torch_onnx-0.0.2/src/torch_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 00:25:17.000000 torch_onnx-0.0.2/src/torch_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 00:25:17.000000 torch_onnx-0.0.2/src/torch_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 00:25:17.000000 torch_onnx-0.0.2/src/torch_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:49:50.679819 torch_onnx-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 01:49:47.000000 torch_onnx-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-27 01:49:50.675819 torch_onnx-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-27 01:49:47.000000 torch_onnx-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-27 01:49:47.000000 torch_onnx-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 01:49:50.679819 torch_onnx-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:49:50.675819 torch_onnx-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:49:50.675819 torch_onnx-0.0.3/src/torch_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 01:49:47.000000 torch_onnx-0.0.3/src/torch_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-05-27 01:49:47.000000 torch_onnx-0.0.3/src/torch_onnx/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-27 01:49:47.000000 torch_onnx-0.0.3/src/torch_onnx/_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:49:50.675819 torch_onnx-0.0.3/src/torch_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-27 01:49:50.000000 torch_onnx-0.0.3/src/torch_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-27 01:49:50.000000 torch_onnx-0.0.3/src/torch_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 01:49:50.000000 torch_onnx-0.0.3/src/torch_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 01:49:50.000000 torch_onnx-0.0.3/src/torch_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 01:49:50.000000 torch_onnx-0.0.3/src/torch_onnx.egg-info/top_level.txt
```

### Comparing `torch_onnx-0.0.2/LICENSE` & `torch_onnx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_onnx-0.0.2/PKG-INFO` & `torch_onnx-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-onnx
-Version: 0.0.2
+Version: 0.0.3
 Summary: Experimental tools for converting PyTorch models to ONNX
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
 Project-URL: Repository, https://github.com/justinchuby/torch-onnx
 Keywords: onnx,pytorch,converter,convertion,exporter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `torch_onnx-0.0.2/README.md` & `torch_onnx-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `torch_onnx-0.0.2/pyproject.toml` & `torch_onnx-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "torch-onnx"
-version = "0.0.2"
+version = "0.0.3"
 description = "Experimental tools for converting PyTorch models to ONNX"
 authors = [{ name = "Justin Chu", email = "justinchu@microsoft.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 keywords = ["onnx", "pytorch", "converter", "convertion", "exporter"]
 classifiers = [
```

### Comparing `torch_onnx-0.0.2/src/torch_onnx/_core.py` & `torch_onnx-0.0.3/src/torch_onnx/_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import ctypes
 import inspect
 import itertools
 import logging
-from typing import Any
+import operator
+import typing
+from typing import Any, Sequence
 
 import numpy as np
 import torch
 import torch.fx
 from onnxscript import ir
 from onnxscript.ir import _convenience as ir_convenience
 from torch.export import graph_signature
@@ -88,14 +90,19 @@
 #     BUFFER_MUTATION = auto()
 #     GRADIENT_TO_PARAMETER = auto()
 #     GRADIENT_TO_USER_INPUT = auto()
 #     USER_INPUT_MUTATION = auto()
 #     TOKEN = auto()
 
 
+def _set_shape_types(values: Sequence[ir.Value], meta_vals: Sequence[torch.Tensor]):
+    for value, meta_val in zip(values, meta_vals):
+        _set_shape_type(value, meta_val)
+
+
 def _set_shape_type(value: ir.Value, meta_val: torch.Tensor | tuple[torch.Tensor]):
     if isinstance(meta_val, tuple):
         logger.warning("Setting shape and type of tensors is not supported yet")
     if isinstance(meta_val, torch.Tensor):
         dims = []
         for dim in meta_val.shape:
             if isinstance(dim, int):
@@ -145,15 +152,15 @@
     Args:
         node: The node to get the namespace and scope of.
 
     Returns:
         (namespace, class_hierarchy, name_scope)
     """
     nn_module_stack = node.meta.get("nn_module_stack")
-    print(nn_module_stack)
+    logger.debug("%s", nn_module_stack)
     if nn_module_stack is None:
         logging.warning("nn_module_stack not found for node %s", node.name)
         return "", [], []
     namespaces = []
     class_hierarchy = []
     name_scopes = []
     for name, nn_module in nn_module_stack.values():
@@ -170,116 +177,160 @@
     node.meta["nn_module_stack"] = nn_module_stack
     namespace, class_hierarchy, name_scopes = _get_node_namespace(node)
     ir_node.metadata_props["namespace"] = namespace
     ir_node.metadata_props["class_hierarchy"] = repr(class_hierarchy)
     ir_node.metadata_props["name_scopes"] = repr(name_scopes)
 
 
+def _handle_getitem_node(
+    node: torch.fx.Node, node_name_to_values: dict[str, ir.Value | Sequence[ir.Value]]
+) -> ir.Value:
+    """Handle a getitem node.
+
+    Add the input value it is getting to the mapping, then return the value.
+    """
+    assert len(node.all_input_nodes) == 1
+    source = node.all_input_nodes[0]
+    source_outputs = node_name_to_values[source.name]
+    assert isinstance(
+        source_outputs, Sequence
+    ), f"Expected {source.name} to output sequence, got {node_name_to_values[source.name]}"
+    index = typing.cast(int, node.args[1])
+    value = source_outputs[index]
+    # Save the getitem value to the values mapping to in case
+    # it is one of the graph outputs
+    node_name_to_values[node.name] = value
+    return value
+
+
 def _add_nodes(
     exported_program: torch.export.ExportedProgram, graph: ir.Graph
 ) -> dict[str, ir.Value]:
-    values: dict[str, ir.Value] = {}
+    node_name_to_values: dict[str, ir.Value | Sequence[ir.Value]] = {}
     for node in exported_program.graph.nodes:
-        print(node.name, node.args, node.target, node.op, node.type, node.kwargs)
+        logger.debug(
+            "%s", (node.name, node.args, node.target, node.op, node.type, node.kwargs)
+        )
         if node.op == "placeholder":
             # Placeholder nodes are user inputs
             # We need to create a new tensor for each user input
             # and add it to the graph's inputs
             name = node.name
             # shape = node.kwargs["shape"]
             # dtype = node.kwargs["dtype"]
             input_ = ir.Input(name)
             input_.meta["node"] = node
-            values[name] = input_
+            node_name_to_values[name] = input_
             # The inputs will be added to the graph later
         elif node.op == "call_function":
+            if node.target == operator.getitem:
+                _handle_getitem_node(node, node_name_to_values)
+                continue
             # Add op to the graph
             op = str(node.target)
-            fx_inputs, attributes = _get_inputs_and_attributes(node)
+            fx_inputs, attributes, input_names, output_names = (
+                _get_inputs_and_attributes(node)
+            )
             inputs = []
             for i, input_ in enumerate(fx_inputs):
                 if input_ is None:
                     inputs.append(None)
                 elif hasattr(input_, "name"):
-                    inputs.append(values[input_.name])
+                    if (
+                        isinstance(input_, torch.fx.Node)
+                        and input_.target == operator.getitem
+                    ):
+                        actual_input = _handle_getitem_node(input_, node_name_to_values)
+                        inputs.append(actual_input)
+                    else:
+                        inputs.append(node_name_to_values[input_.name])
                 else:
                     attributes[f"arg_{i}"] = input_
 
-            output_name = node.name
-            output = ir.Value(name=output_name)
-            _set_shape_type(output, node.meta["val"])
+            outputs = [ir.Value(name=name) for name in output_names]
+            if len(outputs) > 1:
+                _set_shape_types(outputs, node.meta["val"])
+                node_name_to_values[node.name] = outputs
+            else:
+                _set_shape_type(outputs[0], node.meta["val"])
+                node_name_to_values[node.name] = outputs[0]
 
-            values[output_name] = output
             ir_node = ir.Node(
                 "pkg.torch.ops",
                 op,
                 inputs,
                 attributes=ir_convenience.convert_attributes(attributes),
-                outputs=[output],
+                outputs=outputs,
                 name=node.name,
             )
             ir_node.meta["node"] = node
-            graph.append(ir_node)
-
+            ir_node.metadata_props["fx_node"] = str(node.format_node())
+            ir_node.metadata_props["input_names"] = repr(input_names)
             # Record the nn.Module stack for the node
             _set_namespace(node, ir_node)
-    return values
+
+            graph.append(ir_node)
+    return node_name_to_values
 
 
 def _torch_version_integer() -> int:
     return int(torch.__version__.replace(".", ""))
 
 
 def _get_inputs_and_attributes(
     node: torch.fx.Node,
-) -> tuple[list[torch.fx.Node | None], dict[str, Any]]:
-    """Find and Fill in the not provided kwargs with default values."""
+) -> tuple[list[torch.fx.Node | None], dict[str, Any], list[str], list[str]]:
+    """Find and Fill in the not provided kwargs with default values.
 
-    # TODO: aten::sym_size has overload, but fx graph is using
-    # overloadpacket for some reasons.
-    # https://github.com/pytorch/pytorch/issues/97201
-    # We manually assigned overload for aten::sym_size.
-    if hasattr(node.target, "_schema"):
-        node_schema = node.target._schema  # type: ignore[union-attr]
-    else:
-        node_schema = torch.ops.aten.sym_size.int._schema  # type: ignore[union-attr]
+    Returns:
+        (inputs, attributes, input_names, output_names)
+    """
+    if inspect.isbuiltin(node.target) or isinstance(node.target, str):
+        inputs = list(node.args)
+        return inputs, {}, [], [node.name]
+
+    # The target should be an ATen operator now
+    node_schema = node.target._schema
 
     # This function assumes the order of arguments in FX op is the
     # same as the order of arguments in TorchScript op.
     inputs = []
+    input_names = []
     attributes = {}
 
     if inspect.isbuiltin(node.target):
         inputs = list(node.args)
     else:
         for arg, schema_arg in zip(node.args, node_schema.arguments):
             if arg is None or isinstance(arg, torch.fx.Node):
                 inputs.append(arg)
+                input_names.append(schema_arg.name)
             else:
                 attributes[schema_arg.name] = arg
         for schema_arg in node_schema.arguments:
             if schema_arg.name not in node.kwargs:
                 continue
             if schema_arg.name in {
                 "layout",
                 "device",
                 "requires_grad",
-                "pin_memory",
                 "memory_format",
                 "implicit",
             }:
                 attr = str(node.kwargs[schema_arg.name])
             if schema_arg.name == "dtype":
                 attr = _torch_dtype_to_onnx_dtype(node.kwargs[schema_arg.name])
             else:
                 attr = node.kwargs[schema_arg.name]
 
             attributes[schema_arg.name] = attr
 
-    return inputs, attributes
+    output_names = [f"{node.name}_{output.name}" for output in node_schema.returns]
+
+    return inputs, attributes, input_names, output_names
 
 
 def exported_program_to_ir_graph(exported_program: torch.export.ExportedProgram):
     # TODO: Make it an Interpreter
     graph = ir.Graph(
         [],
         [],
```

### Comparing `torch_onnx-0.0.2/src/torch_onnx/_patch.py` & `torch_onnx-0.0.3/src/torch_onnx/_patch.py`

 * *Files identical despite different names*

### Comparing `torch_onnx-0.0.2/src/torch_onnx.egg-info/PKG-INFO` & `torch_onnx-0.0.3/src/torch_onnx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-onnx
-Version: 0.0.2
+Version: 0.0.3
 Summary: Experimental tools for converting PyTorch models to ONNX
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
 Project-URL: Repository, https://github.com/justinchuby/torch-onnx
 Keywords: onnx,pytorch,converter,convertion,exporter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

