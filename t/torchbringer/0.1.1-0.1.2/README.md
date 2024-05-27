# Comparing `tmp/torchbringer-0.1.1.tar.gz` & `tmp/torchbringer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbringer-0.1.1.tar", last modified: Sun May 26 16:29:47 2024, max compression
+gzip compressed data, was "torchbringer-0.1.2.tar", last modified: Sun May 26 16:34:07 2024, max compression
```

## Comparing `torchbringer-0.1.1.tar` & `torchbringer-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-25 23:44:21.000000 torchbringer-0.1.1/LICENSE
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7056 2024-05-26 16:29:47.686786 torchbringer-0.1.1/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6287 2024-05-26 16:19:58.000000 torchbringer-0.1.1/README.md
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-26 16:29:47.686786 torchbringer-0.1.1/setup.cfg
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1130 2024-05-26 16:29:29.000000 torchbringer-0.1.1/setup.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-26 16:29:37.000000 torchbringer-0.1.1/torchbringer/__init__.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer/components/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2757 2024-05-26 15:48:03.000000 torchbringer-0.1.1/torchbringer/components/builders.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      610 2024-05-25 16:10:22.000000 torchbringer-0.1.1/torchbringer/components/epsilon.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-25 17:27:12.000000 torchbringer-0.1.1/torchbringer/components/replay_memory.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer/examples/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-26 15:39:23.000000 torchbringer-0.1.1/torchbringer/examples/cartpole_grpc_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-26 15:39:22.000000 torchbringer-0.1.1/torchbringer/examples/cartpole_local_dqn.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer/learners/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     4941 2024-05-26 15:47:32.000000 torchbringer-0.1.1/torchbringer/learners/dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-25 15:17:44.000000 torchbringer-0.1.1/torchbringer/learners/learner_utils.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer/servers/
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer/servers/grpc/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-26 15:38:36.000000 torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_grpc_client.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-26 15:41:48.000000 torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_grpc_server.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-26 15:50:10.000000 torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_pb2.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-26 15:50:10.000000 torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_pb2.pyi
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-26 15:52:44.000000 torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      583 2024-05-26 15:38:36.000000 torchbringer-0.1.1/torchbringer/servers/torchbringer_agent.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer.egg-info/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7056 2024-05-26 16:29:47.000000 torchbringer-0.1.1/torchbringer.egg-info/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      792 2024-05-26 16:29:47.000000 torchbringer-0.1.1/torchbringer.egg-info/SOURCES.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-26 16:29:47.000000 torchbringer-0.1.1/torchbringer.egg-info/dependency_links.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       84 2024-05-26 16:29:47.000000 torchbringer-0.1.1/torchbringer.egg-info/requires.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-26 16:29:47.000000 torchbringer-0.1.1/torchbringer.egg-info/top_level.txt
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.506785 torchbringer-0.1.2/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-25 23:44:21.000000 torchbringer-0.1.2/LICENSE
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7296 2024-05-26 16:34:07.506785 torchbringer-0.1.2/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6527 2024-05-26 16:33:08.000000 torchbringer-0.1.2/README.md
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-26 16:34:07.506785 torchbringer-0.1.2/setup.cfg
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1130 2024-05-26 16:34:01.000000 torchbringer-0.1.2/setup.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.496785 torchbringer-0.1.2/torchbringer/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-26 16:34:01.000000 torchbringer-0.1.2/torchbringer/__init__.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.496785 torchbringer-0.1.2/torchbringer/components/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2757 2024-05-26 15:48:03.000000 torchbringer-0.1.2/torchbringer/components/builders.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      610 2024-05-25 16:10:22.000000 torchbringer-0.1.2/torchbringer/components/epsilon.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-25 17:27:12.000000 torchbringer-0.1.2/torchbringer/components/replay_memory.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.496785 torchbringer-0.1.2/torchbringer/examples/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-26 15:39:23.000000 torchbringer-0.1.2/torchbringer/examples/cartpole_grpc_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-26 15:39:22.000000 torchbringer-0.1.2/torchbringer/examples/cartpole_local_dqn.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.496785 torchbringer-0.1.2/torchbringer/learners/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     4941 2024-05-26 15:47:32.000000 torchbringer-0.1.2/torchbringer/learners/dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-25 15:17:44.000000 torchbringer-0.1.2/torchbringer/learners/learner_utils.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.496785 torchbringer-0.1.2/torchbringer/servers/
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.506785 torchbringer-0.1.2/torchbringer/servers/grpc/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-26 15:38:36.000000 torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_grpc_client.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-26 15:41:48.000000 torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_grpc_server.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-26 15:50:10.000000 torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_pb2.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-26 15:50:10.000000 torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_pb2.pyi
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-26 15:52:44.000000 torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      583 2024-05-26 15:38:36.000000 torchbringer-0.1.2/torchbringer/servers/torchbringer_agent.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.506785 torchbringer-0.1.2/torchbringer.egg-info/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7296 2024-05-26 16:34:07.000000 torchbringer-0.1.2/torchbringer.egg-info/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      792 2024-05-26 16:34:07.000000 torchbringer-0.1.2/torchbringer.egg-info/SOURCES.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-26 16:34:07.000000 torchbringer-0.1.2/torchbringer.egg-info/dependency_links.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       84 2024-05-26 16:34:07.000000 torchbringer-0.1.2/torchbringer.egg-info/requires.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-26 16:34:07.000000 torchbringer-0.1.2/torchbringer.egg-info/top_level.txt
```

### Comparing `torchbringer-0.1.1/LICENSE` & `torchbringer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/PKG-INFO` & `torchbringer-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -31,14 +31,15 @@
 To install TorchBringer, run
 
 ```bash
 pip install --upgrade pip
 pip install torchbringer
 ```
 
+### Local
 Here's a simple project for running a TorchBringer agent on gymnasium's Cartpole environment.
 
 ```python
 import gymnasium as gym
 from itertools import count
 import torch
 from torchbringer.servers.torchbringer_agent import TorchBringerAgent
@@ -69,35 +70,46 @@
         terminal = terminated or truncated
 
         if terminal:
             dqn.step(state, reward, terminal)
             break
 ```
 
+### Server
+To start a TorchBringer server on a particular port, run
+
+```bash
+python -m torchbringer.servers.grpc.torchbringer_grpc_server <PORT>
+```
+
+You can communicate with this server by using the provided Python client (see below) or develop a client of your own from the files found in `torchbringer/servers/grpc` in this repo to communicate with the server from applications built with different programming languages. 
+
+```python
+from torchbringer.servers.grpc.torchbringer_grpc_client import TorchBringerGRPCAgentClient
+```
+
 ## Reference
 
 `cartpole_local_dqn.py` provides a simple example of TorchBringer being used on gymnasium's CartPole-v1 envinronment. `cartpole_grpc_dqn.py` provides an example of how to use the gRPC interface to learn remotely.
 
 The main class that is used in this framework is `TorchBringerAgent`, implemented in `servers/`. The gRPC server has an interface very similar to it.
 
 ### TorchBringerAgent
 | Method | Parameters | Explanation |
 |---|---|---|
 | initialize() | config: dict | Initializes the agent according to the config. Read the config section for information on formatting |
 | step() | state: Tensor, reward: Tensor, terminal: bool | Performs an optimization step and returns the selected action for this  |
-| experience_and_optimize() | state: Tensor, reward: Tensor, terminal: bool | Performs an optimization step without selecting an action |
 
 ### gRPC interface
 Note that there is a client implemented in `servers/torchbringer_grpc_client.py` that has the exact same interface as `TorchBringerAgent`. This reference is mostly meant for building clients in other programming languages.
 
 | Method | Parameters | Explanation |
 |---|---|---|
 | initialize() | config: string | Accepts a serialized config dict |
 | step() | state: Matrix(dimensions list[int], value: list[float]), reward: float, terminal: bool | State should be given as a flattened matrix, action is returned the same way  |
-| experience_and_optimize() | state: Matrix(dimensions list[int], value: list[float]), reward: float, terminal: bool | State should be given as a flattened matrix |
 
 ## Config formatting
 The config file is a dictionary that specifies the behavior of the agent. The RL implementation is specified by the value of the key "type". It also accepts a variety of other arguments depending on the imeplementation type.
 
 Currently supported implementations are `dqn`.
 
 The following specify the arguments allowed by each implementation type.
```

### Comparing `torchbringer-0.1.1/README.md` & `torchbringer-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 To install TorchBringer, run
 
 ```bash
 pip install --upgrade pip
 pip install torchbringer
 ```
 
+### Local
 Here's a simple project for running a TorchBringer agent on gymnasium's Cartpole environment.
 
 ```python
 import gymnasium as gym
 from itertools import count
 import torch
 from torchbringer.servers.torchbringer_agent import TorchBringerAgent
@@ -45,35 +46,46 @@
         terminal = terminated or truncated
 
         if terminal:
             dqn.step(state, reward, terminal)
             break
 ```
 
+### Server
+To start a TorchBringer server on a particular port, run
+
+```bash
+python -m torchbringer.servers.grpc.torchbringer_grpc_server <PORT>
+```
+
+You can communicate with this server by using the provided Python client (see below) or develop a client of your own from the files found in `torchbringer/servers/grpc` in this repo to communicate with the server from applications built with different programming languages. 
+
+```python
+from torchbringer.servers.grpc.torchbringer_grpc_client import TorchBringerGRPCAgentClient
+```
+
 ## Reference
 
 `cartpole_local_dqn.py` provides a simple example of TorchBringer being used on gymnasium's CartPole-v1 envinronment. `cartpole_grpc_dqn.py` provides an example of how to use the gRPC interface to learn remotely.
 
 The main class that is used in this framework is `TorchBringerAgent`, implemented in `servers/`. The gRPC server has an interface very similar to it.
 
 ### TorchBringerAgent
 | Method | Parameters | Explanation |
 |---|---|---|
 | initialize() | config: dict | Initializes the agent according to the config. Read the config section for information on formatting |
 | step() | state: Tensor, reward: Tensor, terminal: bool | Performs an optimization step and returns the selected action for this  |
-| experience_and_optimize() | state: Tensor, reward: Tensor, terminal: bool | Performs an optimization step without selecting an action |
 
 ### gRPC interface
 Note that there is a client implemented in `servers/torchbringer_grpc_client.py` that has the exact same interface as `TorchBringerAgent`. This reference is mostly meant for building clients in other programming languages.
 
 | Method | Parameters | Explanation |
 |---|---|---|
 | initialize() | config: string | Accepts a serialized config dict |
 | step() | state: Matrix(dimensions list[int], value: list[float]), reward: float, terminal: bool | State should be given as a flattened matrix, action is returned the same way  |
-| experience_and_optimize() | state: Matrix(dimensions list[int], value: list[float]), reward: float, terminal: bool | State should be given as a flattened matrix |
 
 ## Config formatting
 The config file is a dictionary that specifies the behavior of the agent. The RL implementation is specified by the value of the key "type". It also accepts a variety of other arguments depending on the imeplementation type.
 
 Currently supported implementations are `dqn`.
 
 The following specify the arguments allowed by each implementation type.
```

### Comparing `torchbringer-0.1.1/setup.py` & `torchbringer-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='torchbringer',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.1.1',    
+    version='0.1.2',    
     description='A PyTorch library for deep reinforcement learning ',
     url='https://github.com/moraguma/TorchBringer',
     author='Moraguma',
     author_email='g170603@dac.unicamp.br',
     license='MIT',
     packages=find_namespace_packages(),
     install_requires=[
```

### Comparing `torchbringer-0.1.1/torchbringer/components/builders.py` & `torchbringer-0.1.2/torchbringer/components/builders.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/torchbringer/components/epsilon.py` & `torchbringer-0.1.2/torchbringer/components/epsilon.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/torchbringer/components/replay_memory.py` & `torchbringer-0.1.2/torchbringer/components/replay_memory.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/torchbringer/examples/cartpole_grpc_dqn.py` & `torchbringer-0.1.2/torchbringer/examples/cartpole_grpc_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/torchbringer/examples/cartpole_local_dqn.py` & `torchbringer-0.1.2/torchbringer/examples/cartpole_local_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/torchbringer/learners/dqn.py` & `torchbringer-0.1.2/torchbringer/learners/dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_grpc_client.py` & `torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_grpc_client.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_grpc_server.py` & `torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_grpc_server.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_pb2.py` & `torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_pb2.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_pb2.pyi` & `torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_pb2_grpc.py` & `torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/torchbringer/servers/torchbringer_agent.py` & `torchbringer-0.1.2/torchbringer/servers/torchbringer_agent.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.1/torchbringer.egg-info/PKG-INFO` & `torchbringer-0.1.2/torchbringer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -31,14 +31,15 @@
 To install TorchBringer, run
 
 ```bash
 pip install --upgrade pip
 pip install torchbringer
 ```
 
+### Local
 Here's a simple project for running a TorchBringer agent on gymnasium's Cartpole environment.
 
 ```python
 import gymnasium as gym
 from itertools import count
 import torch
 from torchbringer.servers.torchbringer_agent import TorchBringerAgent
@@ -69,35 +70,46 @@
         terminal = terminated or truncated
 
         if terminal:
             dqn.step(state, reward, terminal)
             break
 ```
 
+### Server
+To start a TorchBringer server on a particular port, run
+
+```bash
+python -m torchbringer.servers.grpc.torchbringer_grpc_server <PORT>
+```
+
+You can communicate with this server by using the provided Python client (see below) or develop a client of your own from the files found in `torchbringer/servers/grpc` in this repo to communicate with the server from applications built with different programming languages. 
+
+```python
+from torchbringer.servers.grpc.torchbringer_grpc_client import TorchBringerGRPCAgentClient
+```
+
 ## Reference
 
 `cartpole_local_dqn.py` provides a simple example of TorchBringer being used on gymnasium's CartPole-v1 envinronment. `cartpole_grpc_dqn.py` provides an example of how to use the gRPC interface to learn remotely.
 
 The main class that is used in this framework is `TorchBringerAgent`, implemented in `servers/`. The gRPC server has an interface very similar to it.
 
 ### TorchBringerAgent
 | Method | Parameters | Explanation |
 |---|---|---|
 | initialize() | config: dict | Initializes the agent according to the config. Read the config section for information on formatting |
 | step() | state: Tensor, reward: Tensor, terminal: bool | Performs an optimization step and returns the selected action for this  |
-| experience_and_optimize() | state: Tensor, reward: Tensor, terminal: bool | Performs an optimization step without selecting an action |
 
 ### gRPC interface
 Note that there is a client implemented in `servers/torchbringer_grpc_client.py` that has the exact same interface as `TorchBringerAgent`. This reference is mostly meant for building clients in other programming languages.
 
 | Method | Parameters | Explanation |
 |---|---|---|
 | initialize() | config: string | Accepts a serialized config dict |
 | step() | state: Matrix(dimensions list[int], value: list[float]), reward: float, terminal: bool | State should be given as a flattened matrix, action is returned the same way  |
-| experience_and_optimize() | state: Matrix(dimensions list[int], value: list[float]), reward: float, terminal: bool | State should be given as a flattened matrix |
 
 ## Config formatting
 The config file is a dictionary that specifies the behavior of the agent. The RL implementation is specified by the value of the key "type". It also accepts a variety of other arguments depending on the imeplementation type.
 
 Currently supported implementations are `dqn`.
 
 The following specify the arguments allowed by each implementation type.
```

### Comparing `torchbringer-0.1.1/torchbringer.egg-info/SOURCES.txt` & `torchbringer-0.1.2/torchbringer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

