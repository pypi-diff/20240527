# Comparing `tmp/dagstream-0.1.4-py3-none-any.whl.zip` & `tmp/dagstream-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,26 @@
-Zip file size: 11372 bytes, number of entries: 20
--rw-r--r--  2.0 unx      880 b- defN 80-Jan-01 00:00 pyproject.toml
+Zip file size: 13762 bytes, number of entries: 24
+-rw-r--r--  2.0 unx     1011 b- defN 80-Jan-01 00:00 pyproject.toml
 -rw-r--r--  2.0 unx      145 b- defN 80-Jan-01 00:00 dagstream/__init__.py
--rw-r--r--  2.0 unx     3674 b- defN 80-Jan-01 00:00 dagstream/dagstream.py
--rw-r--r--  2.0 unx     4713 b- defN 80-Jan-01 00:00 dagstream/executor.py
--rw-r--r--  2.0 unx       82 b- defN 80-Jan-01 00:00 dagstream/graph_components/__init__.py
+-rw-r--r--  2.0 unx     4831 b- defN 80-Jan-01 00:00 dagstream/dagstream.py
+-rw-r--r--  2.0 unx     5140 b- defN 80-Jan-01 00:00 dagstream/executor.py
+-rw-r--r--  2.0 unx      206 b- defN 80-Jan-01 00:00 dagstream/graph_components/__init__.py
+-rw-r--r--  2.0 unx     2461 b- defN 80-Jan-01 00:00 dagstream/graph_components/_interface.py
 -rw-r--r--  2.0 unx       96 b- defN 80-Jan-01 00:00 dagstream/graph_components/dags/__init__.py
--rw-r--r--  2.0 unx     2218 b- defN 80-Jan-01 00:00 dagstream/graph_components/dags/functional_dag.py
--rw-r--r--  2.0 unx      404 b- defN 80-Jan-01 00:00 dagstream/graph_components/dags/interface.py
--rw-r--r--  2.0 unx      148 b- defN 80-Jan-01 00:00 dagstream/graph_components/nodes/__init__.py
--rw-r--r--  2.0 unx     1790 b- defN 80-Jan-01 00:00 dagstream/graph_components/nodes/functional_node.py
--rw-r--r--  2.0 unx     1568 b- defN 80-Jan-01 00:00 dagstream/graph_components/nodes/interface.py
--rw-r--r--  2.0 unx     1402 b- defN 80-Jan-01 00:00 dagstream/graph_components/nodes/node_state.py
+-rw-r--r--  2.0 unx     3514 b- defN 80-Jan-01 00:00 dagstream/graph_components/dags/functional_dag.py
+-rw-r--r--  2.0 unx      428 b- defN 80-Jan-01 00:00 dagstream/graph_components/dags/interface.py
+-rw-r--r--  2.0 unx       27 b- defN 80-Jan-01 00:00 dagstream/graph_components/edges/__init__.py
+-rw-r--r--  2.0 unx      385 b- defN 80-Jan-01 00:00 dagstream/graph_components/edges/_edge.py
+-rw-r--r--  2.0 unx       59 b- defN 80-Jan-01 00:00 dagstream/graph_components/nodes/__init__.py
+-rw-r--r--  2.0 unx     2996 b- defN 80-Jan-01 00:00 dagstream/graph_components/nodes/functional_node.py
+-rw-r--r--  2.0 unx      988 b- defN 80-Jan-01 00:00 dagstream/graph_components/nodes/node_state.py
+-rw-r--r--  2.0 unx       36 b- defN 80-Jan-01 00:00 dagstream/utils/__init__.py
 -rw-r--r--  2.0 unx      309 b- defN 80-Jan-01 00:00 dagstream/utils/errors.py
+-rw-r--r--  2.0 unx      248 b- defN 80-Jan-01 00:00 dagstream/utils/util.py
 -rw-r--r--  2.0 unx       81 b- defN 80-Jan-01 00:00 dagstream/version.py
 -rw-r--r--  2.0 unx       51 b- defN 80-Jan-01 00:00 dagstream/viewers/__init__.py
--rw-r--r--  2.0 unx     1725 b- defN 80-Jan-01 00:00 dagstream/viewers/viewer.py
--rw-r--r--  2.0 unx      549 b- defN 80-Jan-01 00:00 dagstream-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2753 b- defN 80-Jan-01 00:00 dagstream-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dagstream-0.1.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1739 b- defN 16-Jan-01 00:00 dagstream-0.1.4.dist-info/RECORD
-20 files, 24415 bytes uncompressed, 8492 bytes compressed:  65.2%
+-rw-r--r--  2.0 unx     1947 b- defN 80-Jan-01 00:00 dagstream/viewers/viewer.py
+-rw-r--r--  2.0 unx      549 b- defN 80-Jan-01 00:00 dagstream-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2753 b- defN 80-Jan-01 00:00 dagstream-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dagstream-0.1.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2091 b- defN 16-Jan-01 00:00 dagstream-0.1.5.dist-info/RECORD
+24 files, 30440 bytes uncompressed, 10318 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -9,53 +9,65 @@
 
 Filename: dagstream/executor.py
 Comment: 
 
 Filename: dagstream/graph_components/__init__.py
 Comment: 
 
+Filename: dagstream/graph_components/_interface.py
+Comment: 
+
 Filename: dagstream/graph_components/dags/__init__.py
 Comment: 
 
 Filename: dagstream/graph_components/dags/functional_dag.py
 Comment: 
 
 Filename: dagstream/graph_components/dags/interface.py
 Comment: 
 
+Filename: dagstream/graph_components/edges/__init__.py
+Comment: 
+
+Filename: dagstream/graph_components/edges/_edge.py
+Comment: 
+
 Filename: dagstream/graph_components/nodes/__init__.py
 Comment: 
 
 Filename: dagstream/graph_components/nodes/functional_node.py
 Comment: 
 
-Filename: dagstream/graph_components/nodes/interface.py
+Filename: dagstream/graph_components/nodes/node_state.py
 Comment: 
 
-Filename: dagstream/graph_components/nodes/node_state.py
+Filename: dagstream/utils/__init__.py
 Comment: 
 
 Filename: dagstream/utils/errors.py
 Comment: 
 
+Filename: dagstream/utils/util.py
+Comment: 
+
 Filename: dagstream/version.py
 Comment: 
 
 Filename: dagstream/viewers/__init__.py
 Comment: 
 
 Filename: dagstream/viewers/viewer.py
 Comment: 
 
-Filename: dagstream-0.1.4.dist-info/LICENSE
+Filename: dagstream-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: dagstream-0.1.4.dist-info/METADATA
+Filename: dagstream-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: dagstream-0.1.4.dist-info/WHEEL
+Filename: dagstream-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: dagstream-0.1.4.dist-info/RECORD
+Filename: dagstream-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyproject.toml

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dagstream"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["sakamoto <sakamoto@ricos.co.jp>"]
 license = "Apache-2.0"
 classifiers = []
 readme = "README.md"
 homepage = "https://github.com/ricosjp/dagstream"
 repository = "https://github.com/ricosjp/dagstream"
@@ -35,7 +35,15 @@
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 
 [tool.isort]
 profile = "black"
+
+
+[tool.coverage.report]
+exclude_also = [
+    "def __repr__",
+    "@(abc\\.)?abstractmethod",
+    "raise NotImplementedError"
+    ]
```

## dagstream/dagstream.py

```diff
@@ -1,47 +1,73 @@
-from typing import Callable, Iterable, Optional
+from typing import Callable, Iterable, Optional, Union
 
-from dagstream.graph_components import FunctionalDag, IDrawableGraph
-from dagstream.graph_components.nodes import (
-    FunctionalNode,
+from dagstream import utils
+from dagstream.graph_components import (
+    FunctionalDag,
+    IDrawableGraph,
     IDrawableNode,
     IFunctionalNode,
 )
+from dagstream.graph_components.nodes import FunctionalNode
 from dagstream.utils.errors import DagStreamCycleError
 
 
 class DagStream(IDrawableGraph):
     def __init__(self) -> None:
-        self._functions: set[IFunctionalNode] = set()
+        self._name2node: dict[str, IFunctionalNode] = {}
+        # This counter aims to distinguish
+        # between nodes which have the same function name
+        self._SAME_NAME_COUNTER: dict[str, int] = {}
+
+    def check_exists(self, node: Union[str, IFunctionalNode]) -> bool:
+        if isinstance(node, IFunctionalNode):
+            return node.mut_name in self._name2node
 
-    def check_exists(self, node: IFunctionalNode) -> bool:
-        return node in self._functions
+        if isinstance(node, str):
+            return node in self._name2node
+
+        raise NotImplementedError()
 
     def get_drawable_nodes(self) -> Iterable[IDrawableNode]:
-        return self._functions
+        return self._name2node.values()
 
-    def get_functions(self) -> set[IFunctionalNode]:
-        return self._functions
+    def get_functions(self) -> Iterable[IFunctionalNode]:
+        return self._name2node.values()
 
     def emplace(self, *functions: Callable) -> tuple[IFunctionalNode, ...]:
         """create a functional node corresponding to each function
 
         Returns
         -------
         tuple[IFunctionalNode, ...]
             functional node corresponding to each function
         """
 
         # To ensure orders
-        _functions: list[IFunctionalNode] = []
+        _nodes: list[IFunctionalNode] = []
         for func in functions:
-            node = FunctionalNode(func)
-            _functions.append(node)
-            self._functions.add(node)
-        return tuple(_functions)
+            node_name = self._create_node_name(func)
+            node = FunctionalNode(func, mut_node_name=node_name)
+            _nodes.append(node)
+            self._name2node.update({node.mut_name: node})
+
+        return tuple(_nodes)
+
+    def _create_node_name(self, user_function: Callable) -> str:
+        function_name = utils.get_function_name(user_function)
+        if function_name not in self._name2node:
+            return function_name
+
+        _counter = self._SAME_NAME_COUNTER.get(function_name, 0)
+        _counter += 1
+
+        node_name = f"{function_name}_{_counter}"
+
+        self._SAME_NAME_COUNTER[function_name] = _counter
+        return node_name
 
     def construct(
         self, mandatory_nodes: Optional[set[IFunctionalNode]] = None
     ) -> FunctionalDag:
         """create functional dag
 
         Solving dependencies and create dag structure composed of functional nodes
@@ -56,68 +82,71 @@
         -------
         FunctionalDag
             dag structure object composed of functional nodes
         """
         self._detect_cycle()
 
         if mandatory_nodes is None:
-            functions = self._functions
+            functions = self._name2node
         else:
             functions = self._extract_functions(mandatory_nodes)
 
         return FunctionalDag(functions)
 
     def _extract_functions(
         self, mandatory_nodes: set[IFunctionalNode]
-    ) -> set[IFunctionalNode]:
-        visited: set[IFunctionalNode] = set()
+    ) -> dict[str, IFunctionalNode]:
+        visited: dict[str, IFunctionalNode] = {}
 
         for node in mandatory_nodes:
             self._extract_subdag(node, visited)
         return visited
 
     def _extract_subdag(
-        self, mandatory_node: IFunctionalNode, visited: set[IFunctionalNode]
+        self, mandatory_node: IFunctionalNode, visited: dict[str, IFunctionalNode]
     ):
-        if mandatory_node in visited:
+        if mandatory_node.mut_name in visited:
             return
 
-        visited.add(mandatory_node)
-        predecessors: list[IFunctionalNode] = [v for v in mandatory_node.predecessors]
+        visited.update({mandatory_node.mut_name: mandatory_node})
+        predecessors: list[str] = [v for v in mandatory_node.predecessors]
 
         while len(predecessors) != 0:
-            node = predecessors.pop()
-            if node in visited:
+            node_name = predecessors.pop()
+            node = self._name2node[node_name]
+            if node.mut_name in visited:
                 continue
-            visited.add(node)
+            visited.update({node.mut_name: node})
 
             for next_node in node.predecessors:
                 predecessors.append(next_node)
 
         return None
 
     def _detect_cycle(self):
-        finished = set()
-        seen = set()
-        for func in self._functions:
-            if func in finished:
+        finished: set[str] = set()
+        seen: set[str] = set()
+        for node in self._name2node.values():
+            if node.mut_name in finished:
                 continue
-            self._dfs_detect_cycle(func, finished, seen)
+            self._dfs_detect_cycle(node, finished, seen)
         return None
 
     def _dfs_detect_cycle(
         self,
         start: IFunctionalNode,
-        finished: set[IFunctionalNode],
-        seen: set[IFunctionalNode],
+        finished: set[str],
+        seen: set[str],
     ) -> None:
-        for node in start.successors:
-            if node in finished:
+        for edge in start.successors:
+            node = self._name2node[edge.to_node]
+
+            if node.mut_name in finished:
                 continue
 
-            if (node in seen) and (node not in finished):
+            if (node.mut_name in seen) and (node.mut_name not in finished):
                 raise DagStreamCycleError("Detect cycle in your definition of dag.")
 
-            seen.add(node)
+            seen.add(node.mut_name)
             self._dfs_detect_cycle(node, finished, seen)
 
-        finished.add(start)
+        finished.add(start.mut_name)
```

## dagstream/executor.py

```diff
@@ -1,11 +1,10 @@
 import multiprocessing as multi
-from typing import Any
+from typing import Any, Union
 
-from dagstream.dagstream import IFunctionalNode
 from dagstream.graph_components import FunctionalDag
 
 
 class StreamExecutor:
     def __init__(self, functional_dag: FunctionalDag) -> None:
         """Executor for FunctionalDag Object.
 
@@ -22,39 +21,53 @@
         if not isinstance(functional_dag, FunctionalDag):
             raise ValueError(
                 "functional_dag is not a instance of FunctionalDag. "
                 "Maybe, you forget to call 'your_dagstream.construct()' beforehand."
             )
         self._dag = functional_dag
 
-    def run(self, *args, **kwargs) -> dict[str, Any]:
+    def run(
+        self,
+        *args: Any,
+        first_args: Union[tuple[Any], None] = None,
+        save_all_state: bool = False,
+        **kwargs,
+    ) -> dict[str, Any]:
         """Run functions sequencially according to static order.
 
         Input parameters are passed to all functions.
 
         Returns
         -------
         dict[str, Any]
             Key is name of function, value is returned objects from each function.
         """
         results: dict[str, Any] = {}
+
         while self._dag.is_active:
             nodes = self._dag.get_ready()
             for node in nodes:
+                if node.n_predecessors == 0 and first_args is not None:
+                    for arg in first_args:
+                        node.receive_args(arg)
+
                 result = node.run(*args, **kwargs)
-                results.update({node.name: result})
-                self._dag.done(node)
+                self._dag.send(node.mut_name, result)
+                self._dag.done(node.mut_name)
+
+                if self._dag.check_last(node) or save_all_state:
+                    results.update({node.mut_name: result})
 
         return results
 
 
 class StreamParallelExecutor:
     """Parallel Executor for FunctionalDag Object."""
 
-    def __init__(self, functional_dag: FunctionalDag, n_processes: int = 1) -> None:
+    def __init__(self, functional_dag: FunctionalDag, n_process: int = 1) -> None:
         """THIS IS EXPERIMENTAL FEATURE. Parallel Executor for FunctionalDag Object.
 
         Parameters
         ----------
         functional_dag : FunctionalDag
             FunctionalDag instance which is already constructed from DagStream Object
         n_processes : int, optional
@@ -68,24 +81,25 @@
         if not isinstance(functional_dag, FunctionalDag):
             raise ValueError(
                 "functional_dag is not a instance of FunctionalDag. "
                 "Maybe, you forget to call 'your_dagstream.construct()' beforehand."
             )
 
         self._dag = functional_dag
-        self._n_processes = n_processes
+        self._n_processes = n_process
         if self._n_processes <= 0:
-            raise ValueError(f"n_processes must be larger than 0. Input: {n_processes}")
+            raise ValueError(f"n_processes must be larger than 0. Input: {n_process}")
 
-    def _worker(self, input_queue: multi.Queue, done_queue: multi.Queue):
-        for func, args, kwargs in iter(input_queue.get, "STOP"):
-            result = func.run(*args, **kwargs)
-            done_queue.put((func, result))
-
-    def run(self, *args, **kwargs) -> dict[str, Any]:
+    def run(
+        self,
+        *args: Any,
+        first_args: Union[tuple[Any], None] = None,
+        save_all_state: bool = False,
+        **kwargs,
+    ) -> dict[str, Any]:
         """Run functions in parallel.
 
         Parameters are passed to all functions.
         Please note that parameters are not shared between multiple processes.
 
         Returns
         -------
@@ -93,42 +107,48 @@
             Key is name of function, value is returned objects from each function.
         """
         task_queue: multi.Queue = multi.Queue()
         done_queue: multi.Queue = multi.Queue()
         all_processes: list[multi.Process] = []
 
         results: dict[str, Any] = {}
-        _name2nodes: dict[str, IFunctionalNode] = {
-            node.name: node for node in self._dag._nodes
-        }
 
         while self._dag.is_active:
             nodes = self._dag.get_ready()
 
-            for node_func in nodes:
-                task_queue.put((node_func, args, kwargs))
+            for node in nodes:
+                if node.n_predecessors == 0 and first_args is not None:
+                    for arg in first_args:
+                        node.receive_args(arg)
+
+                task_queue.put((node, args, kwargs))
 
             # Start worker processes
             n_left_process = self._n_processes - len(all_processes)
             for _ in range(n_left_process):
-                process = multi.Process(
-                    target=self._worker, args=(task_queue, done_queue)
-                )
+                process = multi.Process(target=_worker, args=(task_queue, done_queue))
                 process.start()
                 all_processes.append(process)
 
             while not done_queue.empty():
                 _done_node, _result = done_queue.get()
 
-                # HACK: When using multiprocessing, id(IFunctionalNode)
+                # NOTE: When using multiprocessing, id(IFunctionalNode)
                 # after running is not the same as one before running.
-                # This operation is incorporated in the Dagstream object,
-                # after names of all nodes are guranteed to be unique.
-                done_node = _name2nodes[_done_node.name]
-                self._dag.done(done_node)
-                results.update({done_node.name: _result})
+
+                self._dag.send(_done_node.mut_name, _result)
+                self._dag.done(_done_node.mut_name)
+
+                if self._dag.check_last(_done_node) or save_all_state:
+                    results.update({_done_node.mut_name: _result})
 
             if not self._dag.is_active:
                 for _ in range(self._n_processes):
                     task_queue.put("STOP")
 
         return results
+
+
+def _worker(input_queue: multi.Queue, done_queue: multi.Queue):
+    for func, args, kwargs in iter(input_queue.get, "STOP"):
+        result = func.run(*args, **kwargs)
+        done_queue.put((func, result))
```

## dagstream/graph_components/__init__.py

```diff
@@ -1 +1,7 @@
+from dagstream.graph_components._interface import (
+    IDagEdge,
+    IDrawableNode,
+    IFunctionalNode,
+    INodeState,
+)
 from dagstream.graph_components.dags import FunctionalDag, IDrawableGraph  # NOQA
```

## dagstream/graph_components/dags/functional_dag.py

```diff
@@ -1,74 +1,116 @@
-from typing import Iterable
+from typing import Any, Iterable, Union
 
-from dagstream.graph_components.nodes import IDrawableNode, IFunctionalNode, INodeState
+from dagstream.graph_components._interface import (
+    IDrawableNode,
+    IFunctionalNode,
+    INodeState,
+)
 
 from .interface import IDrawableGraph
 
 
 class FunctionalDag(IDrawableGraph):
-    def __init__(self, nodes: set[IFunctionalNode]) -> None:
-        self._nodes = nodes
+    def __init__(self, name2nodes: dict[str, IFunctionalNode]) -> None:
+        self._name2nodes = name2nodes
         self._n_finished: int = 0
-        self._n_functions: int = len(self._nodes)
+        self._n_functions: int = len(self._name2nodes)
 
-        self._name2state: dict[IFunctionalNode, INodeState] = {
-            node: node.prepare() for node in self._nodes
+        self._name2state: dict[str, INodeState] = {
+            node.mut_name: node.prepare() for node in name2nodes.values()
         }
         self._ready_nodes: list[IFunctionalNode] = [
-            node for node in self._nodes if self._name2state[node].is_ready
+            node
+            for node in name2nodes.values()
+            if self._name2state[node.mut_name].is_ready
         ]
 
+        self._last_node_names: set[str] = {
+            node.mut_name for node in name2nodes.values() if self._is_last_node(node)
+        }
+
+    def _is_last_node(self, node: IFunctionalNode):
+        n_successors = sum(
+            [1 for edge in node.successors if edge.to_node in self._name2nodes]
+        )
+        return n_successors == 0
+
     @property
     def is_active(self) -> bool:
         """Check whether unfinished functions exist or not
 
         Returns
         -------
         bool
             True if not finished functions exist
         """
         return self._n_finished < self._n_functions
 
-    def check_exists(self, node: IFunctionalNode) -> bool:
+    def check_last(self, node: Union[str, IFunctionalNode]):
+        if isinstance(node, str):
+            return node in self._last_node_names
+
+        if isinstance(node, IFunctionalNode):
+            return node.mut_name in self._last_node_names
+
+        raise NotImplementedError()
+
+    def check_exists(self, node: Union[IFunctionalNode, str]) -> bool:
         """Chech whether node exists in this functional dag.
 
         Parameters
         ----------
         node : IFunctionalNode
             functional node to search
 
         Returns
         -------
         bool
             True if node exists in this functional dag.
         """
-        return node in self._nodes
+        if isinstance(node, IFunctionalNode):
+            return node.mut_name in self._name2nodes
+        if isinstance(node, str):
+            return node in self._name2nodes
+
+        raise NotImplementedError()
 
     def get_drawable_nodes(self) -> Iterable[IDrawableNode]:
-        return self._nodes
+        return self._name2nodes.values()
 
     def get_ready(self) -> tuple[IFunctionalNode, ...]:
         result = tuple(self._ready_nodes)
         self._ready_nodes.clear()
         return result
 
-    def done(self, *finished_nodes: IFunctionalNode) -> None:
+    def send(self, node_name: str, result: Any) -> None:
+        node = self._name2nodes[node_name]
+
+        for edge in node.successors:
+            if not edge.is_pipe:
+                continue
+
+            if not self.check_exists(edge.to_node):
+                continue
+
+            next_node = self._name2nodes[edge.to_node]
+            next_node.receive_args(result)
+
+    def done(self, *node_names: str) -> None:
         """Register nodes as finished and update state
 
         Parameters
         ----------
         *finished_nodes : IFunctionalNode
             finished nodes
 
         """
-        for node in finished_nodes:
+        for name in node_names:
             self._n_finished += 1
-            for successor in node.successors:
-                if successor not in self._nodes:
-                    # If it is last node,
-                    # successor does not exists
+            finished_node = self._name2nodes[name]
+            for edge in finished_node.successors:
+                if not self.check_exists(edge.to_node):
                     continue
 
-                self._name2state[successor].forward()
-                if self._name2state[successor].is_ready:
-                    self._ready_nodes.append(successor)
+                self._name2state[edge.to_node].forward()
+                if self._name2state[edge.to_node].is_ready:
+                    self._ready_nodes.append(self._name2nodes[edge.to_node])
```

## dagstream/graph_components/dags/interface.py

```diff
@@ -1,14 +1,14 @@
 import abc
-from typing import Iterable
+from typing import Iterable, Union
 
-from dagstream.graph_components.nodes import IDrawableNode, IFunctionalNode
+from dagstream.graph_components._interface import IDrawableNode, IFunctionalNode
 
 
 class IDrawableGraph(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def get_drawable_nodes(self) -> Iterable[IDrawableNode]:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def check_exists(self, node: IFunctionalNode) -> bool:
+    def check_exists(self, node: Union[IFunctionalNode, str]) -> bool:
         raise NotImplementedError()
```

## dagstream/graph_components/nodes/__init__.py

```diff
@@ -1,4 +1,2 @@
 # flake8: noqa
 from .functional_node import FunctionalNode
-from .interface import IDrawableNode, IFunctionalNode
-from .node_state import INodeState
```

## dagstream/graph_components/nodes/functional_node.py

```diff
@@ -1,64 +1,101 @@
 from __future__ import annotations
 
-import types
-from typing import Callable
+from typing import Any, Callable, Iterable, Union
 
-from .interface import IDrawableNode, IFunctionalNode
-from .node_state import ReadyNodeState
+from dagstream import utils
+from dagstream.graph_components._interface import (
+    IDagEdge,
+    IDrawableNode,
+    IFunctionalNode,
+)
+from dagstream.graph_components.edges import DagEdge
+from dagstream.graph_components.nodes.node_state import ReadyNodeState
+
+# NOTE: If FunctionalNode has reference to other nodes,
+# one node has almost all information of DAG.
+# It costs too much memory and it is difficult to multi-processing.
+# So, a node has only names about connected ones.
 
 
 class FunctionalNode(IFunctionalNode, IDrawableNode):
-    def __init__(self, user_function: Callable) -> None:
+    def __init__(
+        self, user_function: Callable, *, mut_node_name: Union[str, None] = None
+    ) -> None:
         self._user_function = user_function
-        self._from: set[IFunctionalNode] = set()
-        self._to: set[IFunctionalNode] = set()
-        self._name = self._get_name(user_function)
-
-    def _get_name(self, user_function: Callable) -> str:
-        if isinstance(user_function, types.FunctionType):
-            return user_function.__name__
+        self._from: set[str] = set()
+        self._to_edges: dict[str, IDagEdge] = {}
 
-        return user_function.__class__.__name__
+        if mut_node_name is None:
+            mut_node_name = utils.get_function_name(user_function)
+        self._mut_name = mut_node_name
+        self._display_name = utils.get_function_name(user_function)
+
+        self.__received: list[Any] = []
 
     def __repr__(self) -> str:
-        return f"{FunctionalNode.__name__}:{self.name}"
+        return f"{FunctionalNode.__name__}: {self._display_name}"
+
+    def __hash__(self):
+        return hash(self.mut_name)
 
     @property
-    def name(self) -> str:
-        return self._name
+    def display_name(self) -> str:
+        return self._display_name
 
-    @name.setter
-    def name(self, value: str):
-        self._name = value
+    @display_name.setter
+    def display_name(self, value: str):
+        self._display_name = value
+
+    @property
+    def mut_name(self) -> str:
+        return self._mut_name
 
     @property
     def n_predecessors(self) -> int:
         return len(self._from)
 
     @property
-    def predecessors(self) -> set[IFunctionalNode]:
+    def n_successors(self) -> int:
+        return len(self._to_edges)
+
+    @property
+    def predecessors(self) -> set[str]:
         return self._from
 
     @property
-    def successors(self) -> set[IFunctionalNode]:
-        return self._to
+    def successors(self) -> Iterable[IDagEdge]:
+        return self._to_edges.values()
 
     def prepare(self) -> ReadyNodeState:
+        self.__received = []
         return ReadyNodeState(self.n_predecessors)
 
-    def precede(self, *functions: IFunctionalNode) -> None:
-        for func in functions:
-            if func in self._to:
+    def receive_args(self, val: Any) -> None:
+        self.__received.append(val)
+
+    def get_user_function(self) -> Any:
+        return self._user_function
+
+    def get_received_args(self) -> list[Any]:
+        return self.__received
+
+    def precede(self, *nodes: IFunctionalNode, pipe: bool = False) -> None:
+        for node in nodes:
+            if node.mut_name in self._to_edges:
                 continue
-            self._to.add(func)
-            func.succeed(self)
 
-    def succeed(self, *functions: IFunctionalNode) -> None:
-        for func in functions:
-            if func in self._from:
+            self._to_edges[node.mut_name] = DagEdge(
+                from_node=self.mut_name, to_node=node.mut_name, pipe=pipe
+            )
+            node.succeed(self, pipe=pipe)
+
+    def succeed(self, *nodes: IFunctionalNode, pipe: bool = False) -> None:
+        for node in nodes:
+            if node.mut_name in self._from:
                 continue
-            self._from.add(func)
-            func.precede(self)
+            self._from.add(node.mut_name)
+            node.precede(self, pipe=pipe)
 
     def run(self, *args, **kwargs):
-        return self._user_function(*args, **kwargs)
+        result = self._user_function(*self.__received, *args, **kwargs)
+        return result
```

## dagstream/graph_components/nodes/node_state.py

```diff
@@ -1,33 +1,11 @@
-import abc
-
+from dagstream.graph_components._interface import INodeState
 from dagstream.utils.errors import DagStreamNotReadyError
 
 
-class INodeState(metaclass=abc.ABCMeta):
-    @property
-    @abc.abstractmethod
-    def n_predecessors(self) -> int:
-        raise NotImplementedError()
-
-    @property
-    @abc.abstractmethod
-    def is_ready(self) -> bool:
-        raise NotImplementedError()
-
-    @property
-    @abc.abstractmethod
-    def is_finished(self) -> bool:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def forward(self) -> None:
-        raise NotImplementedError()
-
-
 class UnReadyNodeState(INodeState):
     def __init__(self) -> None:
         pass
 
     @property
     def n_predecessors(self) -> int:
         raise DagStreamNotReadyError()
```

## dagstream/viewers/viewer.py

```diff
@@ -1,24 +1,27 @@
 import abc
 import pathlib
+from typing import Union
 
 from dagstream.graph_components import IDrawableGraph
 
 
 class IDrawer(metaclass=abc.ABCMeta):
     def output(self, graph: IDrawableGraph, file_path: pathlib.Path) -> None:
         raise NotImplementedError()
 
 
 class MermaidDrawer(IDrawer):
     def __init__(self) -> None:
         self._spliter = "\n" + " " * 4
         self._dir = "LR"
 
-    def output(self, graph: IDrawableGraph, file_path: pathlib.Path) -> None:
+    def output(
+        self, graph: IDrawableGraph, file_path: Union[pathlib.Path, str]
+    ) -> None:
         """output content to file_path
 
         Parameters
         ----------
         graph : IDrawableGraph
             graph object to draw
         file_path : pathlib.Path
@@ -30,25 +33,28 @@
 
     def _generate(self, graph: IDrawableGraph) -> str:
         context = ["stateDiagram", f"direction {self._dir}"]
         name2id: dict[str, str] = {}
 
         nodes = graph.get_drawable_nodes()
         for i, node in enumerate(nodes):
-            name2id[node.name] = (state_name := f"state_{i}")
-            context.append(f'state "{node.name}" as {state_name}')
+            name2id[node.mut_name] = (state_name := f"state_{i}")
+            context.append(f'state "{node.display_name}" as {state_name}')
 
         for i, node in enumerate(nodes):
-            state_name = name2id[node.name]
+            state_name = name2id[node.mut_name]
             if node.n_predecessors == 0:
                 context.append(f"[*] --> {state_name}")
 
-            succesors = [v for v in node.successors if graph.check_exists(v)]
+            succesors = [v for v in node.successors if graph.check_exists(v.to_node)]
             if len(succesors) == 0:
                 context.append(f"{state_name} --> [*]")
                 continue
 
             for successor in succesors:
-                successor_state = name2id[successor.name]
-                context.append(f"{state_name} --> {successor_state}")
+                successor_state = name2id[successor.to_node]
+                if successor.is_pipe:
+                    context.append(f"{state_name} --> {successor_state}: Pipe")
+                else:
+                    context.append(f"{state_name} --> {successor_state}")
 
         return self._spliter.join(context)
```

## Comparing `dagstream/graph_components/nodes/interface.py` & `dagstream/graph_components/_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,124 @@
 from __future__ import annotations
 
 import abc
-from typing import Any
-
-from .node_state import INodeState
+from typing import Any, Iterable
 
 
 class IDrawableNode(metaclass=abc.ABCMeta):
     @property
     @abc.abstractmethod
-    def name(self) -> str:
-        raise NotImplementedError()
+    def display_name(self) -> str:
+        ...
 
     @property
     @abc.abstractmethod
-    def successors(self) -> set[IFunctionalNode]:
-        raise NotImplementedError()
+    def mut_name(self) -> str:
+        ...
+
+    @property
+    @abc.abstractmethod
+    def successors(self) -> Iterable[IDagEdge]:
+        ...
 
     @property
     @abc.abstractmethod
     def n_predecessors(self) -> int:
-        raise NotImplementedError()
+        ...
 
 
 class IFunctionalNode(IDrawableNode, metaclass=abc.ABCMeta):
     @property
     @abc.abstractmethod
-    def name(self) -> str:
-        raise NotImplementedError()
+    def display_name(self) -> str:
+        ...
 
-    @name.setter
+    @display_name.setter
     @abc.abstractmethod
-    def name(self) -> None:
-        raise NotImplementedError()
+    def display_name(self) -> None:
+        ...
 
     @property
     @abc.abstractmethod
-    def predecessors(self) -> set[IFunctionalNode]:
-        raise NotImplementedError()
+    def mut_name(self) -> str:
+        ...
 
     @property
     @abc.abstractmethod
-    def successors(self) -> set[IFunctionalNode]:
-        raise NotImplementedError()
+    def predecessors(self) -> set[str]:
+        ...
+
+    @property
+    @abc.abstractmethod
+    def successors(self) -> Iterable[IDagEdge]:
+        ...
 
     @property
     @abc.abstractmethod
     def n_predecessors(self) -> int:
-        raise NotImplementedError()
+        ...
+
+    @property
+    @abc.abstractmethod
+    def n_successors(self) -> int:
+        ...
+
+    @abc.abstractmethod
+    def precede(self, *nodes: IFunctionalNode, pipe: bool = False) -> None:
+        ...
+
+    @abc.abstractmethod
+    def succeed(self, *nodes: IFunctionalNode, pipe: bool = False) -> None:
+        ...
+
+    @abc.abstractmethod
+    def prepare(self) -> INodeState:
+        ...
+
+    @abc.abstractmethod
+    def receive_args(self, val: Any) -> None:
+        ...
+
+    @abc.abstractmethod
+    def get_received_args(self) -> list[Any]:
+        ...
+
+    @abc.abstractmethod
+    def get_user_function(self) -> Any:
+        ...
+
+    @abc.abstractmethod
+    def run(self, *args, **kwargs) -> Any:
+        ...
+
 
+class INodeState(metaclass=abc.ABCMeta):
+    @property
     @abc.abstractmethod
-    def precede(self, *functions: IFunctionalNode) -> None:
+    def n_predecessors(self) -> int:
         raise NotImplementedError()
 
+    @property
     @abc.abstractmethod
-    def succeed(self, *functions: IFunctionalNode) -> None:
+    def is_ready(self) -> bool:
         raise NotImplementedError()
 
+    @property
     @abc.abstractmethod
-    def prepare(self) -> INodeState:
+    def is_finished(self) -> bool:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def run(self, *args, **kwargs) -> Any:
+    def forward(self) -> None:
         raise NotImplementedError()
+
+
+class IDagEdge(metaclass=abc.ABCMeta):
+    @property
+    @abc.abstractmethod
+    def is_pipe(self) -> bool:
+        ...
+
+    @property
+    @abc.abstractmethod
+    def to_node(self) -> str:
+        ...
```

## Comparing `dagstream-0.1.4.dist-info/LICENSE` & `dagstream-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dagstream-0.1.4.dist-info/METADATA` & `dagstream-0.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagstream
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Home-page: https://github.com/ricosjp/dagstream
 License: Apache-2.0
 Author: sakamoto
 Author-email: sakamoto@ricos.co.jp
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `dagstream-0.1.4.dist-info/RECORD` & `dagstream-0.1.5.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-pyproject.toml,sha256=MAfL_kAFZWrUwMT6abpOrzSNUnJdiyvb1_GIL6pjq7I,880
+pyproject.toml,sha256=tiqKCk67XJS7uYKH6ljZJ-Z2DXd0PnieXGEzu1QrvLM,1011
 dagstream/__init__.py,sha256=7XZXKHfQ0-ntevS22INjkiJ1FH1fhGoMWEmg_6llJlY,145
-dagstream/dagstream.py,sha256=K5SOEl-sDQDBMw8VO-gOCpuk7HJdpOHx9i8bvWB0sog,3674
-dagstream/executor.py,sha256=i65Bx8RZMeHOV16xr0n5rnvqPCgzr_v9mo12HSVTrec,4713
-dagstream/graph_components/__init__.py,sha256=enJTDKoCf97EgekcN_umujqMFm9CoUhckm5Z2judxNY,82
+dagstream/dagstream.py,sha256=mQ-sXx3ufP1b9WCus8oA9rthjBwP7VaoakvDVgDSCJc,4831
+dagstream/executor.py,sha256=Aze7J31s4XMgTrHsQR3SMlhxOoLvwQUNDIpYM4lLTwU,5140
+dagstream/graph_components/__init__.py,sha256=C6Grt6QNMRe41fbbZSZ_9onKmPcU07LhMpKUgRMtg24,206
+dagstream/graph_components/_interface.py,sha256=USdzisNpcAuM_YWMZLfB8TnluZBT-UA333aEYSqiZhQ,2461
 dagstream/graph_components/dags/__init__.py,sha256=8XXuNbq-HMmgDztEK0cN1CV1IBtLASq9myQV8UHKxeM,96
-dagstream/graph_components/dags/functional_dag.py,sha256=PFv79bcS00zj3Uu5XfzcWIu3SVjygHQzhIOaxFAeSQQ,2218
-dagstream/graph_components/dags/interface.py,sha256=xgsyiIFtkx9iakirukD4tRv492Bdz1pMRMqmakwrF6c,404
-dagstream/graph_components/nodes/__init__.py,sha256=XC9RoOaGcGzNs1IiZXeTVxtabNNc_X0iCK1W9N6xKkE,148
-dagstream/graph_components/nodes/functional_node.py,sha256=ax_UtoZSheSBgJM03CMi_Xgry9R-X19qOzKfjVCdFcY,1790
-dagstream/graph_components/nodes/interface.py,sha256=tUXRf5bx9nzsTzFe1v9x6jzsLx5hAbkI7Y037lI_-Tw,1568
-dagstream/graph_components/nodes/node_state.py,sha256=VMVo1cBdWc9jI_5F_DDNhwPfXSzYI-fsOqRqVgWLqRs,1402
+dagstream/graph_components/dags/functional_dag.py,sha256=F6mVwLGdsorkDiDu7LUXkZHEhMOaAPAie1XICgjRduc,3514
+dagstream/graph_components/dags/interface.py,sha256=TNEIYzJOhlnLog_F8a2NSz5QO-PT1SXyDSWLfDzUJro,428
+dagstream/graph_components/edges/__init__.py,sha256=_zvnYULxs3QkSTsuHIVXN1N2UvGC1sIheLGLQokboKo,27
+dagstream/graph_components/edges/_edge.py,sha256=rgVYSRGjSaSBsJ9rmKj-jWbp5vu2y5IS8vmT51nb3gg,385
+dagstream/graph_components/nodes/__init__.py,sha256=IJwTayppLPhwSEHwPD0XrAAS3t0QLd3FNP-vPbe4LoA,59
+dagstream/graph_components/nodes/functional_node.py,sha256=0qf-LYJ86OX-OdgDa1ZthVJuEhX1xxx36mI3YX4g6Zo,2996
+dagstream/graph_components/nodes/node_state.py,sha256=7yK3JevUbYmaHtrB9Cz6T4qTswTEQX_dJcE3bH-0NP0,988
+dagstream/utils/__init__.py,sha256=k04gSE3zlwU2K7iRdw54qgkAnXLgEGojsgyKLgomgj0,36
 dagstream/utils/errors.py,sha256=v70Mef1AC6Lv2r1Dr56_eZ4HWoVVLC2AC6TL87f4HzE,309
+dagstream/utils/util.py,sha256=0fkXsx4zS5MYzJWVnDDUXQJH6wUAQoAZ-PSXYwz5L9k,248
 dagstream/version.py,sha256=52eq0hdOZ19xMJqe7e4sVjLkwbVTMZhaGwPK5PqLPeM,81
 dagstream/viewers/__init__.py,sha256=sMCw2RCj1BibKpUNcT2PezpsIFJ6leFPTguuUcUr-SI,51
-dagstream/viewers/viewer.py,sha256=iPRiToUZXT6-to-xPWA6WDhdRRLekWQzmKWL60WviOg,1725
-dagstream-0.1.4.dist-info/LICENSE,sha256=t0fJJ7NyvQCuqIIIJwoYAzXhtjvuFf6g34ppElQCGr0,549
-dagstream-0.1.4.dist-info/METADATA,sha256=OGeGKWs4nX-G5ROMJmD9iETKkqYPMJUELaX9vAbx4a8,2753
-dagstream-0.1.4.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-dagstream-0.1.4.dist-info/RECORD,,
+dagstream/viewers/viewer.py,sha256=Ib05rN0NSy8xNIL2yP_wM2xROfnUIEedYnquajyjdJw,1947
+dagstream-0.1.5.dist-info/LICENSE,sha256=t0fJJ7NyvQCuqIIIJwoYAzXhtjvuFf6g34ppElQCGr0,549
+dagstream-0.1.5.dist-info/METADATA,sha256=eJt-DQoWAh5uMwghLdxkNriNOBDZM3YG7kgqwA_i88Q,2753
+dagstream-0.1.5.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+dagstream-0.1.5.dist-info/RECORD,,
```

